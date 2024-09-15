Here's a `README.md` file you can use for your project repository:

---

# Color Blind Test with Animated Image Transitions

This project is a web-based color blind test application that presents users with a series of images and interactive answer buttons. The test includes animated image transitions, a responsive progress bar to track user progress, and a results summary at the end.

## Features

- **Animated Image Transitions**: Smooth diagonal reveal animation for each image using CSS keyframes.
- **Responsive Design**: Works across different screen sizes, ensuring a consistent experience on desktop and mobile.
- **Progress Tracking**: A dynamic progress bar to track user progression through the test.
- **Results Summary**: Displays correct and user-selected answers at the end of the test.
- **Restart Option**: Allows users to restart the test from either the game or result view.
- **Preloaded Images**: Images are preloaded to ensure smooth transitions without delay.

## Demo

You can see the project in action by visiting [Demo URL] (replace with the demo link if available).

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/color-blind-test.git
   ```

2. Navigate to the project directory:
   ```bash
   cd color-blind-test
   ```

3. Open the `index.html` file in your browser to run the application.

## Usage

1. Users are presented with an image and multiple answer buttons.
2. Click the appropriate button to select the answer based on the displayed image.
3. A progress bar at the top shows your progress through the test.
4. Once all questions are answered, a results summary is displayed.
5. Users can restart the test at any time using the restart button.

## Technologies Used

- **HTML5**
- **CSS3** (including keyframe animations)
- **JavaScript**
- **Bootstrap 5**

## CSS Animations

The image transitions use a diagonal reveal animation. If the animation slows down image loading, preloading is used to ensure smooth transitions.

```css
.image {
  width: 300px;
  height: 300px;
  opacity: 1;
  -webkit-mask-image: linear-gradient(135deg, black 0%, black 50%, transparent 50%, transparent 100%);
  mask-image: linear-gradient(135deg, black 0%, black 50%, transparent 50%, transparent 100%);
  mask-size: 300% 300%;
  -webkit-mask-size: 300% 300%;
  animation: revealDiagonal 3s forwards ease-in-out;
}

@keyframes revealDiagonal {
  0% {
    -webkit-mask-position: 100% 100%;
    mask-position: 100% 100%;
  }
  100% {
    -webkit-mask-position: 0% 0%;
    mask-position: 0% 0%;
  }
}
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to modify it to suit your specific project needs!
