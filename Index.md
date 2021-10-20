<!DOCTYPE html>
<head>
    <strong>Robert Swanke | Software Engineer</strong>
<head>
<br>
<br>
<br>
    
<strong>Self - Assessment:</strong>
<br>
<br>
<strong>Overview:</strong>
<br>
There are many different aspects to my programming projects that I believe showcase my strengths in the computer science industry. I think to start, showing my capability of understand multiple languages shows my versatility. During my time within the Computer Science Software Engineering program at Southern New Hampshire I learned a good amount of technical skills and techniques that will last a lifetime and that are directly used while working within the field. There are many skills less technical than the others, but all of them are critical to making a successful real-world application. I think programs that have the ability to use or be changed into more than one language can be extremely powerful in the software engineering realm. Both the data structures and algorithms project were based off of the Java programming language. I think these projects show my understanding of object-oriented programming and algorithms, including traversal methods and search options. Finally, for the database project I created it in MongoDB with the Python language. This artifact helped to show my understanding of databases and how to correctly implement API's with CRUD operations.
<br>
<br>
<strong>Team Environments</strong>
<br>
When it comes to collaborating in a team environment, I believe that I learned the most from using Git when it comes to programming. I only used Github a handfull of times before I started at SNHU, so learning how to commit, pull, and set up a dashboard helped me to better understand Git. I think that this is the primary source of team environments and collaboration in today's work enviroment. Knowing how to use Git is important for any team environment. The same holds true for any repository.
<br>
<br>
<strong>Communicating to Stakeholders</strong>
<br>
I do not think that my projects directly communicate with stakeholders, but I believe that they can see their own system implementented into the things I have done. It might not be catter for them at the given moment but I can be redone to benefit them further. I have a clear derivative for each of my programs and am able to  meet the goals. It is important when communicating to stake holders that you can establish what your project can and can not do, how it can and can not be implemented, and a complete pathway forward to completeion.
<br>  
<br>
<strong>Software Design and Engineering</strong>
<br>
Software engineering is the focus of all of the projects. Although, the focus was to enhance the projects, correct mistakes, take out anything extra and add anything that might of been a second thought. I also believe I showed my software engineering skills in different ways in the data structures & algorithms project and the database project. Adding and updating the code was a challenge as it has been a while since I have dealt with these projects but I believe I was able to be successful and make improvements upon the original code. The database program which was a full stack project made use of many different frameworks and packages. All of which led to a functional database.  
<br>
<br>
<strong>Data Structures and Algorithms</strong>
<br>
Data structures and algorithms are the primary focus of the second artifact. Overall, I think  that I was able to convey my understanding of data structures in this artifact pretty well. I used both a singly linked list and a binary tree for the data structures. Each of these methods hold data in different ways. I believe having two data structures instead of one was beneficial to showing my ability of creating data structures. I also used a few different traversal methods for these data structures. These algorithms allow for traversing through the data structures at a quick efficiency, along with searching through the linked list correctly. Data structures and algorithms are the backbone to a large amount of software engineering, and I believe I was able to correctly convey my skill in these categories.
<br>
<br>
<strong>Database</strong>
<br>
My artifact for the database project was created using MongoDB, JavaScript, Node.JS, Express and Mongoose. There are a few components for this database and I found this artifact the most challenging out of all of them since it dealt with the front end, back end, a database and then connecting them. The database is primarily a restful API that uses the standard CRUD methods. MongoDB is the database that is used to store information such as indexes, documents, and models. This project was by far the most difficult, I struggled with the database project the more than any other project to date but it showed me that I at least have a decent grasp on databases and how to correctly implement them into a project. Although the algorithms are fairly simple, I believe I was able to implemented them in conjunction with the .xlsl files with reading and writing included with Pandas.
<br>
<br>
<strong>Security</strong>
<br>
Society’s increasing reliance upon the internet for things like finance and communication means that cybercrime promises to be even more profitable in the future. Cybercrime is a huge industry and is here to stay. Companies need to prepare properly to combat it and programmers can help combat cybercrimes by using the set coding standards.    
<br>
<br>
<strong>Reason for Inclusion</strong>
<br>
I decided to chose these three artifacts because I believe they show different skills in the computer science industry. The code conversion, variables updates, structure, arithmetic operations, loops and defensive programming all focus on my software engineering and language skills. The data structures focus primarily on my object-oriented programming skills and the database focuses on the understanding of how to develop and implement a fullstack. These programs do not function together but they all show separate skills that I think are extremely useful when programming. Overall, I believe I was able to convey my skills and accurately portray them in my portfolio and am looking forward to what the future brings for me with in the software engineering industry. 
    
    
</body>

</html>


### Software Design and Engineering (IT-145: Foundation in Application Development)
	
