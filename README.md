                Console.Write("Age: "); 
                 var age = Convert.ToInt32(Console.ReadLine()); 
                 Console.Write("Year: "); 
                 var year = Convert.ToInt32(Console.ReadLine()); 
                 Console.Write("Gpa: "); 
                 var gpa = Convert.ToSingle(Console.ReadLine()); 
                  
                 try{ 
                     var student = new Student(name, age, year, gpa); 
                     database.AddStudent(student); 
                 } 
                 catch(Exception e) 
                 { 
                     Console.WriteLine(e.Message); 
                 } 
                 break; 
             case 2: 
                 Console.Write("Name: "); 
                 var name2 = Console.ReadLine(); 
                 Console.Write("Age: "); 
                 var age2 = Convert.ToInt32(Console.ReadLine()); 
                 Console.Write("Salary: "); 
                 var salary = Convert.ToDouble(Console.ReadLine()); 
                 Console.Write("JoinYear: "); 
                 var joinYear = Convert.ToInt32(Console.ReadLine()); 
  
                 try{ 
                     var staff = new Staff(name2, age2, salary, joinYear); 
                     database.AddStaff(staff); 
                      
                 } 
                 catch(Exception e) 
                 { 
                     Console.WriteLine(e.Message); 
                 } 
                 break; 
             case 3: 
                 Console.Write("Name: "); 
                 var name3 = Console.ReadLine(); 
                 Console.Write("Age: "); 
                 var age3 = Convert.ToInt32(Console.ReadLine()); 
  
                 try{ 
                     var person = new Person(name3, age3); 
                     database.AddPerson(person); 
                 } 
                 catch(Exception e) 
                 { 
                     Console.WriteLine(e.Message); 
                 } 
                 break; 
             case 4: 
                 database.PrintAll(); 
                 break; 
             default: 
                 return; 
             } 
         }  
     }   
 };
