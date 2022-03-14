Part b:
	Empty array to assign and store values, in this case the elements are the words in the text Corleone.
	punctuation_replace function was created to replace the unnecessary values that consist as part of the string.
	The punctuations among the same words would be counted differently if they were not removed.
	The manner in which they are removed is by importing the string library, identifying their punctuations and replacing them with an empty string "".
	
Part c:
	To store the values for the two columns, word and count, a dictionary was created.
	The words in the array from Part a, were then stored into the dictionary and counted every iteration with a for loop.
	The Pandas library was later used to present the data in the dictionary as a dataframe.
	Orient was set as index to follow the requirements, and the columns I could not get them to identify as two seperae columns even though there clearly are two columns.
	Initially I thought of simply setting columns as: columns=['Word', 'Count'] but unfortunately it returns a dimensions error.
	The solutions to this issue was simply creating a 'Word:Count' single column name.
	
Part d:
	This part begins by importing all of the stop words not as a text file but rather copying and pasting all of the given words and storing them to an array.
	From there a data frame copy is made and set for the sorted words without the stop words as specified.
	Dropping all of the stop words, the results are then sorted in descending order according to count.
	
Part e:
	To store the amount of chapters, an empty array was initialized, along with setting a variable to state the inital count of the chapters is zero.
	Opening the file and reading its contents, they are then assigned as file.
	Corleone utilizes CHAPTER as the text to reference a new chapter, so that is what was used for a text splitter.
	From there a pop() method is used to remove the element at location 0.
	From the previous parts; dictionary, word counter, and now chapter count are used to keep and gather data on the chapters and their data.
	Two for loops are utilized to iterate through the words in each chapter and maintain clarity.
	The first for loop deals with all the words in each chapter split respectively and then revised whether they are words.
	If they are words, they get returned to the variable that stores all the words for each chapter.
	The second for loop deals with the processing of those words gathered from the first for loop.
	Each word is processed accordingly and will be stored in the dictionary.
	If the word is already in the dictionary for this specific chapter, then initialize as zero, else aggregate one to the current value.
	Finally all of the chapters are presented in the same format as the previous parts using the Pandas library data frame capabilities.
	
