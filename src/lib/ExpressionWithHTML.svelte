<script>
    const user = {
        loggedIn : true
    }
    const toggle = ()=>{
        user.loggedIn = !user.loggedIn
    }
</script>
{#if user.loggedIn}
<button on:click={toggle}>
	Log out
</button>
{/if}
{#if !user.loggedIn}
<button on:click={toggle}>
	Log in
</button>
{/if}