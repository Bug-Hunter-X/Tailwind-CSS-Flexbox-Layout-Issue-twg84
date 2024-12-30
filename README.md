# Tailwind CSS Flexbox Layout Bug

This repository demonstrates a bug where Tailwind CSS classes are not applied correctly within a flexbox layout.  The expected behavior is for two divs to occupy equal width within their parent container. However, one div expands to take the full width, ignoring the `w-1/2` class.

## Steps to Reproduce

1. Clone this repository.
2. Open `bug.html` in a web browser.
3. Observe that the red div occupies the entire width, while the blue div is not displayed as expected.

## Solution

The solution involves adding the `flex-shrink-0` class to the child divs. This prevents them from shrinking below their minimum size, ensuring that they each occupy their allocated space within the flex container.

See `bugSolution.html` for the corrected code.