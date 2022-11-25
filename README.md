# 25-11.22
{https://www.codewars.com/kata/51edd51599a189fe7f000015}
error square
My solution:
public class Solution {
  public static double solution(int[] arr1, int[] arr2) {
    double res=0;
    for(int i=0;i<arr1.length;i++)
      {
      res+=(arr1[i]-arr2[i])*(arr1[i]-arr2[i]);
    }
    return res/(arr1.length);
  }
}
My favourite solution:
public class Solution {
    public static double solution(int[] arr1, int[] arr2) {
        return java.util.stream.IntStream.range(0, arr1.length).map(i -> arr1[i] - arr2[i]).map(diff -> diff * diff).average().getAsDouble();
    }
}
