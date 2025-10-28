# Tower-of-hanoi
The Tower of Hanoi is a classic mathematical puzzle that demonstrates the concept of recursion in computer programming. This project provides a C program (or any other language you choose) to solve the Tower of Hanoi problem by moving a set of disks from one rod to another following specific rules.
# 🏗️ Tower of Hanoi Project

## 📘 Project Overview
The **Tower of Hanoi** is a classic mathematical puzzle that demonstrates the concept of **recursion** in programming.  
This project provides a program to solve the Tower of Hanoi problem by moving a set of disks between three rods according to specific rules.

---

## 🎯 Objective
To implement the Tower of Hanoi algorithm using **recursion** and display each step involved in transferring disks from the source rod to the destination rod.

---

## 🧩 Problem Statement
You are given three rods — **A (Source)**, **B (Auxiliary)**, and **C (Destination)** — and **n disks** of different sizes stacked in ascending order on rod A (smallest on top).  
The task is to move all disks from **A** to **C** following these rules:

1. Only one disk can be moved at a time.  
2. A disk can only be placed on top of a larger disk or an empty rod.  
3. All disks must end up on the destination rod in the same order.

---

## 💡 Algorithm
1. Move (n-1) disks from Source to Auxiliary.  
2. Move the nth (largest) disk from Source to Destination.  
3. Move (n-1) disks from Auxiliary to Destination.  

This recursive pattern continues until only one disk remains to move.

---

## 🧠 Example Output

