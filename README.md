fetch(new Request('https://github.com',{
    method:'POST',
    headers: {'Content-Type' : 'application/x-www-form-urlencoded'},
    body : "/login/oauth/access_tokenclient_id=5df8ed462d8ae416eb1a&scope=repo&client_secret=43f47a1b8f96868e18d9af30a058f27a8a02a883&code=fdc20ab510c719a7f3d8"
})).then((resp)=>{console.log(resp)})


axios({
  method: 'post',
    url: 'https://github.com/login/oauth/access_token\?client_id=5df8ed462d8ae416eb1a&scope=repo&client_secret=43f47a1b8f96868e18d9af30a058f27a8a02a883&code=fdc20ab510c719a7f3d8',
    headers: {
      accept: 'application/json',
    }
})
.then(function(response) {
  console.log(response);
})
.catch(function (error) { 
   console.log('error',error);
});
