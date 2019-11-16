# Simple material design

> This repository focuses only on basic components made for high performance.

## Components (TODO)
- [ ] Alerts
- [ ] Badge
- [x] Buttons
- [ ] Card
- [ ] Forms
- [x] Grids
- [ ] Inputs
- [ ] Modals
- [x] Navbar
- [ ] Typography

## Grids 

> This is the simplest component, it divides the layout into 12 columns.

- **container**: all other tags must be inside it
- **row**: create a row, columns settings must be inside a row
- **col**: create a column, to defines column sizes want use **md**, **sm** or **xs** tag in same item
   - **md-**: md is for devices with width greater than 768px, **usage:** *md-{number of columns}*
   - **sm-**: sm is for devices with width greater than 576px and less than 768px, **usage:** *sm-{number of columns}
   - **xs-**: xs is for devices with width less than 576px, **usage:** *xs-{number of columns}*

### Usage: 
``` html
<div class="container">
    <div class="row">
        <div class="col md-6 sm-12 xs-12">
            Side I
        </div>
        <div class="col md-6 sm-12 xs-12">
            Side II
        </div>
    </div>
</div>
``` 
## Buttons

It's just beautiful buttons
> **important:** all buttons are colorless, you'll want define a new class and customize yourself, like this: 
``` css
/* for example you put *black* class in the button */
.black {
    color: #FFFFFF; /* font color */
    background: #000000; /* background color */
}
```

### Usage:
``` html
    <button class="btn black">Click here</button>
```

## Navbar

Navbar by default is fixed on top and has a height of 60px

### Usage: 
``` html
 <header class="header black">
    <input type="checkbox" id="btn-menu">
    <label for="btn-menu" class="hamburger-menu"></label>
    <div class="overlay" id="overlay"></div>
    <div class="menu">
        <ul class="nav-list">
            <li class="nav-link">Link 1</li>
            <li class="nav-link">Link 2</li>
            <li class="nav-link">Link 3</li>
        </ul>
    </div>
    <h1 class="nav-title">Logo</h1>
</header>
```