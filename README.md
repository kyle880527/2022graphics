# week03-1
```c++
#include <GL/glut.h>
void display()
{
    glClear(GL_COLOR_BUFFER_BIT | GL_DEPTH_BUFFER_BIT);
    glColor3f(1,1,0);///黃色
    glutSolidTeapot(0.3);///0.3實心茶壺
    glutSwapBuffers();///交換2倍的buffer
}
int main(int argc,char**argv)///進階的main函式
{
    glutInit(&argc, argv);///初始化
    glutInitDisplayMode( GLUT_DOUBLE | GLUT_DEPTH);///2倍+3D
    glutCreateWindow("week03的視窗");///建視窗
    glutDisplayFunc(display);///今天用來畫圖的函式
    glutMainLoop();///主要的迴圈
    return 0;
}

```
# week03-2
```c++
#include <GL/glut.h>
void display()
{
    glClear(GL_COLOR_BUFFER_BIT | GL_DEPTH_BUFFER_BIT);
    glColor3f(1,1,0);///黃色
    glBegin(GL_TRIANGLES);
        glColor3f(1.0f, 1.0f, 1.0f);    glVertex2f(0.0f,  0.5f);
        glColor3f(0.0f, 1.0f, 1.0f);    glVertex2f(0.87f,  -1.0f);
        glColor3f(0.0f, 0.0f, 1.0f);    glVertex2f(-0.87f,  1.0f);
    glEnd();
    glutSwapBuffers();///交換2倍的buffer
}
int main(int argc,char**argv)///進階的main函式
{
    glutInit(&argc, argv);///初始化
    glutInitDisplayMode( GLUT_DOUBLE | GLUT_DEPTH);///2倍+3D
    glutCreateWindow("week03的視窗");///建視窗
    glutDisplayFunc(display);///今天用來畫圖的函式
    glutMainLoop();///主要的迴圈
    return 0;
}

```
