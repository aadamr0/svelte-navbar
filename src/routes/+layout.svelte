<script>
    import Header from '../components/header.svelte'
    import Sidebar from '../components/desktopSidebar.svelte'

    import '../globals.css'
</script>


<div id="app">
    <div class="header-div"><Header /></div> 
    <div class="sidebar-div"><Sidebar /></div>
    <div class="content"><slot /></div>
</div>


<style>

    #app {
        display: flex;
    }

    .sidebar-div {
        flex-basis: 20%;
    }

    .header-div {
        display: none;
    }

    @media only screen and (max-width: 768px) {

        #app {
            flex-direction: column;
        }

        .header-div {
            display: block;
        }

        .sidebar-div {
            display: none;
        }
    }
</style>