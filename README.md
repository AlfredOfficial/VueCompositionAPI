# CompositionAPI Blog Demo

A simple Vue 3 project demonstrating the use of the Composition API to display a list of blog posts with basic styling.

## Features

- Vue 3 with `<script setup>` and Composition API
- Static list of posts with author, date, title, and body
- Styled with SCSS (Sass) and Google Fonts
- Material Icons for action buttons

## Project Structure

```
src/
  assets/
    main.css         # Global styles and font import
  views/
    HomeView.vue     # Main blog post view with SCSS styling
```

## Setup

1. **Install dependencies**

   ```
   npm install
   ```

2. **Install Sass (if not already installed)**

   ```
   npm install -D sass
   ```

3. **Run the development server**

   ```
   npm run dev
   ```

4. **Open your browser**

   Visit [http://localhost:5173](http://localhost:5173) (or the port shown in your terminal).

## Styling

- Uses the [Kanit](https://fonts.google.com/specimen/Kanit) font from Google Fonts.
- Custom SCSS for the blog post cards and layout.
- Material Icons for delete and bookmark buttons.

## Customization

- To add or edit posts, modify the `posts` array in `src/views/HomeView.vue`.
- To change global styles, edit `src/assets/main.css`.
- To update component styles, edit the `<style lang="scss" scoped>` block in `HomeView.vue`.

## License

This project is for educational/demo
