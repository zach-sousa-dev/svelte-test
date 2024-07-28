<script>
    import logo from './assets/appLogoFull.svg';
    import Div from './lib/Div.svelte';

    const songList =    [
                            {
                                'name': 'The Real Slim Shady',
                                'artist': 'Eminem'
                            },

                            {
                                'name': 'Lose Yourself',
                                'artist': 'Eminem'
                            },

                            {
                                'name': 'Purple Pills',
                                'artist': 'D12'
                            }
                        ];
</script>

<main>
    <img src={logo} alt="Logo for app called trackIt">
    
    {#if 1+1 == 2}
        <p>1+1 does, in fact, equal 2.</p>
    {:else}
        <p>Else...</p>
    {/if}

    {#each songList as song}
        <p><b>SONG:</b> {song.name} <b>ARTIST:</b> {song.artist}</p>
    {/each}

    <Div text="This is a component." />
</main>