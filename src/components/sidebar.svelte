<script>
  export let title = "Sidebar Title";
  import { Link } from 'svelte-routing';
</script>

<style>
  .sidebar {
      width: 250px;
      height: 100vh;
      background-color: #f4f4f4;
      padding: 1rem;
      position: fixed;
      left: 0;
      top: 0;
      overflow-y: auto;
  }

  .sidebar ul {
      list-style-type: none;
      padding: 0;
  }

  .sidebar li {
      margin: 1rem 0;
  }

  
</style>

<div class="sidebar">
  <h2>{title}</h2>
  <ul>
      <li><Link to="/library">Library</Link></li>
      <li><Link to="/addItem">Add Items</Link></li>
      
      <li><Link to="/add-collection">Add Collection</Link></li>
      <li><Link to="/publish">Publish</Link></li>
      <li><Link to="/dashboards">Dashboards</Link></li>
      <br><br>
      <li><Link to="/settings">Settings</Link></li>
      <li><Link to="/support">Support</Link></li>
  </ul>
</div>
