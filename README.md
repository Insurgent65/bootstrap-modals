Bootstrap 5 modal dynamic content
=================================
### Modals with dynamically loaded content an modals over modals

Highly recommended for use with: [modal close on back buttom](https://github.com/FranBar1966/bootstrap-5-modal-close-on-back)

## Installation

Add the script to your page, you can download it from [here](https://github.com/FranBar1966/bootstrap-5-modal-dynamic)

```html
<script src="modal-dynamic.min.js"></script>
```

Or from CDN:

```html
<script src="https://cdn.jsdelivr.net/gh/FranBar1966/bootstrap-5-modal-dynamic@master/src/modal-dynamic.min.js"></script>
```

### See: [DEMO](https://franbar1966.github.io/bootstrap-5-modal-dynamic/example/)


## Usage

Add the .modal-dynamic class to the link to open the button, the following link has the minimum options:

```html
    <a class="modal-dynamic" href="#modal-id" data-url="/url" data-template="#template-id">Open modal</a>

    <div id="template-id" class="modal" tabindex="-1">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title">Modal title</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <p>The content of body will be dynamically substituted by data-url.</p>
                </div>
                <div class="modal-footer">
                    <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
                </div>
            </div>
        </div>
    </div>
```

Note that you cannot mix the options with Bootstrap's native modal.

### Options

```code
 href="#modal-id"         set #modal-id to modal (REQUIRED)
 data-template="#id"      ID of the modal  (REQUIRED)
 data-url="#id"           modal content by html from #id (REQUIRED #id or /url)
 data-url="/url"          modal content by ajax /url (REQUIRED #id or /url)
 data-title="Title"       modal title
 data-header="#di"        header html content
 data-noheader="true"     remove modal header if true
 data-nofooter="true"     remove modal header if true
 data-width="100"         modal size width in px
 data-width="100px"       modal size width in px
 data-width="100%"        modal size width in %
 data-class="fade"        add class to modal
 data-keyboard="false"    default true
 data-backdrop="static"   default none
 ```
