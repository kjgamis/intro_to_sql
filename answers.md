## Questions

1. Find all the robots from Star Wars.

  ```
  SELECT * FROM robots WHERE source = 'Star Wars';
  ```

2. Find the robot with an "anxious" personality.

  ```
  SELECT * FROM robots WHERE personality = 'anxious';
  ```

3. Find all recipes that are nut free.

  ```
  SELECT * FROM recipes WHERE nut_free = true;
  ```

4. Count the number of recipes that are gluten free but not vegetarian.

  ```
  SELECT COUNT (id) FROM recipes WHERE gluten_free = true AND vegetarian = false;
  ```

5. Find the animal with the most legs.

  ```
  SELECT MAX(number_of_legs) FROM animals;
  SELECT name FROM animals WHERE number_of_legs = 8;
  ```

6. Find the board game that takes the least amount of time to play.

  ```
  SELECT MIN(mins_to_play) FROM board_games
  SELECT MIN(minutes_required) FROM recipes;
  ```

7. Find the recipe that takes the most time to prepare.

  ```
  SELECT MIN(minutes_required) FROM recipes;
  SELECT name FROM recipes where minutes_required = 15;
  ```

8. Find all the robots whose name starts with the letter M.

  ```
  SELECT name FROM robots WHERE name LIKE 'M%';
  ```

9. Count the number of board games that can be played by 8 people.

  ```
  SELECT COUNT (id) FROM board_games WHERE max_players = 8;
  ```

10. Find all animals that are swimming and egg-laying.

  ```
  SELECT * FROM animals WHERE swimming = true and egg_laying = true;
  ```

11. Find all animals that are swimming and egg-laying but not flying.

  ```
  SELECT * FROM animals WHERE swimming = true and egg_laying = true and flying = false;
  ```

12. Find the board game that supports the largest number of people.

  ```
  SELECT MAX(max_players) from board_games;
  SELECT name FROM board_games WHERE max_players = 30;
  ```
