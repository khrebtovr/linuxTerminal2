# linuxTerminal2

| `Description` | `Command` |
| :---        |  :---  |
| 1. Make folder dir_1 | **mkdir dir_1** |
| 2. Go to the dir_1 folder | **cd dir_1** |
| 3. Create folder inner_dir_1 | **mkdir inner_dir_1** |
| 4. See where you are | **pwd** |
| 5. Being in the dir_1 folder, create an empty text file tf_1.txt | **touch tf_1.txt** |
| 6. Being in the dir_1 folder, use the cat command to create a text file tf_2.txt with the following lines: | **cat > tf_2.txt** |
|- the first 1 |  |
|- second 2 |  |
|- the third 3 |  |
| 7. Go to the folder inner_dir_1 | **cd inner_dir_1** |
| 8. Through cat make a text file tf_3.txt with any lines | **cat > tf_3.txt** |
| 9. Through cat add the line “the second 2” to the text file tf_3.txt | **cat >> tf_3.txt** |
| 10. Through cat add the line “the sec 2” to the text file tf_3.txt | **cat >> tf_3.txt** |
| 11. Through cat add the line “the sec 3” to the text file tf_2.txt | **cat >> ../tf_2.txt** |
| 12. Through cat add the line “the SeCoNd 2” to the text file tf_3.txt | **cat >> tf_3.txt** |
| 13. Through cat add the line “the seConD 2” to the text file tf_2.txt | **cat >> ../tf_2.txt** |
| 14. Make a text file tf_4.txt which will contain 15 lines | **vim tf_4.txt (added text)** |
| 15. Make a text file tF_5.txt which will contain 13 lines | **vim tF_5.txt (added text)** |
| 16. List all files in a folder | **ls -la** |
| 17. Exit folder inner_dir_1 | **cd ..** |
| 18. Output the contents of the tf_3.txt file to the terminal | **cat inner_dir_1/tf_3.txt** |
| 19. Find the path to the file tf_4.txt | **find . -name "tf_4.txt"** |
| 20. Clear the tf_4.txt file from the contents without deleting the file itself | **> ./inner_dir_1/tf_4.txt** |
| 21. Find the path to files that have "tf" in their names | **find . -name "*tf*"** |
| 22. Find the path to files that have "tf" in the name and letters in any case | **find . -iname "*tf*"** |
| 23. Find lines in files where there is a combination of letters “sec” in the current folder | **grep sec * ** |
| 24. Find lines in files where there is a combination of letters “sec” in any case in the current folder | **'grep -i sec *' ** |
| 25. Find lines in files where there is only a combination of letters “sec” in the current folder | **grep -w sec * ** |
| 26. Find lines in files where there is only a combination of letters “sec” in any case in the current folder | **grep -w -i sec * ** |
| 27. Find lines in files where there is a combination of letters “second” in the current folder | ** grep second * ** |
| 28. Find lines in files where there is a combination of letters “second” in any case in the current folder | ** grep -i second * ** |
| 29. Find lines in files where there is a combination of letters “second” in all folders below the level | ** grep -r "second" / ** |
| 30. Find only the path and file name in the lines in | **grep -rl "second" . | cut -d '/' -f 2-** |
| which there is a combination of letters “second” in the current folder | ** grep -v -r second * ** |
| 31. Find all lines in all files where there is no “second” combination | **  ** |
| 32. Find only the name and path to files where there is no “second” combination | |
| 33. Print to the terminal the last 4 lines of any text file | **tail -n 4 inner_dir_1/tF_5.txt** |
| 34. Output to terminal 4 the first lines of any text file | **head -n 4 inner_dir_1/tF_5.txt** |
| 35. Command in one line. Create a folder and create a text file with contents | **mkdir dir_2 && echo "Hello, world!" > dir_2/hello.txt ** |
| 36. Command in one line. Move to any one folder text files that have the word “sec” in their content | ** grep -l 'sec' *.txt | xargs mv -t dir_2/ ** |
| 37. Command in one line. Copy to any one folder text files that have the word “sec” in their content | ** grep -l 'sec' *.txt | xargs cp -t dir_2/ ** |
| 38. Command in one line. Find all lines with "sec" in all text files | ** find . -name "*.txt" -type f -exec grep "sec" {} \; | cat > new_file.txt ** |
| and Copy and paste these lines into one newly created text file | |
| 39. Command in one line. Delete text files that have the word “sec” in their content | ** find . -name "*.txt" -type f -exec grep -q "sec" {} \; -delete ** |
| 40. Just print the line “Good job!!” | **echo "Good job!!"** |
