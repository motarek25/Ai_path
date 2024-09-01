import numpy as np
np1 = np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])
print(np1)
print(np1[1:5])
print(np1.shape)
np2=np.arange(8)
print(np2)
np3=np.arange(0,10,2)#start end steps
print(np3) 
np4=np.zeros(10)
print(np4) 
np5=np.zeros((2,10))
print(np5) 
np6=np.full((10),6)#(count of element) ,val
print(np6) 
np7=np.full((2,10),6)#(columns,count of ele),val 
print(np7) 
l=[1,3,65,78,3,76,54,765,21,56]
np8=np.array(l)
print(np8)
print(np8[2])
print(np8[0:6:2])#start:end:step
# print(l[0:6:2])#start:end:step
np9=np.array([[1,5,7,8,9,4],[11,33,65,78,45,8],[12,34,87,98,56,43]])
print(np9[1,4])
print(np9[0:2,0:4])
# math
np10=np.array([4,9,16,25])
print(np.sqrt(np10))
np11=np.array([-4,-9,-16,25,0])
print(np.absolute(np11))
print(np.max(np11))
print(np.min(np11))
print(np.sign(np11))
print(np.sin(np10))
print(np.cos(np10))
print(np.log(np10))
# find more from dic..
np12=np.array([1,2,4,6,7,8,6,54,9])
npv=np12.view()
print(np12)
print(npv)
np12[3]=90#the change will happen in npv
print(np12)
print(npv)
np13=np.array([10,20,40,60,70,80,60,54,90])
npc=np13.copy()
print(np13)
print(npc)
np13[3]=99#the change will not  happen in npc
print(np13)
print(npc)
# shap (count of rows , count of element) and reshap
print(np12.shape)
print(np9.shape)
print(np7.shape)
np14=np.array([1,2,3,4,5,6,7,8,9,10,11,12])
nprs=np14.reshape(4,3)
print(nprs)
print(nprs.shape)
npr=np14.reshape(2,3,2)
print(npr)
print(npr.shape)
npback=np14.reshape(-1)
print(npback)
print(npback.shape)
# for loop 
npf1=np.array([1,2,3,2,4,5,6,8,9,77,88,65,3,2,23,46,79])
npf2=np.array([[1,3,4,5,6],[7,8,9,33,44]])
npf3=np.array([[1,3,4,5,6],[2,7,4,90,87],[7,8,9,33,44]])
npf4=np.array([[[1,3,4,5,6],[2,7,4,90,87]],[[7,8,9,33,44],[2,3,6,8,5]]])
# for i in npf1:
    # print(i)
# for i in npf2:
    # print(i)
#     for y in i:
#         print(y)
# for i in npf3:
    # print(i)
    # for y in i:
        # print(y)
# for i in npf4:
    # print(i)
    # for y in i:
        # print(y)
        # for z in y:
            # print(z)#==
# for x in np.nditer(npf4):
#     print(x)
# for x in np.nditer(npf1):
#     print(x)
# for x in np.nditer(npf3):
#     print(x)
print(np.sort(npf1))
print(npf1)
npt=np.array(["mohamed","hossam","kareem","mona","Aaron"])
print(npt)
print(np.sort(npt))
npb=np.array([True,False,True,False])
print(npb)
print(np.sort(npb))
print(np.sort(npf4))#sort evry [] in it
s=np.where(npf1==2)#back the index
print(npf1)
print(s)
sr=np.where(npf1%2==0)#back the index
print(sr)
# filter
n=np.array([4,6,7,8])
b=np.array([True,False,True,False])
print(n[b])
f=[]
for t in n:
    if t%2==0:f.append(True)
    else:f.append(False)
print(n[f])
fr=n%2==1
print(n[fr])
