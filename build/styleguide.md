<style>
body {
    overflow-x: hidden;
}
</style>

## **Last Set**: Airbnb special components <a id="last-set" class='ma-btn ma-btn--small ma-btn--minimal' style='float: right;top: 16px;' href='http://bit.ly/2w3Z976'>Download set</a> <div style="font-size:20px;color:#FF5A5F;">Wednesday, 23 Aug 2017</div>

### Main Header

This component represents the main header of Airbnb, which contains a search bar, nav options list, and user avatar logged. Use it adding the class: `.ma-header` to the header html tag

    @example
    <!-- HEADER -->
    <header class="ma-header ma-header--large">

        <!-- Logo -->
        <div class="ma-header__logo-container">
            <a class="link-reset">
                <div class="content">
                    <div class="ma-logo"></div>
                </div>
            </a>
        </div>

        <!-- Search box -->
        <div class="ma-header__search-container">
            <form class="form-content hidden-xs">
                <div class="ma-search-bar">
                    <i class="ma-search-bar__icon" data-feather="search"></i>
                    <label class="screen-reader-only" aria-hidden="true">Search</label>
                    <input class="ma-search-bar__input" placeholder="Search" type="text">
                </div>
            </form>
        </div>

        <!-- Navigation Container -->
        <div class="ma-header__nav-container">
            <nav>
                <ul class="ma-nav-list">
                    <!-- Log in button -->
                    <li class="ma-nav-list__item">
                        <button class="ma-nav-list__item__btn">Log in</button>
                    </li>
                    <!-- Sign up button -->
                    <li class="ma-nav-list__item">
                        <button class="ma-nav-list__item__btn">Sign up</button>
                    </li>
                    <!-- Avatar button -->
                    <li>
                        <a class="ma-nav-list__item__btn link-reset" href>
                            <div class="content">
                                <div class="ma-avatar ma-avatar--tiny ma-avatar--border-minimal round">
                                    <img width="32" height="32" src="{user_avatar_path}" alt="{username}">
                                </div>
                            </div>
                        </a>
                    </li>
                </ul>
            </nav>
        </div>

    </header>


    <!-- DARK SUBNAV -->
    <div class="ma-subnav ma-subnav--dark">
      <nav class="container">
        <div class="ma-subnav__item">
            <a href>Overview</a>
        </div>

        <div class="ma-subnav__item">
            <a href>Review</a>
        </div>

        <div class="ma-subnav__item active">
            <a href>The Host</a>
        </div>

        <div class="ma-subnav__item">
            <a href>Location</a>          
        </div>
      </nav>
    </div>


    <!-- To use feathericons -->
    <!-- reference: https://feathericons.com/ -->
    <script>
      feather.replace()
    </script>


### User profile avatar

Every avatar image based on Airbnb avatar. This component includes: round and square, primary, secondary and minimal border, tiny, small, default and large size. Use it adding the class: `.ma-avatar`, and its respective type and size modifier (e.g. `.ma-avatar--tiny`, `.ma-avatar--large`, `.ma-avatar--border-primary`, `.ma-avatar--border-secondary`).

    @example
    <!-- tiny round avatar without border -->
    <div class="ma-avatar ma-avatar--tiny round">
        <img width="32" height="32" src="{avatar_default_path}" alt="{username}">
    </div>

    <!-- tiny round avatar with primary border -->
    <div class="ma-avatar ma-avatar--tiny ma-avatar--border-primary round">
        <img width="32" height="32" src="{avatar_default_path}" alt="{username}">
    </div>

    <!-- small round avatar without border -->
    <div class="ma-avatar ma-avatar--small round">
        <img width="70" height="70" src="{avatar_default_path}" alt="{username}">
    </div>

    <!-- small round avatar with secondary border -->
    <div class="ma-avatar ma-avatar--small ma-avatar--border-secondary round">
        <img width="70" height="70" src="{avatar_default_path}" alt="{username}">
    </div>

    <!-- default round avatar without border -->
    <div class="ma-avatar ma-avatar--default round">
        <img width="120" height="120" src="{avatar_default_path}" alt="{username}">
    </div>

    <!-- default round avatar with minimal border -->
    <div class="ma-avatar ma-avatar--default ma-avatar--border-minimal round">
        <img width="120" height="120" src="{avatar_default_path}" alt="{username}">
    </div>

    <!-- default square avatar without border -->
    <div class="ma-avatar ma-avatar--default">
        <img width="120" height="120" src="https://s3.amazonaws.com/waysily-img/stylepill/rands-avatar.jpg" alt="Rosita & Sergio">
    </div>

    <!-- default square avatar with minimal border -->
    <div class="ma-avatar ma-avatar--default ma-avatar--border-minimal">
        <img width="120" height="120" src="{avatar_default_path}" alt="{username}">
    </div>


### Special Search box

