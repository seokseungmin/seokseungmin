```java
package Seungmin;

import java.util.Arrays;
import java.util.HashMap;
import java.util.Map;

public class Me {

    private final String name = "SeokSeungMin";
    private final String position = "Backend Developer";
    private final String web = "seokseungmin.github.io/";
    private final String youtube = "https://www.youtube.com/@seokseungmin";
    private final String instagram = "https://www.instagram.com/stone.seok/";
    private final Map<String, String[]> skills;
    private final String[] hobbies = {"Listening to Music", "Watching OTT services", "Playing Video Games"};

    public Me() {
        skills = new HashMap<>();
        skills.put("programming", new String[]{"HTML", "CSS", "JavaScript", "Java", "Kotlin"});
        skills.put("frameworks", new String[]{"Spring", "Firebase"});
        skills.put("tools", new String[]{"IDEA", "Eclipse", "Android Studio", "Postman"});
        skills.put("databases", new String[]{"MySQL"});
        skills.put("buildTools", new String[]{"Maven", "Gradle"});
        skills.put("versionControl", new String[]{"Git"});
    }

    private String getSkillsAsString() {
        StringBuilder skillsStr = new StringBuilder();
        for (Map.Entry<String, String[]> entry : skills.entrySet()) {
            skillsStr.append(entry.getKey()).append(": ").append(Arrays.toString(entry.getValue())).append("\n");
        }
        return skillsStr.toString();
    }

    @Override
    public String toString() {
        return "Hello, my name is " + name + ".\n" +
               "I am currently a " + position + ".\n" +
               "Check out my website: " + web + "\n" +
               "Find me on YouTube: " + youtube + "\n" +
               "Follow me on Instagram: " + instagram+ "\n\n" +
               "Here are some of the skills I have developed:\n" + getSkillsAsString() + "\n" +
               "My hobbies include: " + Arrays.toString(hobbies);
    }

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

