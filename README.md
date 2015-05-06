# Pusher Gmail Zap Activity Stream

A Web Component created to display an activity stream for the Pusher integration with Zapier. This specifically creates an activity stream based on events it receives with the following characteristics:

* Events are triggered on a channel named `email`
* The events are named `new_email`
* The event data payload has` `subject` and `body` properties

You can read more about the Pusher Zapier integration here:
**TODO: update when blog post goes out**

## Usage

Include the webcomponents.js polyfill

```html
<script src="//cdnjs.cloudflare.com/ajax/libs/webcomponentsjs/0.6.1/webcomponents.min.js"></script>
```

Link in the Pusher Gmail Zap Activity Stream

```html
<link rel="import" href="//leggetter.github.io/pusher-gmail-zap-as/pusher-gmail-zap-as.html" />
```

Use the `pusher-gmail-zap-as` tag with the following attributes:

* `app-key` - the Pusher Application key to connect to and through which the events are being triggered
* `debug` - *optional* log debug information to the browser console
* `cluster` - *optional* lets you set the Pusher cluster to connect to

Example:

```html
<pusher-gmail-zap-as app-key="b9441efbc094b5934835" debug></pusher-gmail-zap-as>
```