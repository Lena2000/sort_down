# sort_down
//Сортировка по убыванию

package org.apache.poi.hssf.usermodel;

import java.util.Arrays;


public class Main {

    public static void main(String[] args) {
        int[] arr = {5, 8, 1, 0, 44, 78, 2, 3};
        System.out.println(Arrays.toString(arr) + "-------->");

        for (int i = arr.length-1; i > 0; i--) {
            for (int k = 0; k<i; k++) {

                if (arr[k]<arr[k+1]){
                    int c = arr[k+1];
                    arr[k+1]=arr[k];
                    arr[k]=c;

                }
                System.out.println(Arrays.toString(arr));
            }
        }
    }
}
