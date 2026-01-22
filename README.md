# weather-report-c-lang
#include <stdio.h>
int main() {
	int a[7],avg,sum,n,m;
	for(int i=0;i<7;i++){
	    scanf("%d",&a[i]);
	}
	for(int i=0;i<7;i++){
	    
	    sum += a[i];
	}
	avg = sum/7;
	printf("Average temperature for the week : %d\n",avg);
	int min,max;
	min = a[0];
	for(int i=0;i<7;i++){
	    if(a[i]<min){
	        min = a[i];
	    }
	}
	max = a[0];
	for(int i=0;i<7;i++){
	    if(a[i]>max){
	        max = a[i];
	    }
	}
	printf("The highest temp of the week was %d\nThe lowest temp of the week was %d\n",max,min);
    for(int i=0;i<7;i++){
        if(max==a[i]){
            n = i+1;
        }
    }
    for(int i=0;i<7;i++){
        if(min==a[i]){
            m = i+1;
        }
    }
    printf("Highest temp - Day%d\nLowest temp - Day%d",n,m);
}
