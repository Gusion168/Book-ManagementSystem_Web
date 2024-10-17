<script>
	import Sidebar from "./components/sidebar.svelte";
	import { Router, Route } from 'svelte-routing';
	import LibraryPage from "./pages/library_page.svelte";
	import AddItemPage from "./pages/addItem_page.svelte";
	import DashboardPage from "./pages/dashboard.svelte";
	import AddCollectionPage from "./pages/addCollection_page.svelte";
    import PublishPage from "./pages/publish_page.svelte";
    import Dashboard from "./pages/dashboard.svelte";
    import SettingPage from "./pages/setting_page.svelte"
    import SupportPage from "./pages/support_page.svelte"
      </script>
      
      <main>
	<Router>
	    <Sidebar title="My Book Management System" />
	    <Route path="/library" component={LibraryPage} />
	    <Route path="/addItem" component={AddItemPage}/>
	    <Route path="/add-collection" component={AddCollectionPage}/>
	    <Route path="/publish" component={PublishPage}/>
	    <Route path="/dashboards" component={Dashboard}/>
	    <Route path="/settings" component={SettingPage}/>
	    <Route path="/support" component={SupportPage}/>

	</Router>
      </main>
      
      <style>
	main {
	    text-align: center;
	    padding: 1em;
	    max-width: 240px;
	    margin: 0 auto;
	}
      
	
      
	@media (min-width: 640px) {
	    main {
	        max-width: none;
	    }
	}
      </style>
      