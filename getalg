#coding:utf-8



def getMd5(content):
    f1= b'\x01\x23\x45\x67'
    f2= b'\x89\xab\xcd\xef'
    f3= b'\xfe\xdc\xba\x98'
    f4= b'\x76\x54\x32\x10'
    f5 = b'\x78\xa4\x6a\xd7'
    result = 0
    if f1 in content:
        result += 1
    if f2 in content:
        result += 1
    if f3 in content:
        result += 1
    if f4 in content:
        result += 1
    if f5 in content:
        result += 1
    
    return result
    


def getsha1(content):
    f1= b'\x99\x79\x82\x5a'
    f2= b'\xa1\xeb\xd9\x6e'
    f3= b'\xdc\xbc\x1b\x8f'
    f4= b'\xd6\xc1\x62\xca'
    result = 0
    if f1 in content:
        result += 1
    if f2 in content:
        result += 1
    if f3 in content:
        result += 1
    if f4 in content:
        result += 1
    
    return result    

def getsm3(content):
    f1= b'\x6f\x16\x80\x73'
    f2= b'\xb9\xb2\x14\x49'
    f3= b'\xd7\x42\x24\x17'
    f4= b'\x00\x06\x8a\xda' 
    result = 0
    if f1 in content:
        result += 1
    if f2 in content:
        result += 1
    if f3 in content:
        result += 1
    if f4 in content:
        result += 1
    
    return result    

def gettea(content):
    f1= b'\xb9\x79\x37\x9e'

    result = 0
    if f1 in content:
        result += 5

    
    return result    

def getbf(content):
    f1 = b'\xa6\x0b\x31\xd1'
    f2 = b'\xac\xb5\xdf\x98'
    f3 = b'\xdb\x72\xfd\x2f'
    f4 = b'\xb7\xdf\x1a\xd0'
    result = 0
    if f1 in content:
        result += 1
    if f2 in content:
        result += 1
    if f3 in content:
        result += 1
    if f4 in content:
        result += 1
        
    return result

def getcrc32(content):
    f1 = b'\x20\x83\xb8\xed'
    result = 0
    if f1 in content:
        result += 1  
        
    return result
def getBase64(content):
    import string
    f1 = string.ascii_uppercase+string.ascii_lowercase+string.digits+'+/'
    f1 = f1.encode()
    result = 0
    if f1 in content:
        result += 4  
        
    return result

def getBase58(content):
    import string
    f1 = '123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz'
    f1 = f1.encode()
    result = 0
    if f1 in content:
        result += 4  
        
    return result

def getBase32(content):
    import string
    f1 = string.ascii_uppercase+'234567'
    f1 = f1.encode()
    result = 0
    if f1 in content:
        result += 4  
        
    return result

def getBase24(content):
    import string
    f1 = b'BCDFGHJKMPQRTVWXYZ2346789'#Windows序列号的编码格式
    result = 0
    if f1 in content:
        result += 4  
        
    return result

def getBase60(content):
    import string
    f1 = string.digits+string.ascii_uppercase+string.ascii_lowercase[:-2]
    f1 = f1.encode()
    result = 0
    if f1 in content:
        result += 4  
        
    return result

def getrc5(content):
    f1 = b'\xe1\xb7'
    f2 = b'\x9e\x37'
    f3 = b'\x63\x51\xe1\xb7'
    f4 = b'\x6b\x2a\xed\x8a\x62\x51\xe1\xb7'
    result = 0
    if f1 in content:
        result += 1
    if f2 in content:
        result += 1
    if f3 in content:
        result += 1
    if f4 in content:
        result += 1
        
    return result


def getAlg(content):
    print('getMd5: ',getMd5(content))
    print('getsha1: ',getsha1(content))
    print('getsm3: ',getsm3(content))
    print('gettea: ',gettea(content))
    print('getbf: ',getbf(content))
    print('getcrc32: ',getcrc32(content))
    print('getBase64: ',getBase64(content))
    print('getBase58: ',getBase58(content))
    print('getBase32: ',getBase32(content))
    print('getBase24: ',getBase24(content))
    print('getBase60: ',getBase60(content))
    print('getrc5: ',getrc5(content))
    return

if __name__ == '__main__':
    
    import sys
    file = sys.argv[1]
    with open(file, 'rb') as f:
        
        getAlg(f.read())
    

    