[Zoo Authentication System: Pre-Enhancements](https://github.com/RJSwanke/RJSwanke.github.io/tree/main/ZooAuthenticationSystem%20-%20Pre-Enhancement)

[Zoo Authentication System: Final](https://github.com/RJSwanke/RJSwanke.github.io/tree/main/ZooAuthenticationSystem)

#### Artifact explanation:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;My artifact is based off of my final project from my IT-145: Foundation in Application Developmen course. The project is a Java program that implements a authentication system along with an MD5 password hashing function. I created this artifact a couple years ago initially as it was one of my first classes at SNHU. The artifact that is included in my portfolio is the same essential program but with minor improvements like in the structure, variables, arithmetic operations, loops and security.

#### Reason for inclusion in portfolio:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;I decided to include this project in my ePortfolio because it shows my proficiency with the Java programming language. Java has been and still is one of the most commonly used object-oriented programming languages in the world. By showing my familiarity with Java it will also show that I understand things like software architecture, proper coding standards and other rules that the community follows. 

#### What the program does: 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The program opens a .txt file based on the user’s login information and then prints it out to the user. The login information contains a user type, a username, and a user password. The password and username are inputted while the type is assigned in the program based on the user’s credentials. The user’s type is passed along with the password to an MD5 conversion function to authenticate the user's login credientials.
```


    //login loop
    //obtain userName & password
        while (true) {
            logout = false;
            userInput = new Scanner(System.in);
            System.out.print("Enter username: ");
            userName = userInput.nextLine();
            System.out.print("Enter password: ");
            password = userInput.nextLine();
            authFile = areCreditialsValid(userName, password);

    //successful login: display role info and logout option
            if (authFile != null) {
                
    //loop until logout
    //display user role information if login successful
                while (true) {
    //add display information
                    displayAuthorizedInformation(authFile);
                    System.out.print("Press \"Q\" to logout: ");
                    String choice = userInput.nextLine();

    //need to give logout option
                        if (choice.equalsIgnoreCase("Q")) {
                            System.out.println("\nLogging out now...");
                            numAttempts = 0;                           
                            logout = true;
                            break;
                        }
                        System.out.println();
                }
            }
            
    //3 attempts will give an unsuccessful login            
            else {
                numAttempts++;
                
                if (numAttempts == 3) {
                    System.out.println("\nTo many unsuccessful login attempts!\nExiting the program...");
                    break;
                }

                else {
                    System.out.println("Invalid username and/or password! Please try again!");
                    System.out.println((3 - numAttempts) + " attempts remain.\n");
                }
            }
            
    //logout with exit option
            if (logout) {
                System.out.print("\nPress \"Q\" to quit application. Press any other key to login as a different user.");
                continueApp = userInput.nextLine();

                if (continueApp.equalsIgnoreCase("Q")) {
                    System.out.println("\nExiting the application...");
                    break;
                }
            }
            
            System.out.println();
        }
    }


    //connect to MD5digest class and login
    //connect to main
    public static String areCreditialsValid(String userName, String password) {

        String md5Password = MD5Digest.md5HashCode(password);
        Scanner fileReader;
        String zooAuthRecord = null;
    
    //checks login against credentials
        try {
            fileReader = new Scanner(new File("credentials.txt"));

            while (fileReader.hasNextLine()) {
                zooAuthRecord = fileReader.nextLine();
                String credCols[] = zooAuthRecord.split("\t");
                
                if (credCols[0].trim().equals(userName)) {
                    
                    if (credCols[1].trim().equals(md5Password)) {
                        return credCols[3];
                    }
                }
            }
            
            fileReader.close();
        }

        catch (FileNotFoundException e) {
        }
        
        return null;
    }
```
#### What I learned: 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;I learned a few things from revisiting this artifact. One of those things is how different but also how similar certain languages can be. I haven't been doing Java lately but it was very easy to pick back up and understand what is going on. I do believe my experience has helped with this but I am not sure if I had to do this a year ago I would be as successful. Things tend to be a bit more simplified in other languages but the implementation of some features can be much more confusing. Every language has it's pros and cons. Overall the code isn't that complex, so the main challenge for me came from brushing up on my Java knowledge and finding ways to implement certain functions. 

------------------------------------------------------------
------------------------------------------------------------

## Data Structures and Algorithms (CS-365: Operating Environments)

[Multithreads: Pre-Enhancements](https://github.com/RJSwanke/RJSwanke.github.io/tree/main/Multithreads%20-%20Pre-Enhancement)
	
[Multithreads: Final](https://github.com/RJSwanke/RJSwanke.github.io/tree/main/Multithreads)

#### Artifact explanation:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This artifact is a program that tests your implementation that lists all thread groups and threads within each group in the JVM.

#### Reason for inclusion in portfolio:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;I decided to include this project in my ePortfolio because it shows my proficiency within the Java programming language and being able to call on outside functions to create threads within the original. Java has been and still is one of the most commonly used object-oriented programming languages in the world. By showing my familiarity with Java it will also show that I understand things like software architecture, proper coding standards and other rules that the community follows. Java is one of the most common languages and I want to show my familiarity with it.

#### What the program does: 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The program aka the threading event object allows one thread to signal an event while an unlimited amount of other threads can be waiting for that event to happen. The key usage in this code is that the threads that are waiting for the event do not necessarily need to stop what they are doing, they can just check the status of the event every once in a while.
```
for (ThreadGroup groupList1 : groupList) {
	//create thread array with double active threads
            	Thread[] list = new Thread[groupList1.activeCount() * 2];
            	groupList1.enumerate(list, false);
	//print group name
	//print list of threads in the groups and their status
            	System.out.println(groupList1.getName());
                	for (Thread list1 : list) {
                    	if (list1 != null) {
                        	System.out.println("\t" + list1.getName() + ":" + list1.getId() + ":" + list1.getState() + ":" + list1.isDaemon());
                    	}

```
#### What I learned: 
These for-loops are better structured this way, they read better and are more secure. After correcting the structure I added to the comments and made sure they were easy to read and not hard to find. I believe that I enhanced this project so that now it is a nice polish project that I am proud to have in my ePortfolio. Reflecting on the process of enhancing and/or modifying my artifact taught me that even though I don't fully understand what is going on, I am still able to read the code and notes to figure out anything I don't understand. With every project I enhance I become more familiar with what a solid software program's code is supposed to look like.    

------------------------------------------------------------
------------------------------------------------------------

## Databases (CS-340: Advanced Programming Concepts)

[Dashboard: Pre-Enhancements](https://github.com/RJSwanke/RJSwanke.github.io/tree/main/Dashboard%20-%20Pre-Enhancement)
	
[Dashboard: Final](https://github.com/RJSwanke/RJSwanke.github.io/tree/main/Dashboard)

#### Artifact explanation:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The artifact from CS 340: Advanced Programming Concepts is a MongoDB client and user interface that allows users to access data about their business which in this case is an animal shelter. This project was written in Python and uses MongoDB.

#### Reason for inclusion in portfolio:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This project is a great project to display in my ePortfolio since it is a different language than Java, uses a database and is a full stack build. Python is a language that is quickly gaining popularity especially in the artificial intelligence world. Having a basic understanding of Python for me shows that I am a diversified programmer that isn't just locked to one language.

#### What the program does: 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This program allows any user to store, change, updates, move and/or retrieve data from a database of their making. It also has other utilities like GPS and search options with a full interface. Below is an example of the radio buttons that were added and the update to the chart & map.
```
    #Radio Buttons
    ),
    html.Hr(),
    dcc.RadioItems(
        id='dogtype',
        options=[
            {'label': 'Water Rescue', 'value': 'Water'},
            {'label': 'Mountian Rescue', 'value': 'Mountian'},
            {'label': 'Disaster Rescue', 'value': 'Disaster'},
            {'label': 'Reset', 'value': 'Reset'}
        ],
        value='MTL',
        labelStyle={'display': 'inline-block'}
    ),
    dt.DataTable(
        id='datatable-id',
        columns=[
            {"name": i, "id": i, "deletable": False, "selectable": True} for i in df.columns
        ],
        data=df.to_dict('records'),
        filter_action='native',
        sort_action='native',
        sort_mode='multi',
        row_selectable='single',
        page_action='native',
        page_current=0,
        page_size=10,

    ),
    html.Br(),
    html.Hr(),
    
    #Chart & Map
    html.Div(className='row',
             style={'display': 'flex'},
             children=[
                 html.Div([dcc.Graph(id="pie-chart")]),
                 html.Div([
                     dl.Map(id='map-id', className='col s12 m6', style={'width': '1000px', 'height': '500px'}, center=[30.75, -97.48], zoom=10, children=[
                         dl.TileLayer(id="base-layer-id"),
                         
                         #Marker,tool tip & popup
                         dl.Marker(position=[30.75, -97.48], children=[

                             dl.Tooltip(df.iloc[0, 4]),
                             dl.Popup([
                                 html.H1("Animal Name"),
                                 html.P(df.iloc[1, 1])

                             ])

                         ])
                     ])

                 ]),
             ])
])

```

![Screenshot (194)](https://user-images.githubusercontent.com/49452450/137618638-ed783840-d6bb-4a67-99ac-a70967ab105d.png)
![Screenshot (193)](https://user-images.githubusercontent.com/49452450/137618641-482b5b60-27ee-41a6-b826-54518668912f.png)

#### What I learned: 
This project taught me a lot by focuses on the understanding of how to develop and implement a fullstack. The knowledge I gained I have been able to apply to other projects. This is a fullstack build and was one of the first times I connected the front end to the back end and then to a database. This project taught me that sometimes trial and error is the only way to figure certain things out.  
