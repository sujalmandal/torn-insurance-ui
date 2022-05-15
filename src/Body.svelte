<script>
    import InsuranceTableBody from './InsuranceTableBody.svelte';
    import Icon from 'svelte-awesome';
    import { refresh, filter, search} from 'svelte-awesome/icons';
</script>    

<main>
    <div id="main-content" class="container">
      <div class="row">
          <div class="col-10">
            <!-- table header -->
            <div class="row">
              <table style="margin-left:2vw">
                <thead>
                  <tr>
                      <th>Name</th>
                      <th>Categories</th>
                      <th>Publish date</th>
                      <th>Modified date</th>
                  </tr>
                </thead>
              </table>  
            </div>
            <div style="overflow-y: scroll; max-height: 75vh;">
              <InsuranceTableBody/>
            </div>
          </div>
          <div class="col-2">
            <div class="container">
              <div class="row">
                <button>Update <span style="margin-left: 0.5vh;"><Icon data={refresh}/></span></button>
              </div>
              <div class="row" style="border-style: hidden; padding: 1em;">
                <input type="text" class="row" placeholder="player name"/>
                <div class="row">Insurance status</div>
                <select class="row">
                  <option>-- All --</option>
                  <option>Claimable</option>
                  <option>Expired</option>
                  <option>Settled</option>
                </select>
                <div class="row">Date from</div>
                <div class="row">
                  <input type="date"/>
                </div>
                <div class="row">Date to</div>
                <div class="row"><input type="date"/></div>
              </div>
              <div class="row">
                <button>Search Insurance <Icon data={search}></Icon></button>
              </div>
          </div>
          </div>
    </div>
    </div> 
</main>

<style>

	main {
		text-align: center;
		padding: 1em;
		max-width: 100vw;
  }
   
</style>