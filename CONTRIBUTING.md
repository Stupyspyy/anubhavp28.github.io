include<stdio.h>
void main()
{
    int i,j,k,l,fre[20]={0},a[]={43,65,51,27,79,11,56,61,82,9,25,36,7,49,55,63,74,81,49,37,40,49,16,75,87};
    for(i=0;i<25;i++)
    {
        if(a[i]>=0 && a[i]<10)
            fre[1]+=1;
        else if(a[i]>=10 && a[i]<20)
            fre[2]+=1;
        else if(a[i]>=20 && a[i]<30)
            fre[3]+=1;
        else if(a[i]>=30 && a[i]<40)
            fre[4]+=1;
        else if(a[i]>=40 && a[i]<50)
            fre[5]+=1;
        else if(a[i]>=50 && a[i]<60)
            fre[6]+=1;
        else if(a[i]>=60 && a[i]<70)
            fre[7]+=1;
        else if(a[i]>=70 && a[i]<80)
            fre[8]+=1;
        else if(a[i]>=80 && a[i]<90)
            fre[9]+=1;
        else if(a[i]>=90 && a[i]<100)
            fre[10]+=1;
    }
        printf("group\trange\tfrequency\n");
        for(i=0;i<10;i++)
        {
        printf("%d\t%d-%d\t%d",i+1,i*10,i*10+9,fre[i]);

        printf("\n");
        }

}
