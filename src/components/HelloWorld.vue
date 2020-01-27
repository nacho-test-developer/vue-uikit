<template>
  <div>
    <nav class="uk-navbar-container" uk-navbar>
      <div class="uk-navbar-left">

          <div class="uk-navbar-item">
              <form class="uk-search uk-search-navbar">
                  <span uk-search-icon></span>
                  <input class="uk-search-input" type="search" placeholder="Search...">
              </form>
          </div>

      </div>
    </nav>
    <div class="uk-height-large uk-background-cover uk-light uk-flex" uk-parallax="bgy: -200" style="background-image: url('https://getuikit.com/docs/images/dark.jpg');">

        <h1 class="uk-width-1-2@m uk-text-center uk-margin-auto uk-margin-auto-vertical">Headline</h1>

    </div>

    <div class="uk-container uk-margin">
      <article class="uk-comment uk-comment-primary">
        <header class="uk-comment-header uk-grid-medium uk-flex-middle" uk-grid>
          <div class="uk-width-auto">
            <img class="uk-comment-avatar" src="https://getuikit.com/docs/images/avatar.jpg" width="80" height="80" alt="">
          </div>
          <div class="uk-width-expand">
            <h4 class="uk-comment-title uk-margin-remove"><a class="uk-link-reset" href="#">Author</a></h4>
            <ul class="uk-comment-meta uk-subnav uk-subnav-divider uk-margin-remove-top">
              <li><a href="#">12 days ago</a></li>
              <li><a href="#">Reply</a></li>
            </ul>
          </div>
        </header>
        <div class="uk-comment-body">
          <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.</p>
        </div>
      </article>
    </div>
    <div class="uk-container uk-container-small uk-margin">
      <div class="uk-flex uk-flex-center uk-margin">
        <div class="uk-card uk-card-default uk-card-body">Item 1</div>
        <div class="uk-card uk-card-default uk-card-body uk-margin-left">Item 2</div>
        <div class="uk-card uk-card-default uk-card-body uk-margin-left">Item 3</div>
      </div>
        <div class="uk-child-width-1-3@m uk-grid-small uk-grid-match" uk-grid>
          <div>
              <div class="uk-card uk-card-default uk-card-body">
                  <h3 class="uk-card-title">Default</h3>
                  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
              </div>
          </div>
          <div>
              <div class="uk-card uk-card-primary uk-card-body">
                  <h3 class="uk-card-title">Primary</h3>
                  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
              </div>
          </div>
          <div>
              <div class="uk-card uk-card-secondary uk-card-body">
                  <h3 class="uk-card-title">Secondary</h3>
                  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
              </div>
          </div>
      </div>
    </div>

    <div class="uk-container">
      <article class="uk-article">
        <progress class="uk-progress" :value="ok" max="100"></progress>
        <!-- This is a button toggling the modal -->
        <button class="uk-button uk-button-default uk-margin-small-right" type="button" uk-toggle="target: #modal-example">Open</button>

        <!-- This is an anchor toggling the modal -->
        <a href="#modal-example" uk-toggle>Open</a>
      </article>
    </div>

    <!-- This is the modal -->
    <div id="modal-example" uk-modal>
      <div class="uk-modal-dialog uk-modal-body">
          <h2 class="uk-modal-title">Headline</h2>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
          <p class="uk-text-right">
              <button class="uk-button uk-button-default uk-modal-close" type="button">Cancel</button>
              <button class="uk-button uk-button-primary" type="button">Save</button>
          </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data () {
    return {
      ok: '30'
    }
  }
}
</script>
