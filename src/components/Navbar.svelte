<script lang="ts">
    import TopAppBar from '@smui/top-app-bar';
    import TopAppBarRow from '@smui/top-app-bar'; 
    import TopAppBarSection from '@smui/top-app-bar'; 
    import TopAppBarTitle from '@smui/top-app-bar';
    import TopAppBarFixedAdjust  from '@smui/top-app-bar';
    import Button from '@smui/button';
  
    let title: string = 'My Svelte App';
  </script>
  
  <div class="flexy">
    <div class="top-app-bar-container flexor">
  <TopAppBar>
    <TopAppBarRow>
      <TopAppBarSection>
        <TopAppBarTitle>{title}</TopAppBarTitle>
      </TopAppBarSection>
      <TopAppBarSection>
        <Button variant="text" color="primary">Home</Button>
        <Button variant="text" color="primary">About</Button>
        <Button variant="text" color="primary">Contact</Button>
      </TopAppBarSection>
    </TopAppBarRow>
  </TopAppBar>
  </div>
  </div>
  <TopAppBarFixedAdjust />
  
  <style>
    :global(body) {
      margin: 0;
      font-family: Arial, sans-serif;
    }
    .top-app-bar-container {
    width: 100%;
    border: 1px solid
      var(--mdc-theme-text-hint-on-background, rgba(0, 0, 0, 0.1));
    margin: 0 18px 18px 0;
    background-color: var(--mdc-theme-background, #fff);
 
    overflow: auto;
    display: inline-block;
  }
  @media (max-width: 480px) {
    .top-app-bar-container {
      margin-right: 0;
    }
  }
  .flexy {
    display: flex;
    flex-wrap: wrap;
  }
  .logo {
    height: 6em;
    padding: 1.5em;
    will-change: filter;
    transition: filter 300ms;
  }
  .logo:hover {
    filter: drop-shadow(0 0 2em #646cffaa);
  }
  </style>
  