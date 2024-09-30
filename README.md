const array1 = [1,"2", 3, '$', '%', 3, 4, 7,"baasa", 1, '#'];

const array2 = array1
  .filter(item => typeof item === 'number') // Remove strings and special characters
  .filter((item, index, arr) => arr.indexOf(item) === index); // Remove repeated values

console.log(array2); // Output: [1, 2, 3, 4, 7]