Special Search Box used by Airbnb on its home page header. It has a beautiful effect on **input focus**. Use it adding the class: `ma-searchbox`

    @example
    <div class="ma-searchbox">
        <div class="ma-searchbox__icon-container">
            <i data-feather="search"></i>
        </div>
        <div class="ma-searchbox__input-container">
            <input class="ma-searchbox__input-container__input" placeholder="Anywhere" type="text">
        </div>
    </div>

    <!-- To use feathericons reference: https://feathericons.com/ -->
    <script>
      feather.replace()
    </script>


## **Set #4**: Airbnb social buttons & helpful buttons<a class='ma-btn ma-btn--small ma-btn--minimal' style='float: right;top: 16px;' href='http://bit.ly/2uQ44ab'>Download set</a> <div style="font-size:20px;color:#FF5A5F;">Wednesday, 16 Aug 2017</div>

### Facebook button

A simple and minimalist Facebook button based on Airbnb theme. Use it adding the modifier: `.ma-btn--facebook`

    @example
    <button class="ma-btn ma-btn--default ma-btn--facebook">
        <div class="ma-btn__content">
            <div class="ma-btn__content__icon-container">
                <i class="fa fa-facebook" aria-hidden="true"></i>
            </div>
            <div class="space-left-2">
                <span>Log in with Facebook</span>
            </div>
        </div>
    </button>


### Google button

A simple and minimalist Google button based on Airbnb theme. Use it adding the modifier: `.ma-btn--google`

    @example
    <button class="ma-btn ma-btn--default ma-btn--google">
        <div class="ma-btn__content">
            <div class="ma-btn__content__icon-container">
                <!-- Google icon SVG -->
                <i class="google-icon"></i>
            </div>
            <div class="space-left-2">
                <span>Log in with Google</span>
            </div>
        </div>
    </button>


### Helpful button

A button used by Airbnb on Reviews and recommendations section. Use it adding the modifier: `.ma-btn--helpful` adding size and type modifiers (e.g. `.ma-btn--small`, `.ma-btn--primary`)

    @example
    <!-- Helpful Primary Button -->
    <button class="ma-btn ma-btn--helpful ma-btn--helpful--small ma-btn--helpful--primary">
        <span>
            <i class="fa fa-thumbs-o-up" aria-hidden="true"></i>
            <div class="ma-btn--helpful__text">Helpful</div>
            <div class="ma-btn--helpful__count">3</div>
        </span>
    </button>


    <!-- Helpful Secondary Button -->
    <button class="ma-btn ma-btn--helpful ma-btn--helpful--small ma-btn--helpful--secondary">
        <span>
            <i class="fa fa-thumbs-o-up" aria-hidden="true"></i>
            <div class="ma-btn--helpful__text">Helpful</div>
            <div class="ma-btn--helpful__count">3</div>
        </span>
    </button>


    <!-- Helpful Minimal Button -->
    <button class="ma-btn ma-btn--helpful ma-btn--helpful--small ma-btn--helpful--minimal">
        <span>
            <i class="fa fa-thumbs-o-up" aria-hidden="true"></i>
            <div class="ma-btn--helpful__text">Helpful</div>
            <div class="ma-btn--helpful__count">3</div>
        </span>
    </button>


## **Set #3**: Airbnb main subnavs <a class='ma-btn ma-btn--small ma-btn--minimal' style='float: right;top: 16px;' href='http://bit.ly/2wpxCzp'>Download set</a> <div style="font-size:20px;color:#FF5A5F;">Wednesday, 9 Aug 2017</div>

### Simple navbar

A simple and beautiful navbar used by Airbnb commonly in 'room profile'. Use it adding the modifier: `.ma-subnav--simple`

    @example
    <div class="ma-subnav ma-subnav--simple">
        <nav class="container">
            <div class="ma-subnav__item">
                <div class="content">
                    <a href>Overview</a>
                </div>
            </div>

            <span class="space-right-1 space-left-1"> · </span>

            <div class="ma-subnav__item">
                <div class="content">
                    <a href>Review</a>
                </div>
            </div>

            <span class="space-right-1 space-left-1"> · </span>

            <div class="ma-subnav__item">
                <div class="content">
                    <a class="active" href>The Host</a>
                </div>
            </div>

            <span class="space-right-1 space-left-1"> · </span>

            <div class="ma-subnav__item">
                <div class="content">
                    <a href>Location</a>
                </div>
            </div>

        </nav>
    </div>


### Tabs navbar

This navbar is used by Airbnb commonly in front page to navigate each relevant section. Use it adding the modifier: `.ma-subnav--tabs`

    @example
    <div class="ma-subnav ma-subnav--tabs">
        <nav class="container">
            <div class="ma-subnav__item space-right-4">
                <div class="content">
                    <a class="link-reset" href>FOR YOU</a>
                </div>
            </div>

            <div class="ma-subnav__item space-right-4">
                <div class="content active">
                    <a class="link-reset" href>HOMES</a>
                </div>
            </div>

            <div class="ma-subnav__item space-right-4">
                <div class="content">
                    <a class="link-reset" href>EXPERIENCES</a>
                </div>
            </div>

            <div class="ma-subnav__item">
                <div class="content">
                    <a class="link-reset" href>PLACES</a>
                </div>
            </div>

        </nav>
    </div>



