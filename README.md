Hash Table Implementation with Linked List Chaining

This C program demonstrates the implementation of a hash table with linked list chaining to efficiently store and manage records. The records are read from an input file, hashed, and then inserted into the hash table. Additionally, the program includes functions to display the records stored in the hash table.
Code Structure

The program consists of the following key components:
struct RecordType

This structure defines the record type with fields for id, name, order, and a next pointer for linked list chaining.
struct HashType

This structure represents the hash table, containing a pointer to a RecordType. The hash table is initialized using calloc to ensure that all pointers are initially set to NULL.
hash Function

The hash function calculates the hash value for a given integer x and table size.
parseData Function

This function reads data from an input file, parses it, and stores it in an array of RecordType structures. It returns the size of the data.
printRecords Function

This function prints the records stored in an array of RecordType structures.
insertRecord Function

This function inserts a record into the hash table using the hash value to determine the index. If the index is unoccupied, the record is directly assigned. If the index is occupied, the record is added to the end of the linked list.
displayRecordsInHash Function

This function displays the records stored in the hash table, including linked list contents. It skips indices that are free.
main Function

The main function serves as the entry point. It reads records from the input file, inserts them into the hash table, displays the records in the hash table, and frees allocated memory.
Usage

To use this program, ensure you have an input file named "input.txt" with the appropriate data format. Compile and run the program, and it will display the records in the hash table.

