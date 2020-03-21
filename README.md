# DaydayUp
def dayUP(df):
    dayup = 1
    for i in range(365):
        if i % 4 in [0,1]:
            dayup = dayup * (1 - 0.01)
        else :
            dayup = dayup * (1 + dayfactor)
    return dayup
dayfactor = 0.01
while dayUP(dayfactor) < 37.78 :
    dayfactor += 0.001
print("工作日的努力参数应为{:.3f}".format(dayfactor))