## **Set #2**: Airbnb main inputs  <a class='ma-btn ma-btn--small ma-btn--minimal' style='float: right;top: 16px;' href='http://bit.ly/2v9aOj5'>Download set</a> <div style="font-size:20px;color:#FF5A5F;">Wednesday, 2 Aug 2017</div>

### Small input

Small input commonly used by Airbnb on its forms such as edit profile, account, or setting. Use it adding the modifier: `.ma-input--small`

    @example.slim
    <div class="form-group">
        <label for="input1">Small Input Text</label>
        <input id="input1" type="text" class="ma-input ma-input--small" placeholder="Name">
    </div>


### Default input

Default input commonly used by Airbnb on its forms such as edit profile, account, or setting. Use it adding the modifier: `.ma-input--default`

    @example.slim
    <div class="form-group">
        <label for="input1">Default Input Text</label>
        <input id="input1" type="text" class="ma-input ma-input--default" placeholder="Email Address">
    </div>

### Large input

Large input commonly used by Airbnb on its forms such as edit profile, account, or setting. Use it adding the modifier: `.ma-input--large`

    @example.slim
    <div class="form-group">
        <label for="input1">Large Input Text</label>
        <input id="input1" type="text" class="ma-input ma-input--large" placeholder="First Name">
    </div>

### Default Invalid input

Default invalid input styles. Use it adding the modifier: `.ma-input--invalid`

    @example.slim
    <div class="form-group">
        <label for="input5">Invalid Input Text</label>
        <input id="input5" type="text" class="ma-input ma-input--default ma-input--invalid" placeholder="Invalid Input Text">
        <p class="ma-msg ma-msg--small ma-msg--alert space-top-1">
            Name required.
        </p>
    </div>


## **Set #1**: Airbnb main buttons <a class='ma-btn ma-btn--small ma-btn--minimal' style='float: right;top: 16px;' href='http://bit.ly/2vQJzLV'>Download set</a> <div style="font-size:20px;color:#FF5A5F;">Wednesday, 26 Jul 2017</div>


### Primary button

A simple and minimalist button based on Airbnb primary color. Use it adding the modifier: `.ma-btn--primary`

    @example
    <button class="ma-btn ma-btn--small ma-btn--primary">
        Log in
    </button>


### Secondary button

A simple and minimalist button based on Airbnb secondary color. Use it adding the modifier: `.ma-btn--secondary`

    @example
    <button class="ma-btn ma-btn--small ma-btn--secondary">
        Log in
    </button>


### Primary Outline button

A simple and minimalist outline button based on Airbnb primary color. Use it adding the modifier: `.ma-btn--primary-without-bg`

    @example
    <button class="ma-btn ma-btn--small ma-btn--primary-without-bg">
        Log in
    </button>

<br>

# Styleguide options

### Head
    meta(name="viewport" content="width=device-width, initial-scale=1")
    link(rel='stylesheet' href='https://maxcdn.bootstrapcdn.com/bootstrap/3.2.0/css/bootstrap.min.css')
    link(rel='stylesheet' href='build/styles/styleguide.css')
    link(rel='stylesheet' href='build/styles/styleguide-reset.css')
    link(rel='stylesheet' href='build/styles/app.min.css')
    link(rel='stylesheet' href='https://cdn.rawgit.com/styledown/styledown/v1.0.2/data/styledown.css')
    link(rel='stylesheet' href='https://fonts.googleapis.com/css?family=Source+Sans+Pro')
    link(rel='stylesheet' href='https://fonts.googleapis.com/css?family=Lato')
    script(src='https://cdn.rawgit.com/styledown/styledown/v1.0.2/data/styledown.js')
    script(src='https://use.fontawesome.com/99e7a6e2c6.js')
    script(src='https://unpkg.com/feather-icons/dist/feather.min.js')

### Body

    .jumbotron.jumbotron-styleguide
        .container
            h1(style="font-weight:400")
                | Stylepill
            p.ma-p.ma-p--default
                | Theme of the month:
                strong(style="color: #FF5A5F")
                    | Airbnb

            hr

            p.ma-p(style="font-size:15px;font-weight:600")
                | Follow us on Twitter, we'll show you our works, triumphs, failures, 100% transparent.
            p
                a.btn.btn-default(href="https://www.twitter.com/seruda") @seruda
                a.btn.btn-default(href="https://www.twitter.com/rosa7082") @rosa7082
            p   
                a.btn.btn-default(href="http://eepurl.com/cYzCeX") Join list
    .container
        div(sg-content)
