## Algorithm

- Check if the provided array of genres is empty. If it is, then select a random movie from the list and return it as an array with a single movie.
- If the provided array of genres is not empty, then create three empty arrays for movies that have all three genres, two genres, and one genre respectively.
- Loop through each movie in the list and check if it has all three genres. If it does, add it to the array for movies with all three genres.
- If a movie does not have all three genres, then check if it has two genres. If it does, add it to the array for movies with two genres.
- If a movie does not have two genres, then check if it has one genre. If it does, add it to the array for movies with one genre.
- Concatenate the three arrays in the order of movies with all three genres, two genres, and one genre.
- Return the concatenated array.

## Complexity

### Time Complexity:

O(n\*m), where n is the number of movies in the list and m is the maximum number of genres in the provided array. The loop through each movie has a time complexity of O(n), and the set operations have a time complexity of O(m). Find operations have a time complexity of O(n), but they are performed on a smaller subset of movies. Therefore, the overall time complexity is dominated by the loop through each movie.

### Space Complexity:

O(n), where n is the number of movies in the list. The space complexity is dominated by the storage of the movies array. The sets and result array have a space complexity of O(m) at most, where m is the maximum number of genres in the provided array.
