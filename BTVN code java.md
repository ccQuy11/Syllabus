public class Test {
    public static void main(String[] args){
        System.out.println("Hello");

        for(int i = 0; i<= 5; i++){
            System.out.println("i = " + i);
        }
    }
}


đây là code của bài

Sử dụng javac Test.java để biên soạn file Test.java ra byte code  với tên file mới là Test.class

Sử dụng lệnh java sẽ ra kết quả là 

![image](https://github.com/user-attachments/assets/45cee380-8e08-4e11-9715-53a02ad4f07f)

Mô tả quá trình chạy 

JVM được khởi chạy.

JVM nạp file HelloWorld.class.

JVM tìm phương thức public static void main(String[] args) trong class đó.

JVM bắt đầu thực thi từ dòng đầu tiên trong main().

Sau đó dùng lệnh java -Xms64m -Xmx256m -XX:+UseG1GC Test


![image](https://github.com/user-attachments/assets/8146941e-f7a7-4468-9cb9-d5ac3f512aca)

đây là lệnh để chạy với cấu hình heap size, gc

mô tả

Xms: dung lượng ban đầu

Xmx: dung lượng tối đa

-XX:+UseG1GC: sử dụng GC để dọn dẹp phần thừa nếu dung lượng để chạy gần với mức tối đa
