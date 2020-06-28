#MKDIR

def mkdir(path): 
    import os
    path = path.strip()
    path = path.rstrip("\\")
    isExist = os.path.exists(path)
    if not isExist:
        os.makedirs(path)
        print(path+'done')
        return True
    else:
        print(path+'already exist')
        return False
