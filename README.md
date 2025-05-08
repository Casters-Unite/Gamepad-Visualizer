# use

This is set up to be a visualizer that you overlay over another page with an Iframe or something.

You can achive this by 
1. including ```<script src="https://cdn.tailwindcss.com"></script>``` in the head, and ```<script src="Embed.js"></script>``` in the body.
2. Loading ```https://casters-unite.github.io/Gamepad-Visualizer``` into an Iframe.

There is a browser extension planned that'll Overlay this over any site you want.

## URL Paramaters

*   **`scale=%`**:
    *   Scales the `.controller-container` to the specified percentage.
    *   Example: `?scale=75` (scales to 75%)
    *   Example: `?scale=150` (scales to 150%)
    *   Default: 100% if omitted AND `overlay=true` is not used (otherwise overlay scale takes precedence)
    *   Ignored when `overlay=true` is used.

*   **`selection=hidden`**:
    *   Hides the gamepad selection dropdown.
    *   Example: `?selection=hidden`
    *   Default: Hidden if omitted *and* `overlay=true` is used (otherwise it's visible unless you specify). Visible if `overlay=false`.

*   **`selection=visible`**:
    *   Forces the gamepad selection dropdown to be visible, even in overlay mode.
    *   Example: `?overlay=true&selection=visible`

*   **`overlay=false`**:
     *  Disables overlay mode.  Forces standard centering and 100% scale unless overridden with `scale=`.
