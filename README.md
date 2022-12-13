# 112
112
import java.io.BufferedReader;
import java.io.InputStreamReader;

public class QuerySourceCode {
  public static void main(String[] args) {
    String[] classNames = {
      "java.lang.String",
      "java.util.ArrayList",
      "java.util.HashMap"
    };

    try {
      for (String className : classNames) {
        // 执行 javap 命令
        Process p = Runtime.getRuntime().exec("javap " + className);
        
        // 读取命令的输出
        BufferedReader in = new
