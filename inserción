float Caja[] = new float [10];
float a, aux;
int j, p;

void setup(){
  begin();
  fullScreen(P3D);
}

void draw(){
p++;
  if((p+1)>=Caja.length) noLoop();
  aux=Caja[p];
  j = p-1;
  while((j>=0) && (aux<Caja[j])){
    Caja[j+1] = Caja[j];
    j--;
  }
  Caja[j+1] = aux;
  show();
}

void show(){
    background(0);
    for(int i = 0; i < Caja.length; i++){
    pushMatrix();
    beginShape(BOX);
    strokeWeight(3);
    stroke(255);
    fill(random(255), random(255), random(255));
    translate(map(i, 0, Caja.length, width/Caja.length, width), height/2);
    rotateX(a);
    rectMode(CENTER);
    box(Caja[i]);


    endShape();
    popMatrix();
    delay(100);
    
    a=+1;
  
  }

}
void mousePressed(){
  if(mousePressed==true);{
      show();
    }}
    
void begin(){
  for(int i = 0; i < Caja.length; i++){
    Caja[i]=random(75);
  }
  
}
