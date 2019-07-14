class doktor :
    def __init__(self, val = None):
        self.val = val
        self.next = None


class bulan_kerja:
    def __init__(self):
        self.main_value = None

    def bulan_libur(self, new_value):
        new_node = doktor(new_value)
        new_node .next = self.main_value
        self.main_value  = new_node

    def bulan_kumpul(self, new_value):
        new_node = doktor(new_value)
        last_node = self.main_value
        while last_node.next:
            last_node = last_node.next

        last_node.next = new_node

    def traverse(self):
        dataku = self.main_value
        while dataku is not None:
            print(dataku.val)
            dataku = dataku.next


myList = bulan_kerja()
myList.main_value = doktor("jun")

n2 = doktor("feb")
n3 = doktor("mar")
myList.main_value.next = n2
n2.next = n3

myList.bulan_libur(12)
myList.bulan_kumpul(17)

myList.traverse()