# Uncommon HTML Error: Incorrect Text Content Access

This repository demonstrates a subtle error in accessing the text content of an HTML div element.  Many developers are familiar with `innerHTML`, but the nuanced differences between `innerText` and `textContent` can be easily overlooked.

The `bug.html` file showcases the incorrect approach, while `bugSolution.html` provides the correct implementation.

## The Problem

The primary issue is the misuse of `innerText`. While `innerText` works in many cases, it can produce unexpected results when dealing with complex HTML structures or hidden elements.  `textContent` provides a more consistent and reliable way to retrieve the text content of an element, regardless of the element's structure.

## The Solution

Using `textContent` ensures that all the text content of the element is retrieved, regardless of its formatting and visibility.

If you need the HTML structure along with the text, then you should use `innerHTML`.