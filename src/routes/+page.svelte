<script>
    function authorizeMyAnimeList() {
        const clientId = ''; 
        const redirectUri = encodeURIComponent(''); 
        const responseType = 'token';
        const state = ''; 
        const scope = 'write:users';

        const authorizationUrl = `https://myanimelist.net/v1/oauth2/authorize?response_type=${responseType}&client_id=${clientId}&redirect_uri=${redirectUri}&state=${state}&scope=${scope}`;

        window.location.href = authorizationUrl;
    }
</script>

<button on:click={authorizeMyAnimeList}>Authorize MyAnimeList</button>
