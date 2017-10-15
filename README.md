# busy-base-station
class Basestation():
  def _init_(self,ID,location,capacity):
     self.capacity=capacity
     self.ID=ID
     self.location=location
     self.busy=True

  def _str_(self):
    return "Basestation %s with %d capacity"%(self.capacity)

class Basestation1(Basestation):
  def _init_(self,ID):
    Basestation._init_(self,ID,location,90)
    self.busy=True

  def _str_(self):
    return Basestation._str_(self)+"is a busystation"

class Basestation2(Basestation):
  def _init_(self,ID):
    Basestation._init_(self,ID,location,20)
    self.busy=False

  def _str_(self):
    return Basestation._str_(self)+"is not a busystation"
