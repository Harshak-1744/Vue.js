## Using CDN file 

### Steps to Create a Basic Vue 3 App:

#### Step 1: **Setup Your HTML File**:
- Create a new file on your computer and name it `index.html`.

#### Step 2: **Structure Your HTML**:
- Inside your `index.html`, add the standard HTML structure, which includes `DOCTYPE`, `html`, `head`, and `body` tags.

#### Step 3: **Design Your App's Layout**:
- Inside the `body` tag, create a `div` where Vue will attach the application. Give it an `id` of "content". 

  ```html
  <div id="content">
      <h1>{{ pageTitle }}</h1>
      <p>{{ content }}</p>
  </div>
  ```

  This is where the Vue app will display the title and content you defined in your Vue code.

#### Step 4: **Include Vue.js CDN for Vue 3**:
- Before the closing `body` tag, include Vue 3 using a CDN link., you'd get the CDN link from Vue's official documentation or a trusted CDN provider.

#### Step 5: **Add Your Vue Script**:
- After the CDN link, insert a `script` tag for your Vue.js code. Paste the code you provided:

  ```javascript
  Vue.createApp({
      data() {
          return {
              pageTitle: 'Hello, Kiddo',
              content: 'Welcome to Vue Framework'
          }
      }
  }).mount("#content");
  ```

  This code creates a new Vue 3 application, sets up some reactive data (pageTitle and content), and then mounts the application to the `div` with `id="content"`.

#### Step 6: **Test Your App**:
- Save the `index.html` file.
- Open it with a web browser. You should see the title "Hello, Kiddo" and the content "Welcome to Vue Framework" displayed on the page.


## Example:-
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Basic Vue 3 App</title>
</head>
<body>

<div id="content">
    <h1>{{ pageTitle }}</h1>
    <p>{{ content }}</p>
</div>

<!-- Including Vue 3 from CDN -->
<script src="https://unpkg.com/vue@next"></script>

<script>
    Vue.createApp({
        data() {
            return {
                pageTitle: 'Hello, Kiddo',
                content: 'Welcome to Vue Framework'
            }
        }
    }).mount("#content");
</script>

</body>
</html>
```
