# 计G202 2020322099 邱煜斐
# 实验5

## 实验内容：
    ·业务要求：在某课上,学生要提交实验结果，该结果存储在一个文本文件A中。
              文件A包括两部分内容：
              1，是学生的基本信息；
              2，是学生处理后的作业信息，该作业的业务逻辑内容是：利用已学的字符串处理知识编程完成《长恨歌》古诗的整理对齐工作，写出功能方法，实现如下功能：
                (1).每7个汉字加入一个标点符号，奇数时加“，”，偶数时加“。”
                (2).允许提供输入参数，统计古诗中某个字或词出现的次数
                (3).输入的文本来源于文本文件B读取，把处理好的结果写入到文本文件A
                (4).考虑操作中可能出现的异常，在程序中设计异常处理程序
              输入内容：
                  汉皇重色思倾国御宇多年求不得杨家有女初长成养在深闺人未识天生丽质难自弃一朝选在君王侧回眸一笑百媚生六宫粉黛无颜色春寒赐浴华清池
              温泉水滑洗凝脂侍儿扶起娇无力始是新承恩泽时云鬓花颜金步摇芙蓉帐暖度春宵春宵苦短日高起从此君王不早朝承欢侍宴无闲暇春从春游夜专夜后宫
              佳丽三千人三千宠爱在一身金屋妆成娇侍夜玉楼宴罢醉和春姊妹弟兄皆列士可怜光采生门户遂令天下父母心不重生男重生女骊宫高处入青云仙乐风飘
              处处闻缓歌慢舞凝丝竹尽日君王看不足渔阳鼙鼓动地来惊破霓裳羽衣曲九重城阙烟尘生千乘万骑西南行<未完，待续>

              输出内容：
              汉皇重色思倾国，御宇多年求不得。
              杨家有女初长成，养在深闺人未识。
              天生丽质难自弃，一朝选在君王侧。
              回眸一笑百媚生，六宫粉黛无颜色。
              春寒赐浴华清池，温泉水滑洗凝脂。
              侍儿扶起娇无力，始是新承恩泽时。
              云鬓花颜金步摇，芙蓉帐暖度春宵。
              春宵苦短日高起，从此君王不早朝。
              …………

    ·实验要求：
      1.设计学生类（可利用之前的）；
      2.采用交互式方式实例化某学生；
      3.设计程序完成上述的业务逻辑处理，并且把“古诗处理后的输出”结果存储到学生基本信息所在的文本文件A中。

      
## 实验目的：
    ·掌握字符串String及其方法的使用
    ·掌握文件的读取/写入方法
    ·掌握异常处理结构

## 实验过程：
    ·首先在Students.java中创建Personner父类，并赋予其子类可能用到的元素，然后将学生还有老师的类继承（extends）父类并添加特定元素和属性，从而完成Students.java。
    ·然后在LIst.java中使用set方法写入相应信息，在使用get方法调用相应的信息，然后调用并输出输出相应结果，从而达到测试主类，模拟选课，模拟退课，展示信息的操作。
    ·其他具体详情见核心代码环节
## 核心代码：
    ·1，定义父类，继承代码展示：
    ···
    class personner
    public class Students extends Personner{}
    class Teacher extends Personne{}
    ···
    ·2，这里我们需要用到java.text.SimpleDateFormat类的format方法,其中可以指定年月日时分秒的模式字符串格式。
    ···
    import java.text.SimpleDateFormat;
    import java.util.Date;
    SimpleDateFormat df = new SimpleDateFormat("yyyy-MM-dd HH:mm:ss");//设置日期格式
    ···
    ·3，使用set写入，get调用输出。
## 输出结果：
![](https://github.com/qiuyufei/shiyan3/blob/main/1.png)

## 实验感想：
    ·首先明确了java代码的大框架，明确了子类父类的关系可以使用继承，一个子类只能有一个父类。
    ·其次目前可以比较熟练的使用set和get方法，来达成自己的目的。
    ·然后此次代码的完成在没有思路时完成的很困难，去同学哪里取了不少经，以后会匀出时间去钻研研究。
