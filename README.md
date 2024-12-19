# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug involving the `useEffect` hook.  The bug causes an infinite loop due to a missing dependency in the `useEffect` hook's dependency array.  The solution shows how to correctly add the dependency to fix the problem.

## Bug Description

The `useEffect` hook is used to perform side effects in functional components. However, if a dependency is omitted from the dependency array, the effect will run on every render, potentially leading to an infinite loop or unexpected behavior.

## Solution

The solution involves adding the `count` state variable to the `useEffect` hook's dependency array.  This ensures that the effect only runs when the `count` variable changes.