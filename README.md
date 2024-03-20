

def is_letter(char):

    if (ord('a') <= ord(char) <= ord('z')) or (ord('A') <= ord(char) <= ord('Z')):
        return True
    else:
        return False

def to_lowercase(char):
    if 'A' <= char <= 'Z':
        return chr(ord(char) + 32)  
    else:
        return char
def word_count(text):
    word_count = 0
    in_word = False

    for char in text:
        if char.isalnum(): 
            if not in_word:
                in_word = True
                word_count += 1
        else:  
            in_word = False

    return word_count

def ogr_bilgi():
 
    name = "Sude"
    surname = "Kara"
    student_id = "211213051"
    note = "Merhaba ben 3.sınıf bilgisayar mühendisliği öğrencisiyim."

    print("Ad:", name)
    print("Soyad:", surname)
    print("Öğrenci Numarası:", student_id)
    print("Not:", note)

ogr_bilgi()
