```java
package Seungmin;

import java.util.Arrays;
import java.util.HashMap;
import java.util.Map;

public class Me {

    private String name, position, web, youtube, instagram;
    private Map<String, String[]> skills;
    private String[] architecture;
    private String[] hobbies;

    public Me() {
        // Personal Information
        this.name = "SeokSeungMin";
        this.position = "Backend Developer";
        this.web = "seokseungmin.github.io/";
        this.youtube = "https://www.youtube.com/@seokseungmin";
        this.instagram = "https://www.instagram.com/stone.seok/";

        // Skills and Technologies
        this.skills = new HashMap<>();
        this.skills.put("programming", new String[]{"HTML", "CSS", "JavaScript", "Java", "Kotlin"});
        this.skills.put("frameworks", new String[]{"Spring", "Firebase"});
        this.skills.put("tools", new String[]{"IDEA", "Eclipse", "Android Studio", "Postman"});
        this.skills.put("databases", new String[]{"MySQL"});
        this.skills.put("buildTools", new String[]{"Maven", "Gradle"});
        this.skills.put("versionControl", new String[]{"Git"});

        // Architectural Knowledge
        this.architecture = new String[] {
            "MVC Pattern with Spring Framework",
            "Database Design and Optimization with MySQL",
            "Web Application Development with Java and JSP",
            "Design Patterns in Software Development",
            "Algorithmic Problem Solving",
            "Spring Boot Microservices Architecture"
        };

        // Hobbies
        this.hobbies = new String[]{"Listening to Music", "Watching OTT services", "Playing Video Games"};
    }

    public String[] getMyHobbies() {
        return hobbies;
    }

    public String getFutureGoal() {
        return "Becoming a Back-End Developer.";
    }

    public String getSkillsAsString() {
        StringBuilder skillsStr = new StringBuilder();
        for (Map.Entry<String, String[]> entry : skills.entrySet()) {
            skillsStr.append(entry.getKey()).append(": ").append(Arrays.toString(entry.getValue())).append("\n");
        }
        return skillsStr.toString();
    }

    public String getArchitectureAsString() {
        return "Architecture: " + Arrays.toString(architecture);
    }
    
    @Override
    public String toString() {
        return "Hello, my name is " + name + ".\n" +
               "I am currently aspiring to be a " + position + ".\n" +
               "Check out my website: " + web + "\n" +
               "Find me on YouTube: " + youtube + "\n" +
               "Follow me on Instagram: " + instagram+ "\n\n" +
               "Here are some of the skills I have developed:\n" + getSkillsAsString() + "\n" +
               "My knowledge in architecture includes:\n" + getArchitectureAsString() + "\n" +
               "My hobbies include: " + Arrays.toString(hobbies) + "\n" +
               "My future goal is to become " + getFutureGoal();
    }
}

class Main {
    public static void main(String[] args) {
        Me me = new Me();
        System.out.println(me);
    }
}

```


<div align="center">

[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2F&count_bg=%23FFA500&title_bg=%23545454&icon=github.svg&icon_color=%23E7E7E7&title=Views&edge_flat=false)](https://hits.seeyoufarm.com)<br>

# Languages & Tools

![Front-end](https://skillicons.dev/icons?i=html,css,js,java,kotlin,spring,idea,eclipse,androidstudio,firebase,mysql,postman,maven,gradle,git)<br>

</div>

