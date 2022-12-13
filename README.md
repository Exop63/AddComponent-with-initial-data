# AddComponent-with-initial-data
This is an extension of Component class of Unity.
 Youcan create any component with class name and intial with data.

  
  --------------------------------------------
  ```C#
 public class PlayerSetup : MonoBehaviour
 {
  public string m_Name = ""
  }
  
  var Name = "PlayerSetup";
  var data = new {<br>
      m_Name = "Player one"
  };<br>
  // it's retrun a Component type
  gameObject.AddComponent(Name, data);
  // retrun a T generic type
  // for this example T is PlayerSetup 
  gameObject.AddComponent<PlayerSetup>(Name, data);
  
```
