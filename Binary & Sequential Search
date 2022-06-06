function createArray(size) {
  let brandNewArray = [];
  let i = 100;
  while (size >= 0) {
    i = i + 1;
    brandNewArray.push(i);
    size--;
  }
  return brandNewArray;
}

function sequentialSearchAlgorithm(x) {
  //sequential search is when you check each item by item
  //returns x's location in the array if x is in array and return 0 otherwise
  let array = createArray(30);
  let location = 0;
  while (location <= array.length && array[location] != x) {
    location++;
    if (location > array.length) {
      location = 0;
      return location;
    }
  }
  return 'Location of x is : ' + location;
}

function bynarySearchAlgorithm(x) {
  //determine whether x is in the nondecreasing order of n keys
  //array is indexed from 0 to n
  //output -> location of x
  //while is being used because it is not known how many times a list needs to be iterated

  //steps
  //1 - get items from the biggining and end of the array
  //2 - divide array in half (first position (0)) + last position element / 2
  //3 - select middle element to compare with target value
  //note elements can not be decimal if it is deciamal do not round it
  //4 - then if the element is lower or bigger than the target, the program will know what needs to be eliminated
  //if the element is not found it will return 0

  let array = createArray(9);
  let low = 0;
  let high = array.length - 1;
  let mid;
  let location = 0;
  console.log(array);
  //location will only change directly if the split is x
  while (low < high) {
    mid = Math.floor((low + high) / 2);
    //in an efficient assembler langugae implementation of the algorithm x would be compared with mid only once in each pass

    //is 105 at the position array[26]
    if (x == array[mid]) {
      return (location = mid);
    } else if (x < array[mid]) {
      //removes everything from the right side of the array
      high = mid - 1;
    } else {
      low = mid + 1;
    }
    return location;
  }
}

console.log(sequentialSearchAlgorithm(105));
console.log(bynarySearchAlgorithm(105));
