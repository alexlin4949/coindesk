# CoinDesk

Use the Requests, pandas, and BeautifulSoup package to collect book information from http://books.toscrape.com/ 

By changing the lookup list on the last cell (under the #Main code), the program will starts collecting book information from each category and output as excel file. The default setting in lookup list is ['Science, 'Poetry']. 

The full list that can be put into the lookup list: ['Travel', 'Mystery', 'Historical Fiction', 'Sequential Art', 'Classics', 'Philosophy', 'Romance', 'Womens Fiction', 'Fiction', 'Childrens', 'Religion', 'Nonfiction', 'Music', 'Default', 'Science Fiction', 'Sports and Games', 'Add a comment', 'Fantasy', 'New Adult', 'Young Adult', 'Science', 'Poetry', 'Paranormal', 'Art', 'Psychology', 'Autobiography', 'Parenting', 'Adult Fiction', 'Humor', 'Horror', 'History', 'Food and Drink', 'Christian Fiction', 'Business', 'Biography', 'Thriller', 'Contemporary', 'Spirituality', 'Academic', 'Self Help', 'Historical', 'Christian', 'Suspense', 'Short Stories', 'Novels', 'Health', 'Politics', 'Cultura', 'Erotica', 'Crime']

The overall logic for this program:
1. Use the category_link function to collect link for each categories.
2. The books_link function uses the look up list from the user input to collect link for each books.
3. The find_des and find_info function will collect the book informations and description and combine them into one list called des. The function also collect and create the columns name for later use.
4. Use the output from previous functions to create a DataFrame and output as a excel file.


