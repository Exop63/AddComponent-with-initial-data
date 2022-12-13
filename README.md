# AddComponent-with-initial-data
This is an extension of Component class of Unity.
 Youcan create any component with class name and intial with data.

  
  --------------------------------------------
  ```
 public class PlayerSetup : MonoBehaviour<br>
 {<br>
  public string m_Name = ""<br>
  }<br>
  
  var Name = "PlayerSetup"; <br>
  var data = new {<br>
      m_Name = "Player one"<br>
  };<br>
  // it's retrun a Component type<br>
  gameObject.AddComponent(Name, data);<br>
  // retrun a T generic type<br>
  // for this example T is PlayerSetup <br>
  gameObject.AddComponent<PlayerSetup>(Name, data);
```
