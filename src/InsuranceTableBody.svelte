<script>
    let tableContent = [
            {
            "name": 'Title of post',
                "categories": ['Category 1'],
                "publishDate": 'Oct 27 13:49',
                "modifiedDate": 'Oct 27 12:49',
            },
            {
            "name": 'Title of post',
                "categories": ['Category 1'],
                "publishDate": 'Oct 27 13:49',
                "modifiedDate": 'Oct 27 12:49',
            },
            {
            "name": 'Title of post',
                "categories": ['Category 1'],
                "publishDate": 'Oct 27 13:49',
                "modifiedDate": 'Oct 27 12:49',
            },
            {
            "name": 'Title of post',
                "categories": ['Category 1'],
                "publishDate": 'Oct 27 13:49',
                "modifiedDate": 'Oct 27 12:49',
            },
            {
            "name": 'Title of post',
                "categories": ['Category 1'],
                "publishDate": 'Oct 27 13:49',
                "modifiedDate": 'Oct 27 12:49',
            },
            {
            "name": 'Title of post',
                "categories": ['Category 1'],
                "publishDate": 'Oct 27 13:49',
                "modifiedDate": 'Oct 27 12:49',
            },
            {
            "name": 'Title of post',
                "categories": ['Category 1'],
                "publishDate": 'Oct 27 13:49',
                "modifiedDate": 'Oct 27 12:49',
            },
            {
            "name": 'Title of post',
                "categories": ['Category 1'],
                "publishDate": 'Oct 27 13:49',
                "modifiedDate": 'Oct 27 12:49',
            },
            {
            "name": 'Title of post',
                "categories": ['Category 1'],
                "publishDate": 'Oct 27 13:49',
                "modifiedDate": 'Oct 27 12:49',
            },
            {
            "name": 'Title of post',
                "categories": ['Category 1'],
                "publishDate": 'Oct 27 13:49',
                "modifiedDate": 'Oct 27 12:49',
            },
            {
            "name": 'Title of post',
                "categories": ['Category 1'],
                "publishDate": 'Oct 27 13:49',
                "modifiedDate": 'Oct 27 12:49',
            },
            {
            "name": 'Title of post',
                "categories": ['Category 1'],
                "publishDate": 'Oct 27 13:49',
                "modifiedDate": 'Oct 27 12:49',
            },
            {
            "name": 'Title of post',
                "categories": ['Category 1'],
                "publishDate": 'Oct 27 13:49',
                "modifiedDate": 'Oct 27 12:49',
            },
            {
            "name": 'Title of post',
                "categories": ['Category 1'],
                "publishDate": 'Oct 27 13:49',
                "modifiedDate": 'Oct 27 12:49',
            },
            {
            "name": 'Title of post',
                "categories": ['Category 1'],
                "publishDate": 'Oct 27 13:49',
                "modifiedDate": 'Oct 27 12:49',
            },
            {
            "name": 'Title of post',
                "categories": ['Category 1'],
                "publishDate": 'Oct 27 13:49',
                "modifiedDate": 'Oct 27 12:49',
            },
            {
            "name": 'Title of post',
                "categories": ['Category 1'],
                "publishDate": 'Oct 27 13:49',
                "modifiedDate": 'Oct 27 12:49',
            },
            {
            "name": 'Title of post',
                "categories": ['Category 1'],
                "publishDate": 'Oct 27 13:49',
                "modifiedDate": 'Oct 27 12:49',
            },
        ];
</script>

<main>
    <table class="table">
        <tbody>
            {#each tableContent as row}
            <tr>
                <td>{row.name}</td>
                <td>
                    {#each row.categories as category, index}
                        {category}{#if index != row.categories.length - 1},&nbsp{/if}
                    {/each}
                </td>
                <td>{row.publishDate}</td>
                <td>{row.modifiedDate}</td>
            </tr>
            {/each}
        </tbody>
    </table>
</main>

<style>    
    main{
        height: 100vh;
    }
</style>