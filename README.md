# Arvore-recursiva

```python
def setup():
    size(500, 500)
 
def draw():
    background(99, 182, 196)
    translate(250, 300)
    galho(60)
    
def galho(tamanho):
    ang = radians(mouseX)
    encurtar = .8
    line(0, 0, 0, -tamanho)  
    if tamanho > 8:
        translate(0, -tamanho)
        rotate(ang)
        stroke(90, 216, 150)
        galho(tamanho * encurtar)  
        rotate(2 * -ang)
        stroke(110, 121, 119)
        galho(tamanho * encurtar) 
        rotate(ang)
        translate(0, tamanho)
```        
