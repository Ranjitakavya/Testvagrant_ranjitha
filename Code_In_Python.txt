import itertools
xl=int(input())
thisdict = {
  26:"TOI",
  20.5:"Hindu",
  34: "ET",
  10.5:"BM",
  16.4:"HT",
};
val=[26,20.5,34,10.5,16.4]
nsr=[]
combination=list(itertools.combinations(val, 2))
for i in combination:
    if sum(i)<=xl:
        nsr.append(i)

npp=[]
for i in range(len(nsr)):
        val1=nsr[i][0]
        val2=nsr[i][1]
        npp.append((thisdict[val1],thisdict[val2]))
print(npp)
