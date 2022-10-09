# 📌 final class

> 상속을 금지함

🔻 부모 클레스
``` java
public final class Human {
  ...
}
```

🔻 자식 클레스
> public class Leekyukin <del>extends Human</del> {...}

- final class는 상속할 수 없음

# 📌 final method


🔻 부모 클레스
``` java
public final class Human {

  private String name;

  public void setAge(String name) {
    this.name = name;
  }
}
```

🔻 자식 클레스
> public final class Humanㅤ{  <br>
>  <br>
>  ㅤㅤprivate String name; <br>
>  <br>
>  ㅤㅤpublic void <del>setAge(String name)</del>ㅤ{  <br>
>  ㅤㅤㅤthis.name = name;  <br>
> ㅤㅤ} <br>
> } <br>

- final method는 overriding 불가능



