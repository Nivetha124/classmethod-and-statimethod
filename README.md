# classmethod-and-statimethod
class Student:
    # class variables
    school_name = 'ABC School'

    def __init__(self, name, age):
        self.name = name
        self.age = age

   
    def show(self):
        print('Student:', self.name, self.age)
        print('School:', self.school_name)

   
    def change_School(cls, name):
         print('Previous School name:', cls.school_name)
        cls.school_name = name
        print('School name changed to', Student.school_name)

     def find_notes(subject_name):
        return ['chapter 1', 'chapter 2', 'chapter 3']


nivetha = Student('Nivetha', 12)
nivetha.show()


Student.change_School('Hari School')
