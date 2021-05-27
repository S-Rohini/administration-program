class File:

  
   def get_accounts():
        with open('accounts.txt', 'r') as file:
            return file.read().split('\n')

   
    def add_account(username, password):
        with open('accounts.txt', 'a') as file:
            file.write(username)
            file.write(', ')
            file.write(password)
            file.write('\n')

    
    def get_students():
        with open('student_details.txt', 'r') as file:
            return file.read().split('\n')

   
    def add_student(student_details):
        with open('student_details.txt', 'a') as file:
            file.write(student_details)
            file.write('\n')

    
    def remove_student(student_id):
        pass
