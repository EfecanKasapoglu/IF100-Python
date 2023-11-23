library_input= input("Enter the library: ")
min_page_limit= int(input("Enter a minimum page limit: "))
holiday_length= int(input("Enter the holiday lenght in days: "))
reading_speeds= input("Enter the reading speed for genres: ")
books=library.split(";")
book_details= []

for book in books:
  book_info= book.split(":")
  book_genre= book_info[0]
  book_title=book_info[1]
  book_pages= int(book_info[2])
  book_details.append((book_genre,book_title,book_pages))
reading_speeds_list= reading_speeds.split(";")
genre_speeds= {}
for genre_speed in reading_speeds_list:
  genre,speed= genre_speed.split(":")
  genre_speeds[genre]= int(speed)
day_passed= 0
books_read= []
pages_read=0
books to donate=[]
for book in book_details:
  genre, title, pages= book
  if pages>= min_page_limit and genre in genre_speeds:
    days_to_finish= (pages/ genre_sppeds[genre]
    if days_passed + days_to_finish <= holiday_length:
      
      books_read.append(f"{title} finishes by day {day + days_to_read -1}.")
      pages_read += pages
      day += days_to_read
    else:
      books_to_donate.append(title)
if not books_read:
  print("No book to read! ")
else:
  print("Books Read: ")
  for book in books_read:
    print(book)
  print()
  print(f"Total number of pages read: {pages_read} \n")
if not books_to_donate:
  print("No book to donate! ")
else:
  print("Books to donate: ")
  for i in range(len(books_to_donate)):
    print(str(i+1)+"."+ books_to_donate[i])
