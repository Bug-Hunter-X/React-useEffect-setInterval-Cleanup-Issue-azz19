# React useEffect setInterval Cleanup Issue

This repository demonstrates a common issue with the `useEffect` hook in React when using `setInterval`.  The initial implementation incorrectly handles the cleanup process, leading to memory leaks.  The solution shows how to properly clean up the interval to prevent these issues.

## Problem

The `bug.js` file contains a component that uses `setInterval` within `useEffect` without properly cleaning up the interval. This leads to the interval continuing to run even after the component unmounts, causing memory leaks and potentially unexpected behavior.

## Solution

The `bugSolution.js` file provides a corrected version of the component that uses `clearInterval` to ensure the interval is stopped when the component unmounts, resolving the memory leak issue.