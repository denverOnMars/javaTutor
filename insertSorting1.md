Slide 1: Title Slide

- “Sorting Sports Scores with Insertion Sort in Java: Fun and Easy!”

Slide 2: The Scenario

- Imagine you’re a sports fan keeping track of your favorite teams’ scores
- Your job: Organize the scores from smallest to largest to quickly find the highest scoring games
- We’re going to learn Insertion Sort to help you with this task!

Slide 3: Insertion Sort Explained with an Analogy

- You’ve got a handful of sports scores, written on cards
- You’re arranging them on the table in order, from left (smallest) to right (largest)
- When adding a new card, you slide it into the correct position among the already sorted cards

Slide 4: Insertion Sort Algorithm Breakdown

1. Start with the second score (consider the first one already sorted)
2. Compare it to the one before it
3. If it’s smaller, keep comparing it to previous scores
4. Move scores larger than the current one ahead to create a space
5. Insert the current score in the correct position

Slide 5: Java Code - Signature and First Loop (Visual)

java public static void insertionSort(int[] arr) { int n = arr.length; for (int i = 1; i < n; i++) { // "i" represents the score card we're trying to insert into the sorted part } }

Slide 6: Java Code - Second Loop (Visual)

java for (int j = i; j > 0; j--) { // "j" helps us compare the current score card to the already sorted ones }

Slide 7: Java Code - Complete Insertion Sort Function with Comments

java public static void insertionSort(int[] arr) { int n = arr.length; for (int i = 1; i < n; i++) { for (int j = i; j > 0; j--) { if (arr[j] < arr[j-1]) { int temp = arr[j]; arr[j] = arr[j-1]; arr[j-1] = temp; } else { break; } } } }

Slide 8: Java Code - Organizing Scores

java public static void main(String[] args) { int[] scores = {13, 23, 9, 27, 16}; System.out.println("Unsorted scores: " + Arrays.toString(scores)); insertionSort(scores); System.out.println("Sorted scores: " + Arrays.toString(scores)); }

Slide 9: Output Example

- Unsorted scores: [13, 23, 9, 27, 16]
- Sorted scores: [9, 13, 16, 23, 27]

Slide 10: Wrap-up

- You learned how to use Insertion Sort to sort sports scores
- Easy-to-understand algorithm with decent performance for small data sets
- Impress your friends & family by quickly finding the highest scoring games!

Slide 11: Time Complexity - Analogy


- Imagine organizing 10 basketball cards

- In the best-case scenario: cards are already sorted, and you only need to check each card once

- In the worst-case scenario: cards are sorted in reverse, and you need to check each card multiple times

- As the number of cards increases, the time it takes to add new cards grows exponentially



Slide 12: Time Complexity - Explanation


- The time complexity refers to how the time taken by the algorithm grows based on the input size

- O(n) in the best-case (already sorted)

- O(n^2) in the worst-case and average (random or reversed order)

- Suits smaller data sets better; not ideal for very large sets



Slide 13: Space Complexity - Analogy


- In our basketball card scenario, we didn’t need additional cards or placeholders

- We simply moved the cards around on the table - that’s the only space we needed



Slide 14: Space Complexity - Explanation


- The space complexity refers to the additional memory used by the algorithm

- Insertion Sort is an “in-place” sorting algorithm, meaning it requires no extra memory

- Its space complexity is O(1), meaning it has minimal memory overhead

- Good for sorting tasks where space is limited



Slide 15: Comparing Insertion Sort to Other Algorithms


- Insertion Sort isn’t the only way to sort data

- Other popular sorting algorithms: Bubble Sort, Selection Sort, Merge Sort, Quick Sort

- Each algorithm has its own time and space complexities, and is suited for specific scenarios

- Learning multiple sorting algorithms helps you choose the best one for a particular task
