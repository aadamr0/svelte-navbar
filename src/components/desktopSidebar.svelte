<div class="sidebar">
    <div class="sidebar-section top"> <p>logo</p> </div>
    <div class="sidebar-section mid">
        <nav>
            <a href="/">Home</a>
            <a href="/about">About</a>
        </nav>
    </div>
    <div class="sidebar-section low"></div>
</div>

<style>
    .sidebar {
        width: 100%;
        height: 100%;
        display: flex;
        flex-direction: column;
        border-right: 1px solid grey;
    }

    .sidebar-section {
        flex-basis: 33%;
    }

    .top, .mid {
        border-bottom: 1px solid grey;
    }
</style>
