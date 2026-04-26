# lecture1  List 

//List Inside List

List<String> shortTermCourses = new List<String>{'Apex','flow','Trigger','Aura','lwc','Integration'};  
List<String> LongTermCourses = new List<String>{'Salesforce Admin','Salesforce Development','Interview Preperation'};
    List<List<String>> Courses = new List<List<String>>{shortTermCourses,LongTermCourses} ;
        system.debug(Courses);

for(List<String>Course:Courses){     // for each loop functions
    system.debug(Course);
    
    // you can print in each element in the list
    
    for(String singlelement:Course){
        system.debug(singlelement);
    }
}
