<script>
  import { Router, Route } from "svelte-routing";
  import Home from "./routes/Home.svelte";
  import CourseLibrary from "./routes/CourseLibrary.svelte";

  export let url = ""; // This is fine to export
</script>

<Router {url}>
  <div class="navbar">
      <Route path="/" component={Home} />
      <Route path="/library" component={CourseLibrary} />
  </div>
</Router>