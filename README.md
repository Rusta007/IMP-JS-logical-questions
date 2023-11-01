# IMP-JS-logical-questions

1. You have an array of objects representing people's ages and names:
```
const people = [
  { name: 'Alice', age: 25 },
  { name: 'Bob', age: 30 },
  { name: 'Charlie', age: 20 },
  { name: 'David', age: 35 },
];
```
Your task is to write a function that ```sorts the people array by age in ascending order```. How would you solve this problem?

#### Solution:

```
const people = [
  { name: 'Alice', age: 25 },
  { name: 'Bob', age: 30 },
  { name: 'Charlie', age: 20 },
  { name: 'David', age: 35 },
];

// Sort the array by age in ascending order
people.sort((a, b) => a.age - b.age);

console.log(people);

Output:
[
  { name: 'Charlie', age: 20 },
  { name: 'Alice', age: 25 },
  { name: 'Bob', age: 30 },
  { name: 'David', age: 35 }
]

```

2. You are given an array of objects representing books with title, author, and publication year:
```
const books = [
  { title: 'Book A', author: 'Author X', year: 2020 },
  { title: 'Book B', author: 'Author Y', year: 2015 },
  { title: 'Book C', author: 'Author Z', year: 2012 },
  // ... more books
];
```
Your task is to write a function that ```filters this array to find books published between the years 2010 and 2020```, and then ```sort them in alphabetical order by the book title```. How would you solve this problem?

#### Solution:
```
const books = [
  { title: 'Book A', author: 'Author X', year: 2020 },
  { title: 'Book B', author: 'Author Y', year: 2015 },
  { title: 'Book C', author: 'Author Z', year: 2012 },
  // ... more books
];

// Filter books published between 2010 and 2020
const filteredBooks = books.filter(book => book.year >= 2010 && book.year <= 2020);

// Sort the filtered array by title in alphabetical order
filteredBooks.sort((a, b) => a.title.localeCompare(b.title));

console.log(filteredBooks);

Output:
[
  { title: 'Book A', author: 'Author X', year: 2020 },
  { title: 'Book B', author: 'Author Y', year: 2015 },
  // ... other books meeting the criteria, sorted by title
]

```

















