# oop #abstact
abstarct
from abc import ABC, abstractmethod
class Sekil(ABC):
  @abstractmethod
  def Alan():
    pass
  @abstractmethod
  def Cevre():
    pass

class Ucgen(Sekil):
  def __init__(self,taban,yukseklik):
    self.taban=taban
    self.yukseklik=yukseklik

  def Alan(self):
    return self.taban*self.yukseklik/2
  def Cevre(self):
    return self.taban*3

class Kare(Sekil):
  def __init__(self,kenar):
    self.kenar=kenar

  def Alan(self):
    return self.kenar**2
  def Cevre(self):
    return self.kenar*4

a1=Ucgen(5,10)
a1.Alan()
a1.Cevre()

a2=Kare(10)
a2.Alan()
a2.Cevre()
