# flattenlist
https://app.patika.dev/cucurcun
a = [[1,'a',['cat'],2],[[[3]],'dog'],4,5]

def flat_list(x):
    for item in x:
        if type(item) in [list]:
            for num in flat_list(item):
                yield (num)
        else:yield(item)
list(flat_list(a))
