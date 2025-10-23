# -FILE-HANDLING-UTILITY

Name:- DIVYA JAYANT KHACHANE
COMPANY:- CODETECH IT SOLUTION
DOMAIN:- JAVA PROGRAMMING
TASK1:- FILE HANDLING UTILITY
DURATION:- 4 WEEKS
MENTOR:- NEELA SANTHOSH KUMAR
ID:-CTO4DR697

# CREATE A JAVA PROGRAM TO READ,WRITE, AND MODIFY TEXT FILES

    [<img width="1121" height="327" alt="Image" src="https://github.com/user-attachments/assets/3aaab6f9-1af3-4e4c-8b0a-512f16628e07" />](https://github.com/Divyakhachane2006/-FILE-HANDLING-UTILITY/issues/1#issue-3543615801)

# DELIVERABLE: A SCRIPT DEMONSTRATING FILE OPERATIONS WITH CLEAR DOCUMENTATION
  def create_file(file_name):-"Creates a new file with the specified name"
        
            Args:
              file_name (str): The name of the file to be created
          Returns:
              None
          try:
              with open(file_name, 'w') as file:
                  pass
              print(f"File '{file_name}' created successfully.")
          except Exception as e:
              print(f"Error creating file: {e}")
          
  def write_to_file(file_name, content):-" Writes content to a file"

  
            Args:
              file_name (str): The name of the file to write to.
              content (str): The content to be written
          Returns:
              None
          try:
              with open(file_name, 'w') as file:
                  file.write(content)
              print(f"Content written to file '{file_name}' successfully.")
          except Exception as e:
              print(f"Error writing to file: {e}")

   def read_from_file(file_name):-"Reads content from a file"

   
              Args:
              file_name (str): The name of the file to read from  
          Returns:
              str: The content of the file 
          try:
              with open(file_name, 'r') as file:
                  content = file.read()
                  return content
          except Exception as e:
              print(f"Error reading from file: {e}")
              return 

  def append_to_file(file_name, content):-"Appends content to a file"

  
              Args:
                file_name (str): The name of the file to append to.
                content (str): The content to be appended
            Returns:
                None
            try:
                with open(file_name, 'a') as file:
                    file.write(content)
                print(f"Content appended to file '{file_name}' successfully.")
            except Exception as e:
                print(f"Error appending to file: {e}")

  def delete_file(file_name):-"Deletes a file"

  
                Args:
                file_name (str): The name of the file to be deleted
            Returns:
                None
            try:
                os.remove(file_name)
                print(f"File '{file_name}' deleted successfully.")
            except Exception as e:
                print(f"Error deleting file: {e}")

   def main(): file_name = "example.txt"
   
          
           # Create a file
          create_file(file_name)
          
          # Write to file
          write_to_file(file_name, "Hello, World!")
          
          # Read from file
          content = read_from_file(file_name)
          print(f"File Content: {content}")
          
          # Append to file
          append_to_file(file_name, "\nThis is appended content.")
          
          # Read appended content
          content = read_from_file(file_name)
          print(f"Appended File Content: {content}")
          
          # Delete file
          delete_file(file_name)
                    
