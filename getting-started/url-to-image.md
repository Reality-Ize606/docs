---
description: >-
  Take a screenshot of any URL using the API. Screenshot generated in a real
  instance of Google Chrome.
---

# URL to image

With the API, you can automate taking a screenshot of any website. It's incredibly simple.

Pass the `url` param to the `hcti.io/v1/image` endpoint, and we'll generate a screenshot for you. Here's an example using cURL.

```text
curl -X POST https://hcti.io/v1/image -u 'UserID:APIKey' 
             -d url="https://google.com"
```

{% hint style="info" %}
Don't write code? Don't worry, you can also do this with our [Zapier integration](zapier-integration.md).
{% endhint %}

![Screenshot generated by the API](../.gitbook/assets/image%20%2817%29.png)

### Additional parameters

To customize your image further, you can take advantage of the following optional parameters.

| Parameter |  |
| :--- | :--- |
| viewport\_width | Set the width of Chrome's viewport. Defaults to 1366. |
| viewport\_height | Set the height of Chrome's viewport. Defaults to 768. |
| device\_scale | This adjusts the pixel ratio for the device. Default: 1. Maximum 3. |
| ms\_delay | The number of milliseconds the API should delay before taking the screenshot. This is useful when waiting for JavaScript. If you need to use this, we recommend starting with a low number, such as `500`. Increasing this value slows down the speed of your initial render. |

### Screenshot examples

A full screenshot of `stripe.com`. With device scale set to 2, for a super high resolution image.

![High resolution screenshot generated by the API](../.gitbook/assets/image%20%286%29.png)

Here's a screenshot of `apple.com`.

![Screenshot generated of Apple](../.gitbook/assets/image%20%283%29.png)

### Need help getting started?

We'd be happy to walk you through getting started. Send us an email: **support@htmlcsstoimage.com**. We're experts at generating images and will help you get going using the API.

