#include<iostream.h>
#include<conio.h>
#include<fstream.h>
#include<string.h>
#include<process.h>
#include<dos.h>
#include<stdio.h>
#include<stdlib.h>
#include<time.h>



int c, d, cord[90][30], feed[20], bd=0, mv, mx=3, gre=0, ctra=281;
char Q[50], fl;
ofstream SaveFiles;
ifstream ReadSaveFiles;

//    **********************************JUKE_BOX*****************************

void J_BOX(freq)
{ sound(freq); delay(50); nosound();  }
void RAIN(int x, int ctr)
{
	int y;
	for (y=20; y>1; y--)
	{ gotoxy(x,y); textcolor(2); cprintf("%c",char(219)); delay(2); }

	if (ctr==1)
	{
		for (y=2; y<21; y++)
		{ gotoxy(x,y); textcolor(3); cprintf("%c",char(219)); delay(2); }
	}
	else if (ctr==2)
	{
		for (y=2; y<21; y++)
		{ gotoxy(x,y); textcolor(4); cprintf("%c",char(219)); delay(2); }
	}
	else if (ctr==3)
	{
		for (y=2; y<21; y++)
		{ gotoxy(x,y); textcolor(5); cprintf("%c",char(219)); delay(2); }
	}
	else if (ctr==4)
	{
		for (y=2; y<21; y++)
		{ gotoxy(x,y); textcolor(6); cprintf("%c",char(219)); delay(2); }
	}
	else if (ctr==5)
	{
		for (y=2; y<21; y++)
		{ gotoxy(x,y); textcolor(7); cprintf("%c",char(219)); delay(2); }
	}
	else if (ctr==6)
	{
		for (y=2; y<21; y++)
		{ gotoxy(x,y); textcolor(1); cprintf("%c",char(219)); delay(2); }
	}
	else if (ctr==7)
	{
		for (y=2; y<21; y++)
		{ gotoxy(x,y); textcolor(10); cprintf("%c",char(219)); delay(2); }
	}
	else if (ctr==8)
	{
		for (y=2; y<21; y++)
		{ gotoxy(x,y); textcolor(11); cprintf("%c",char(219)); delay(2); }
	}
	else if (ctr==9)
	{
		for (y=2; y<21; y++)
		{ gotoxy(x,y); textcolor(12); cprintf("%c",char(219)); delay(2); }
	}
	else if (ctr==10)
	{
		for (y=2; y<21; y++)
		{ gotoxy(x,y); textcolor(14); cprintf("%c",char(219)); delay(2); }
	}
	else if (ctr==11)
	{
		for (y=2; y<21; y++)
		{ gotoxy(x,y); textcolor(15); cprintf("%c",char(219)); delay(2); }
	}
	else if (ctr==12)
	{
		for (y=2; y<21; y++)
		{ gotoxy(x,y); textcolor(4); cprintf("%c",char(219)); delay(2); }
	}
	else if (ctr==13)
	{
		for (y=2; y<21; y++)
		{ gotoxy(x,y); textcolor(13); cprintf("%c",char(219)); delay(2); }
	}
	else if (ctr==14)
	{
		for (y=2; y<21; y++)
		{ gotoxy(x,y); textcolor(2); cprintf("%c",char(219)); delay(2); }
	}
	else if (ctr==15)
	{
		for (y=2; y<21; y++)
		{ gotoxy(x,y); textcolor(1); cprintf("%c",char(219)); delay(2); }
	}
	else if (ctr==16)
	{
		for (y=2; y<21; y++)
		{ gotoxy(x,y); textcolor(11); cprintf("%c",char(219)); delay(2); }
	}
}


void M_BOX(int &ctrm)
{

	if (ctrm==1) 	   { J_BOX(100);   RAIN(14,ctrm); }
	else if (ctrm==8)  { J_BOX(120);   RAIN(18,ctrm); }
	else if (ctrm==5)  { J_BOX(140);   RAIN(22,ctrm); }
	else if (ctrm==2)  { J_BOX(160);   RAIN(26,ctrm); }
	else if (ctrm==10)  { J_BOX(180);  RAIN(30,ctrm); ctra=0; ctrm=1; }

	else if (ctrm==9)  { J_BOX(680);   RAIN(70,ctrm); }
	else if (ctrm==4)  { J_BOX(660);   RAIN(66,ctrm); }
	else if (ctrm==3)  { J_BOX(640);   RAIN(62,ctrm); }
	else if (ctrm==7)  { J_BOX(620);   RAIN(58,ctrm); }
	else if (ctrm==6)  { J_BOX(600);   RAIN(54,ctrm); }

	ctrm++;
}

//   /*
void JUTE_BOX()
{
clrscr();

	char stk;
	gotoxy(14,21);
	cout<<"q w e r t y u i o p a s d f g h j k l ; z x c v b n m , . ";
	while (1)
	{
		if (kbhit())
		{
			stk=getch();
			if (stk=='q') 	   { J_BOX(100);   RAIN(14,1); }
			else if (stk=='w') { J_BOX(120);   RAIN(16,2); }
			else if (stk=='e') { J_BOX(140);   RAIN(18,3); }
			else if (stk=='r') { J_BOX(160);   RAIN(20,4); }
			else if (stk=='t') { J_BOX(180);   RAIN(22,5); }
			else if (stk=='y') { J_BOX(200);   RAIN(24,6); }
			else if (stk=='u') { J_BOX(220);   RAIN(26,7); }
			else if (stk=='i') { J_BOX(240);   RAIN(28,8); }
			else if (stk=='o') { J_BOX(260);   RAIN(30,9); }
			else if (stk=='p') { J_BOX(280);   RAIN(32,10); }
			else if (stk=='a') { J_BOX(300);   RAIN(34,11); }
			else if (stk=='s') { J_BOX(320);   RAIN(36,12); }
			else if (stk=='d') { J_BOX(340);   RAIN(38,13); }
			else if (stk=='f') { J_BOX(360);   RAIN(40,14); }
			else if (stk=='g') { J_BOX(380);   RAIN(42,15); }
			else if (stk=='h') { J_BOX(400);   RAIN(44,16); }
			else if (stk=='j') { J_BOX(420);   RAIN(46,1); }
			else if (stk=='k') { J_BOX(440);   RAIN(48,2); }
			else if (stk=='l') { J_BOX(480);   RAIN(50,4); }
			else if (stk==';') { J_BOX(500);   RAIN(52,11); }
			else if (stk=='z') { J_BOX(520);   RAIN(54,9); }
			else if (stk=='x') { J_BOX(540);   RAIN(56,14); }
			else if (stk=='c') { J_BOX(560);   RAIN(58,5); }
			else if (stk=='v') { J_BOX(580);   RAIN(60,6); }
			else if (stk=='b') { J_BOX(600);   RAIN(62,7); }
			else if (stk=='n') { J_BOX(620);   RAIN(64,12); }
			else if (stk=='m') { J_BOX(640);   RAIN(66,13); }
			else if (stk==',') { J_BOX(660);   RAIN(68,15); }
			else if (stk=='.') { J_BOX(680);   RAIN(70,3); }
			else if (stk=='/') exit(0);
		}
	}

getch();
}
//	  */

//   ***************************************************************************

int lvl;

class GAME_DATA
{
   private:
	char name[60];
   public:
	int sl, score, level, coast;
	int Sylvia, Buna, Nathan, Alexis;
	GAME_DATA()	{ Sylvia=0;	Buna=0; Nathan=0; Alexis=0;	coast=0; }
	char *Show_Name()	{	return name;	}
	void Get_Name()     {   cout<<"\nEnter Name: "; gets(name);  }
	void Scr_Add_Ten()	{	score+=10; 	}
	void Scr_Add_Five()	{   score+=5;   }
	void Scr_Sub_Five() {   score-=5;   }
	void Scr_Sub_Ten()  {   score-=10;  }
	void LevelUp()		{	level++;	}
	void Activate_Sylvia()	{	Sylvia=10;	}
	void Activate_Buna()	{	Buna=10;	}
	void Activate_Nathan()	{	Nathan=10;	}
	void Activate_Alexis()	{	Alexis=10;	}
	void Deactivate_Sylvia()	{	Sylvia=0;	}
	void Deactivate_Buna()		{	Buna=0;		}
	void Deactivate_Nathan()	{	Nathan=0;	}
	void Deactivate_Alexis()	{	Alexis=0;	}
	void Plus_Sylvia()	{	Sylvia++;	}
	void Plus_Buna()	{	Buna++;		}
	void Plus_Nathan()	{	Nathan++;	}
	void Plus_Alexis()	{	Alexis++;	}
	void Min_Sylvia()	{	Sylvia--;	}
	void Min_Buna()		{	Buna--;		}
	void Min_Nathan()	{	Nathan--;	}
	void Min_Alexis()	{	Alexis--;	}
	int Silo()			{	return sl;	}
	void Show()
	{
		if      (level==1||level==2||level==3||level==5||level==9||level==10) lvl=1;
		else if (level==6||level==7||level==17||level==18||level==8||level==11||level==12||level==13) lvl=2;
		else if (level==14||level==15||level==16||level==21||level==19||level==20) lvl=3;
		cout<<'\n'<<sl<<'.'<<name<<"\nSCORE: "<<score<<"\tLEVEL: "<<lvl<<"\n";
		cout<<"Sylvia: "<<Sylvia<<"\tBuna: "<<Buna<<"\nNathan: "<<Nathan<<"\tAlexis: "<<Alexis;
		getch();
	}
} GM;

void Update()
{
	int iii=1;
	ReadSaveFiles.open("SAVDAT", ios::in | ios::binary);
	SaveFiles.open("SAVDAT", ios::ate | ios::binary);
	char *nm=GM.Show_Name();
	GAME_DATA _GM;
		ReadSaveFiles.seekg(0);
		while(!ReadSaveFiles.eof())
		{
			int location=ReadSaveFiles.tellg();
			ReadSaveFiles.read((char*)&_GM, sizeof(_GM));
			if (strcmpi(_GM.Show_Name(),nm)==0)
			{
				SaveFiles.seekp(location);
				SaveFiles.write((char*)&GM, sizeof(GM));
				break;
			}
		}
		ReadSaveFiles.close();
		SaveFiles.close();
}

void Delayer(char *str)
{
	int ctrd=0;
	int len=strlen(str);
	for (d=0; d<len; d++)
	{
		textcolor(WHITE); printf("%c",str[d]);
		if (ctrd%12==0)      { sound(600); delay(16); nosound(); }
		else if (ctrd%12==1) delay(16);
		else if (ctrd%12==2) delay(16);
		else if (ctrd%12==3) { sound(400); delay(16); nosound(); }
		else if (ctrd%12==4) delay(16);
		else if (ctrd%12==5) delay(16);
		else if (ctrd%12==6) { sound(200); delay(16); nosound(); }
		else if (ctrd%12==7) delay(16);
		else if (ctrd%12==8) delay(16);
		else if (ctrd%12==9) { sound(400); delay(16); nosound(); }
		else if (ctrd%12==10) delay(16);
		else if (ctrd%12==11) delay(16);
		ctrd++;
	}
}
void Clr_Lower()
{ for (c=1; c<81; c++) for (d=22; d<24; d++) { gotoxy(c,d); textcolor(15); printf("%c",' '); } }

void Clr_Lower_()
{ for (c=1; c<81; c++) for (d=13; d<25; d++) { gotoxy(c,d); textcolor(15); printf("%c",' '); } }

// ****************************PRINCESS_HEATHER**************************

int land[80][23], x=0, y=0, xp, yp, yg, stp=0, xe[100], ye[100], atk=0;
int lz=1, gm_over=0, prin=0, fails=0;

void LAV_DEATH()
{ gotoxy(4,22); textcolor(4); cprintf("%s","BURNT TO ASHES !!"); getch(); }

void SPLASH_DEATH()
{ gotoxy(4,22); textcolor(11); cprintf("%s","SPLASH !!"); getch(); }

void TREE(int xl, int yl)
{ gotoxy(xl,yl); textcolor(2); cprintf("%c",char(219)); land[xl][yl]=2; }

void WATER(int xl, int yl)
{ gotoxy(xl,yl); textcolor(1); cprintf("%c",char(219)); land[xl][yl]=3; }

void LAND(int xl, int yl)
{ gotoxy(xl,yl); textcolor(10); cprintf("%c",char(219)); land[xl][yl]=1; }

void LAND_(int xl, int yl)
{ gotoxy(xl,yl); textcolor(2); cprintf("%c",char(219)); land[xl][yl]=1; }

void SPACE(int xl, int yl)
{ gotoxy(xl,yl); textcolor(16); cprintf("%c",char(219)); land[xl][yl]=0; }

void LAVA(int xl, int yl)
{ gotoxy(xl,yl); textcolor(4); cprintf("%c",char(219)); land[xl][yl]=4; }

void BOLD(int xl, int yl)
{ gotoxy(xl,yl); textcolor(8); cprintf("%c",char(219)); land[xl][yl]=2; }

void KB(int xl, int yl)
{ gotoxy(xl,yl); textcolor(3); cprintf("%c",char(219)); land[xl][yl]=1; delay(40); }

void ME(int xl, int yl)
{ gotoxy(xl,yl); textcolor(BROWN); cprintf("%c",char(2)); }

void SL(int xl, int yl)
{ gotoxy(xl,yl); textcolor(14); cprintf("%c",char(2)); }

void AL(int xl, int yl)
{ gotoxy(xl,yl); textcolor(11); cprintf("%c",char(2)); }

void PE(int xl, int yl)
{ gotoxy(xl,yl); textcolor(11); cprintf("%c",char(15)); land[xl][yl]=5; delay(40); }

void EE(int xl, int yl)
{ gotoxy(xl,yl); textcolor(15); cprintf("%c",char(1));  land[xl][yl]=5; }

void BE(int xl, int yl)
{ gotoxy(xl,yl); textcolor(BROWN); cprintf("%c",char(5));  land[xl][yl]=5; }

void LE(int xl, int yl)
{ gotoxy(xl,yl); textcolor(4); cprintf("%c",char(219));  land[xl][yl]=4; }

void LAZER_1()
{ for (x=62; x<77; x++) LE(x,9); }
void LAZER_2()
{ for (x=76; x>61; x--) LAND(x,9); }
void LAZER_3()
{ for (x=62; x<77; x++) LE(x,7); }
void LAZER_4()
{ for (x=76; x>61; x--) LAND(x,7); }

//   /*
void LANDSCAPE()
{

	//	1st tree lane
	for (yg=2; yg<16; yg++)
	{ gotoxy(23,yg); textcolor(2); land[23][yg]=2; cprintf("%c",char(219)); }

	//	left bottom trees
	for (x=3; x<11; x++) TREE(x,21);
	for (x=3; x<9; x++)  TREE(x,20);
	for (x=3; x<7; x++) { TREE(x,19); TREE(x,18); }
	for (x=3; x<6; x++)  TREE(x,17);
	for (x=3; x<5; x++)  TREE(x,16);
	for (x=3; x<3; x++)  TREE(x,15);
	for (x=3; x<2; x++)  TREE(x,14);

	//  Bottom-Lake
	for (x=20; x<61; x++) WATER(x,21);
	for (x=24; x<52; x++) WATER(x,20);
	for (x=30; x<48; x++) WATER(x,19);
	for (x=33; x<44; x++) WATER(x,18);
	for (x=36; x<41; x++) WATER(x,17);
	for (x=38; x<40; x++) WATER(x,16);

	//  Battle-field Right Tree-Lane
	for (y=2; y<13; y++) TREE(30,y); TREE(29,13); TREE(28,14);

	//  Mid-screen Upper Tree-Lane  & portrusion
	for (x=31; x<54; x++) TREE(x,2);
	for (x=51; x<54; x++) TREE(x,3);
	for (x=53; x<54; x++) TREE(x,4);
	for (x=40; x<51; x++) TREE(x,3);

	//  Mid-screen Boulders
	for (y=5; y<18; y++) BOLD(38,y);

	//  Lava-touching Boulders
	for (y=5; y<15; y++) BOLD(53,y);

	//  Lava-Traps
	for (x=52; x>40; x--) LAVA(x,5); LAND(38,5);
	for (x=39; x<52; x++) LAVA(x,7);
	for (x=52; x>39; x--) LAVA(x,9);
	for (x=39; x<52; x++) LAVA(x,11);
	for (x=52; x>39; x--) LAND(x,4);

	//  Lava-Lake
	for (x=43; x<56; x++) LAVA(x,15);
	for (x=45; x<58; x++) LAVA(x,16);
	for (x=45; x<60; x++) LAVA(x,17);
	for (x=49; x<57; x++) LAVA(x,18);
	LAVA(55,13); LAVA(55,14); LAVA(54,14);

	//  Upper-Lake
	for (x=54; x<71; x++) WATER(x,2);
	for (x=54; x<69; x++) WATER(x,3);
	for (x=54; x<62; x++) WATER(x,4);
	for (x=54; x<58; x++) WATER(x,5);
	for (x=54; x<56; x++) WATER(x,6); WATER(54,7);

	// Hori-Boulders
	for (x=60; x<74; x++) BOLD(x,17); BOLD(69,18); BOLD(69,19); BOLD(69,20);

	//  top-House Tree-Lane
	for (y=7; y<10; y++)  TREE(60,y);
	for (y=7; y<10; y++)  TREE(61,y);
	for (x=60; x<74; x++) TREE(x,6);

	//  Lower-Right Enemies
	BE(69,21);  BE(71,21);  BE(74,21);  BE(76,21);  BE(70,20);  BE(72,20);
	BE(74,20);  BE(75,20);  BE(70,19);  BE(71,19);  BE(73,19);  BE(76,19);
	BE(70,18);  BE(72,18);  BE(74,18);  BE(76,18);  BE(73,17);  BE(76,17);

	//  Right-Mid Weed
	for (x=59; x>53; x--)
	{ gotoxy(x,9); textcolor(8); land[x][9]=5; cprintf("%c",char(1)); }

}
//   */

//   /*
void HOUSE()
{
	for (x=60; x<74; x++)
	{
		gotoxy(x,10); textcolor(16); land[x][10]=2;
		cprintf("%c",char(219));
		gotoxy(x,15); textcolor(16); land[x][15]=2;
		cprintf("%c",char(219));
	}
	gotoxy(74,15); textcolor(16); land[74][15]=2; cprintf("%c",char(219));
	gotoxy(75,15); textcolor(16); land[75][15]=2; cprintf("%c",char(219));
	gotoxy(76,15); textcolor(16); land[76][15]=2; cprintf("%c",char(219));
	for (int yy=11; yy<15; yy++)
	{
		gotoxy(60,yy); textcolor(16); land[60][yy]=2;
		cprintf("%c",char(219));
		gotoxy(61,yy); textcolor(16); land[61][yy]=2;
		cprintf("%c",char(219));
	}
	for (y=11; y<15; y++)
	{ gotoxy(66,y); textcolor(8); land[66][y]=2; cprintf("%c",char(219)); }
	gotoxy(66,13); textcolor(6); land[66][13]=5; cprintf("%c",char(219));
	gotoxy(67,13); textcolor(4); land[67][13]=5; cprintf("%c",char(1));
	gotoxy(64,12); textcolor(5); land[64][12]=2; cprintf("%c",char(2));
}
//   */


void MAP__()
{
	clrscr();
	for (x=3; x<77; x++)
	{ for (y=2; y<22; y++) { gotoxy(x,y); cout<<land[x][y]; } }
}


void UP(int a, int &xc, int &yc)
{
  if (a==1)
  {
	if (land[xc][yc-1]==1) { yc--; LAND(xc,yc+1); ME(xc,yc); }
	else if (land[xc][yc-1]==4||land[xc][yc]==4) { LAV_DEATH(); gm_over=1; }
	else if (land[xc][yc-1]==3||land[xc][yc]==3) { SPLASH_DEATH(); gm_over=1; }
  }
  else if (a==3)
  { if (land[xc][yc-1]==1) { yc--; LAND(xc,yc+1); AL(xc,yc); } }
  else if (a==5)
  { if (land[xc][yc-1]==1) { yc--; LAND(xc,yc+1); SL(xc,yc); } }
  else if (a==7)
  { if (land[xc][yc-1]==0) { yc--; SPACE(xc,yc+1); PE(xc,yc); } }
  else
  {
	if (land[xc][yc]==3||land[xc][yc]==2||land[xc][yc]==4) stp=1;
	else if (land[xc][yc-1]==1) { yc--; LAND(xc,yc+1); land[xc][yc+1]=1; PE(xc,yc); }
	else if (land[xc][yc-1]==3||land[xc][yc-1]==2||land[xc][yc-1]==4) { LAND(xc,yc); stp=1; }
	else if (land[xc][yc-1]==5) { yc--; LAND(xc,yc+1); KB(xc,yc); delay(40); LAND(xc,yc); stp=1; }
  }
}

void DOWN(int a, int &xc, int &yc)
{
  if (a==1)
  {
	if (land[xc][yc+1]==1) { yc++; LAND(xc,yc-1); ME(xc,yc); }
	else if (land[xc][yc+1]==4||land[xc][yc]==4) { LAV_DEATH(); gm_over=1; }
	else if (land[xc][yc+1]==3||land[xc][yc]==3) { SPLASH_DEATH(); gm_over=1; }
  }
  else if (a==3)
  { if (land[xc][yc+1]==1) { yc++; LAND(xc,yc-1); AL(xc,yc); } }
  else if (a==5)
  { if (land[xc][yc+1]==1) { yc++; LAND(xc,yc-1); SL(xc,yc); } }
  else
  {
	if (land[xc][yc]==3||land[xc][yc]==2||land[xc][yc]==4) stp=1;
	else if (land[xc][yc+1]==1) { yc++; LAND(xc,yc-1); land[xc][yc-1]=1; PE(xc,yc); }
	else if (land[xc][yc+1]==3||land[xc][yc+1]==2||land[xc][yc+1]==4) { LAND(xc,yc); stp=1; }
	else if (land[xc][yc+1]==5) { yc++;  LAND(xc,yc-1); KB(xc,yc); delay(40); LAND(xc,yc); stp=1; }
  }
}
void LEFT(int a, int &xc, int &yc)
{
  if (a==1)
  {
	if (land[xc-1][yc]==1) { xc--; LAND(xc+1,yc); ME(xc,yc); }
	else if (land[xc-1][yc]==4||land[xc][yc]==4) { LAV_DEATH(); gm_over=1; }
	else if (land[xc-1][yc]==3||land[xc][yc]==3) { SPLASH_DEATH(); gm_over=1; }
  }
  else if (a==6)
  { if (land[xc-1][yc]==0) { xc--; SPACE(xc+1,yc); ME(xc,yc); } }
  else if (a==3)
  { if (land[xc-1][yc]==1) { xc--; LAND(xc+1,yc); AL(xc,yc); } }
  else if (a==5)
  { if (land[xc-1][yc]==1) { xc--; LAND(xc+1,yc); SL(xc,yc); } }
  else
  {
	if (land[xc][yc]==3||land[xc][yc]==2||land[xc][yc]==4) stp=1;
	else if (land[xc-1][yc]==1) { xc--; LAND(xc+1,yc); land[xc+1][yc]=1; PE(xc,yc); }
	else if (land[xc-1][yc]==3||land[xc-1][yc]==2||land[xc-1][yc]==4) { LAND(xc,yc); stp=1; }
	else if (land[xc-1][yc]==5) { xc--; LAND(xc+1,yc); KB(xc,yc); delay(40); LAND(xc,yc); stp=1; }
  }
}
void RIGHT(int a, int &xc, int &yc)
{
  if (a==1)
  {
	if (land[xc+1][yc]==1) { xc++; LAND(xc-1,yc); ME(xc,yc); }
	else if (land[xc+1][yc]==4||land[xc][yc]==4) { LAV_DEATH(); gm_over=1; }
	else if (land[xc+1][yc]==3||land[xc][yc]==3) { SPLASH_DEATH(); gm_over=1; }
  }
  else if (a==6)
  { if (land[xc+1][yc]==0) { xc++; SPACE(xc-1,yc); ME(xc,yc); } }
  else if (a==3)
  { if (land[xc+1][yc]==1) { xc++; LAND(xc-1,yc); AL(xc,yc); } }
  else if (a==5)
  { if (land[xc+1][yc]==1) { xc++; LAND(xc-1,yc); SL(xc,yc); } }
  else
  {
	if (land[xc][yc]==3||land[xc][yc]==2||land[xc][yc]==4) stp=1;
	else if (land[xc+1][yc]==1) { xc++; LAND(xc-1,yc); PE(xc,yc); }
	else if (land[xc+1][yc]==3||land[xc+1][yc]==2||land[xc+1][yc]==4) { LAND(xc,yc); stp=1; }
	else if (land[xc+1][yc]==5) { xc++; LAND(xc-1,yc); KB(xc,yc); LAND(xc,yc);  stp=1; }
  }
}


int Princess_Heather()
{
clrscr();

	for (int i1=1; i1<81; i1++)     land[i1][1]=2;
	for (int i2=2; i2<80; i2++)  	land[i2][22]=2;
	for (int j1=2; j1<23; j1++)     land[2][j1]=2;
	for (int j2=2; j2<23; j2++)  	land[77][j2]=2;
	for (y=2; y<22; y++)	for (x=3; x<77; x++)	LAND(x,y);
	gotoxy(12,8); textcolor(3); cprintf("%c",char(2)); land[12][8]=2;
	gotoxy(3,4); textcolor(9); cprintf("%c",char(2));  land[3][4]=2;
	gotoxy(4,3); textcolor(14); cprintf("%c",char(2)); land[4][3]=2;
	gotoxy(7,3); textcolor(9); cprintf("%c",char(2));  land[7][3]=2;
	gotoxy(6,4); textcolor(9); cprintf("%c",char(2));  land[6][4]=2;
	gotoxy(3,3); textcolor(14); cprintf("%c",char(2)); land[3][3]=2;
	gotoxy(3,2); textcolor(9); cprintf("%c",char(2));  land[3][2]=2;
	gotoxy(5,2); textcolor(14); cprintf("%c",char(2)); land[5][2]=2;
	gotoxy(7,2); textcolor(9); cprintf("%c",char(2));  land[7][2]=2;
	gotoxy(7,4); textcolor(14); cprintf("%c",char(2)); land[7][4]=2;
	ME(13,9);
	LANDSCAPE();
	HOUSE();

	Clr_Lower();
	gotoxy(1,22);
	Delayer("NATHAN: You seem to have a knack for Frost Spells, I want you to use them now.\n");
	Delayer("( Press 'i', 'j', 'k', 'l', to release Frost_Balls. ");
  Frost_Test:
	xp=13, yp=9;
	char mov_=getch();
	if (mov_=='i')
	{  yp--; while(stp==0) UP(2,xp,yp);  }
	else if (mov_=='j')
	{  xp--; while(stp==0) LEFT(2,xp,yp); }
	else if (mov_=='k')
	{  yp++; while(stp==0) DOWN(2,xp,yp); }
	else if (mov_=='l')
	{  xp++; while(stp==0) RIGHT(2,xp,yp); }
	else goto Frost_Test;
	Clr_Lower();
	gotoxy(1,22);
	Delayer("NATHAN: Your Frost_Balls seem Strong, They'll come in hand when you need to\n");
	Delayer("        Break through obstacles. Use it wisely. Now here's what you need to do");
	getch();
	Clr_Lower();
	gotoxy(1,22);
	Delayer("NATHAN: You need to go through that narrow path between the trees. You'll\n");
	Delayer("        Come across a bunch of traps, be clever.");
	getch();
	Clr_Lower();
	gotoxy(1,22);
	Delayer("NATHAN: You'll then see a house. Our Zork Princess, Princess Heather has\n");
	Delayer("        been kidnapped by these Quazarks. Wipe them out and rescue her!");
	getch();
	Clr_Lower();
	gotoxy(1,22);
	Delayer("YOU   : That seems like a good workout....Yea OK. I'll try my best.....\n");
	getch();
	Delayer("NATHAN: BEST OF LUCK.... Watch out for Lava traps and Frozen Water !!");
	getch();

  BEG:
	clrscr();
	for (x=3; x<77; x++) for (y=2; y<22; y++) LAND(x,y);
	for (int i3=1; i3<81; i3++)     land[i3][1]=2;
	for (int i4=2; i4<80; i4++)  	land[i4][22]=2;
	for (int j3=2; j3<23; j3++)     land[2][j3]=2;
	for (int j4=2; j4<23; j4++)  	land[77][j4]=2;

	int xc=13, yc=9;
	for (y=2; y<22; y++)	for (x=3; x<77; x++)	LAND(x,y);
	char mov;
	ME(xc,yc);
	LANDSCAPE();
	HOUSE();
	gotoxy(12,8); textcolor(3); cprintf("%c",char(2)); land[12][8]=2;
	gotoxy(3,4); textcolor(9); cprintf("%c",char(2));  land[3][4]=2;
	gotoxy(4,3); textcolor(14); cprintf("%c",char(2)); land[4][3]=2;
	gotoxy(7,3); textcolor(9); cprintf("%c",char(2));  land[7][3]=2;
	gotoxy(6,4); textcolor(9); cprintf("%c",char(2));  land[6][4]=2;
	gotoxy(3,3); textcolor(14); cprintf("%c",char(2)); land[3][3]=2;
	gotoxy(3,2); textcolor(9); cprintf("%c",char(2));  land[3][2]=2;
	gotoxy(5,2); textcolor(14); cprintf("%c",char(2)); land[5][2]=2;
	gotoxy(7,2); textcolor(9); cprintf("%c",char(2));  land[7][2]=2;
	gotoxy(7,4); textcolor(14); cprintf("%c",char(2)); land[7][4]=2;
	while (gm_over!=1)
	{
		stp=0;
		xp=xc; yp=yc;
		for (x=40; x<51; x++) land[x][3]=-1;
		if (kbhit())
		{
			if(lz%2==0) LAZER_1();
			if(lz%4==0) LAZER_3();
			if(lz%2!=0) LAZER_2();
			if(lz%4!=0) LAZER_4();
			lz++;
			mov=getch();
			if (mov=='w')
				UP(1,xc,yc);
			else if (mov=='a')
				LEFT(1,xc,yc);
			else if (mov=='s')
				DOWN(1,xc,yc);
			else if (mov=='d')
				RIGHT(1,xc,yc);
			else if (mov=='/')
				exit(0);
			else if (mov==']')
				MAP__();
			else if (mov=='[') { LANDSCAPE(); HOUSE(); }
			else if (mov=='m')
			{	LAND(xc,yc); xc=65; yc=19;	}
			if (mov=='i')
			{  yp--; while(stp==0) UP(2,xp,yp);  }
			else if (mov=='j')
			{  xp--; while(stp==0) LEFT(2,xp,yp); }
			else if (mov=='k')
			{  yp++; while(stp==0) DOWN(2,xp,yp); }
			else if (mov=='l')
			{  xp++; while(stp==0) RIGHT(2,xp,yp); }
		}
		if (xc==64 && yc==13) { prin=1; gm_over=1; }
	}
	if (prin==0)
	{
		clrscr(); cout<<"YOU COULDN'T SAVE THE PRINCESS.....TRY AGAIN !!";
		getch(); gm_over=0; fails++;
		goto BEG;
	}
	else
	{
		clrscr(); cout<<"CONGRATS!!"; getch();
		for (int xx=1; xx<81; xx++) for (int yy=1; yy<24; yy++) land[xx][yy]=0;
		return fails;
	}

getch();
}

// ***********************************************************************


// *******************************ORNLU*********************************

void FORREST()
{
clrscr();

	for (x=11; x<70; x++) for (y=4; y<12; y++) { LAND(x,y); delay(5); }

	for (x=10; x<71; x++) { TREE(x,3);  delay(5); }
	for (x=10; x<71; x++) { TREE(x,12); delay(5); }
	for (y=3; y<12; y++)  { TREE(10,y); delay(5); }
	for (y=3; y<12; y++)  { TREE(70,y); delay(5); }

	for (x=27; x<70; x++) { TREE(x,4);  delay(5); }
	for (x=28; x<70; x++) { TREE(x,5);  delay(5); }
	for (x=29; x<70; x++) { TREE(x,6);  delay(5); }
	for (x=30; x<70; x++) { TREE(x,7);  delay(5); }
	for (x=31; x<70; x++) { TREE(x,8);  delay(5); }

	for (x=11; x<21; x++) { TREE(x,6);  delay(5); }
	for (x=11; x<22; x++) { TREE(x,7);  delay(5); }
	for (x=11; x<23; x++) { TREE(x,8);  delay(5); }

	for (x=50; x<61; x++) { LAND(x,9);  delay(5); }
	for (x=51; x<62; x++) { LAND(x,8);  delay(5); }
	for (x=52; x<63; x++) { LAND(x,7);  delay(5); }
	for (x=53; x<64; x++) { LAND(x,6);  delay(5); }
	for (x=55; x<71; x++) { LAND(x,5);  delay(5); }

}

void ORNLU()
{
clrscr();

	int ctry=1;
	FORREST();
	int xm=23, xa=12, ym=5, ya=10, ctrx=0;
	ME(xm,ym); AL(xa,ya);
	for (int h=0; h<11; h++)
	{
		if (ym!=10)
		{
			if (ctrx%2==0) { DOWN(1,xm,ym);  ctrx++; delay(150); }
			else           { RIGHT(1,xm,ym); ctrx++; delay(150); }
		}
		RIGHT(3,xa,ya); delay(150);
	}
	RIGHT(3,xa,ya); delay(150);
	GM.Activate_Alexis();

	Clr_Lower_();
	gotoxy(1,13);
	Delayer("	     (You reach for your dagger.....) \n");
	Delayer("ALEXIS: First time in this tournament, huh? Seems to me you must be on your \n");
	RIGHT(3,xa,ya); RIGHT(1,xm,ym); gotoxy(1,15);
	Delayer("        toes all this while, now that you are in a very remote, homesick \n");
	Delayer("        part of this vast continent. Yea, This forrest does bring out the\n");
	RIGHT(3,xa,ya); RIGHT(1,xm,ym); gotoxy(1,17);
	Delayer("        creeps......\n");
	Delayer("YOU   : You talk a lot for a stranger, all others I've met on my way either\n");
	RIGHT(3,xa,ya); RIGHT(1,xm,ym); gotoxy(1,19);
	Delayer("        gave no attention, or gave the killer-eye looks.\n");
	Delayer("ALEXIS: Thats whats special about this tournament, no one's a friend till \n");
	RIGHT(3,xa,ya); RIGHT(1,xm,ym); gotoxy(1,21);
	Delayer("        you actually do something about it. And that ain't easy either...\n");
	Delayer("        I mean, even I can be the betrayer sort, you don't know.....\n");
	RIGHT(3,xa,ya); RIGHT(1,xm,ym);
	fl=getch();
	if (fl=='/') exit(0);

	Clr_Lower_();
	gotoxy(1,13);
	Delayer("YOU   : This forrest, why Ornlu, why not Green-Pine, I mean there are a lot \n");
	Delayer("        of Green-Pines down here..... \n");
	RIGHT(3,xa,ya); RIGHT(1,xm,ym); gotoxy(1,15);
	Delayer("ALEXIS: It is said that the great Wolf Ornlu once used to live here. They\n");
	Delayer("        believe his follwers still reside these very woods, coming out in\n");
	RIGHT(3,xa,ya); RIGHT(1,xm,ym); gotoxy(1,17);
	Delayer("        the dark to pounce on their weak preys.\n");
	Delayer("YOU   : I'm sorry, isn't it dark already, are we in danger??\n");
	RIGHT(3,xa,ya); RIGHT(1,xm,ym); gotoxy(1,19);
	Delayer("ALEXIS: AHH...you city dwellers, this is how late you keep awake?? \n");
	RIGHT(3,xa,ya); RIGHT(1,xm,ym); gotoxy(1,20);
	Delayer("        Evening's barely ended, these 'followers' come out when its pitch \n");
	Delayer("        black out here......like REALLY DARK.....\n");
	RIGHT(3,xa,ya); RIGHT(1,xm,ym);

	for (x=10; x<71; x++)
	{
		for (y=3; y<13; y++)
		{
			if ((x==xa&&y==ya)||(x==xm&&y==ym)) continue;
			if (land[x][y]==2) { gotoxy(x,y); textcolor(8); cprintf("%c",char(219));  }
			else               { gotoxy(x,y); textcolor(16); cprintf("%c",char(219)); }
		}
		delay(20);
	}
	sound(200); delay(250); sound(180); delay(250); sound(160); delay(250);
	sound(140); delay(250); sound(120); delay(250); nosound();

	fl=getch();
	if (fl=='/') exit(0);

	Clr_Lower_();
	gotoxy(1,13);
	Delayer("YOU   : You mean something like this?? Cuz I can't even see you if I dont try...\n");
	Delayer("ALEXIS: Howdaa....This isn't suppose to happen, something's wrong.... \n");
	Delayer("        I think someone's using a spell..... I think we aren't alone.....\n\n");
	getch();
	Delayer("<    >: Precisely, young mage !! You got instincts, I'll give you that...\n");
	Delayer("YOU   : Who in the 10 hells was that? \n");
	Delayer("ALEXIS: I...I don't....What's that ?? \n");
	fl=getch();
	if (fl=='/') exit(0);

	for (x=10; x<71; x++)
	{
		for (y=3; y<13; y++)
		{
			if (ctry%8==0)
			{
				if ((x==xa&&y==ya)||(x==xm&&y==ym)) continue;
				gotoxy(x,y); textcolor(4); cprintf("%c",char(219));
			} ctry++;
		}
		delay(20);
	}
	fl=getch();
	if (fl=='/') exit(0);

	Clr_Lower_();
	gotoxy(1,13);
	Delayer("RAVEN : Oh don't be alarmed, I come in peace.....\n");
	Delayer("( A large hand curved out stone emerges from the ground and grabs Alexis \n");
	Delayer("ALEXIS: Yea, cuz where you come from, this is how you greet everyone.....\n");
	Delayer("RAVEN : HAHAA...The funny type...Isn't she funny,"); Delayer(GM.Show_Name());
	fl=getch();
	if (fl=='/') exit(0);
	Delayer("\n      : haha.........I don't like funny\n");
	Delayer("( STONE_HAND STRENGTHENS GRIP, ALEXIS IN PURE AGONY ) \n");
	Delayer("YOU   : What's your deal man, are you some kind of sadist or something ? Cuz the\n");
	Delayer("        tournament hasn't even started yet, and killing spells aren't allowed! \n");

	Clr_Lower_();
	gotoxy(1,13);
	Delayer("RAVEN : My name's Raven by the way.... I don't ask for much...\n");
	Delayer("        I just want you to make a promise. You may not know this, but I know....\n");
	Delayer("        We...we need to team up man... Its meant to be !! \n");
	Delayer("YOU   : What, me? You must get it wrong, cuz I'm just here to try my luck...\n");
	Delayer("      : I'm not even a mage yet... I'm just here to explore my chances\n");
	Delayer("RAVEN : I know, but I know far more things about you than even.....YOU !!\n");
	Delayer("YOU   : I...I don't understand.... its, a lot to process. \n");
	Delayer("RAVEN : Join me and you'll know..... But first we need to get rid of this loose\n");
	Delayer("        end, she heard too much. Do it for me, would you "); Delayer(GM.Show_Name());
	fl=getch();
	if (fl=='/') exit(0);

	Clr_Lower_();
	gotoxy(1,13);
	Delayer("(A) No I won't, it isn't morale  (B) Take out dagger and attack RAVEN\n");
	Delayer("(C) Well if I do, what's in it for me?? \n");
	cin>>Q[12];
	if (Q[12]=='A'||Q[12]=='a')
	{
		GM.Deactivate_Alexis(); GM.Scr_Add_Five();
		Delayer("RAVEN : CHAP CHAP, Time's Over , gotta move on....\n");
		Delayer(" ( Large Stone Spear emerges from the ground and impales Alexis dead )\n");
		gotoxy(xa,ya); textcolor(4); cprintf("%c",char(219));
		gotoxy(1,18);
		Delayer("RAVEN : You and I gotta a lot of catching up to do....\n");
		Delayer("YOU   : NNNOOOOOOOO........You'll pay for that !!\n");
		for (x=10; x<71; x++)
		{
			for (y=3; y<13; y++)
			{
				if (x==xm&&y==ym) continue;
				if (land[x][y]==2) TREE(x,y); else LAND(x,y);
				delay(20);
			}
		}
	}
	else if (Q[12]=='B'||Q[12]=='b')
	{
		GM.Scr_Add_Five(); GM.Scr_Add_Ten(); GM.Plus_Alexis();
		Delayer("( Raven simply jusy flicks his finger, and you fly off few metres behind )\n");
		Delayer("RAVEN : Brave little lad aren't you, I like it....\n");
		Delayer("        I tell you what..... I spare the girl this time, and the next time we \n");
		Delayer("        cross paths, I want you to think closely what told you today....SeeYa \n");
		for (x=10; x<71; x++)
		{
			for (y=3; y<13; y++)
			{
				if (x==xm&&y==ym) continue;
				if (land[x][y]==2) TREE(x,y); else LAND(x,y);
				delay(20);
			}
		}
	  part:
		Clr_Lower_();
		gotoxy(1,13);
		Delayer("( The stone hands release Alexis..... Alexis struggles for air )\n");
		RIGHT(3,xa,ya); RIGHT(1,xm,ym);
		RIGHT(3,xa,ya); RIGHT(1,xm,ym);
		RIGHT(3,xa,ya); RIGHT(1,xm,ym);
		gotoxy(1,14);
		Delayer("ALEXIS: Thanks "); Delayer(GM.Show_Name()); Delayer("...That is your name, right?\n");
		RIGHT(3,xa,ya); RIGHT(1,xm,ym);
		RIGHT(3,xa,ya); RIGHT(1,xm,ym);
		RIGHT(3,xa,ya); RIGHT(1,xm,ym);
		RIGHT(3,xa,ya); RIGHT(1,xm,ym); gotoxy(1,15);
		Delayer("YOU   : Yaa, Are you alright?? \n");
		RIGHT(3,xa,ya); RIGHT(1,xm,ym);
		RIGHT(3,xa,ya); RIGHT(1,xm,ym);
		RIGHT(3,xa,ya); RIGHT(1,xm,ym);
		RIGHT(3,xa,ya); RIGHT(1,xm,ym); gotoxy(1,16);
		Delayer("ALEXIS: Yaa, I'm fine, Did you know that guy?? \n");
		RIGHT(3,xa,ya); RIGHT(1,xm,ym);
		RIGHT(3,xa,ya); RIGHT(1,xm,ym);
		RIGHT(3,xa,ya); RIGHT(1,xm,ym);
		RIGHT(3,xa,ya); RIGHT(1,xm,ym); gotoxy(1,17);
		Delayer("YOU   : EXACTLY, I never saw him in my life....Wizardry is kinda avoided \n");
		RIGHT(3,xa,ya); RIGHT(1,xm,ym);
		RIGHT(3,xa,ya); RIGHT(1,xm,ym);
		RIGHT(3,xa,ya); RIGHT(1,xm,ym);
		RIGHT(3,xa,ya); RIGHT(1,xm,ym); gotoxy(1,18);
		Delayer("        where I come from....\n");
		Delayer("ALEXIS: Strange things are about to happen in  this tournament, I feel it! \n");
		RIGHT(3,xa,ya); RIGHT(1,xm,ym); gotoxy(1,20);
		Delayer("ALEXIS: Ohh, I guess this is where we part.....\n");
		Delayer("YOU   : What do you mean, aren't you in the tournament??\n");
		Delayer("ALEXIS: I am, but I gotta take care of some stuff first.\n");
		getch();
		Delayer("YOU   : GoodLuck then, we're gonna meet again soon.\n");
		int ctrz=0;
		for (int g=0; g<11; g++)
		{
			if (ya!=6)
			{
				if (ctrz%2==0) { UP(3,xa,ya);  ctrz++; delay(150); }
				else           { RIGHT(3,xa,ya); ctrz++; delay(150); }
			}
			if (xm!=70) RIGHT(1,xm,ym); delay(150);
		}

	}
	else if (Q[12]=='C'||Q[12]=='c')
	{
		bd=1;
		GM.Deactivate_Alexis(); GM.Scr_Sub_Ten();
		Delayer("RAVEN : Hahaa, always looking for some profit....I tell you what.....\n");
		Delayer("        I first end the girl.....And then we talk profits. How 'bout that?\n");
		Delayer(" ( Large Stone Spear emerges from the ground and impales Alexis dead )\n");
		gotoxy(xa,ya); textcolor(4); cprintf("%c",char(219));
		gotoxy(1,18);
		Delayer("RAVEN : CIAO !\n");
		Delayer("YOU   : Daaamn it !! He's a real threat, I need to be careful next time.... \n");
		for (x=10; x<71; x++)
		{
			for (y=3; y<13; y++)
			{
				if (x==xm&&y==ym) continue;
				if (land[x][y]==2) TREE(x,y); else LAND(x,y);
				delay(20);
			}
		}
	}
}

// /*




void CREDITS()
{
clrscr();

	for (x=1; x<81; x++) { for (y=1; y<24; y++) { gotoxy(x,y); textcolor(WHITE); cprintf("%c",char(219)); } }
	gotoxy(1,1); clrscr();
	textcolor(15);  gotoxy(30,2);
	Delayer("BROUGHT TO YOU BY,\n");
	getch(); gotoxy(30,4);
	Delayer("1) Swagat S. Bhuyan -  \n");
	Delayer("\t Chief Syntax designer.\n");
	Delayer("\t Chief Datafile Storage Developer.\n");
	Delayer("\t Assistant Story-line Developer.\n");
	Delayer("\t Assistant Sound-board Designer.\n");
	Delayer("\t Chief Game-Algorithm Developer.\n");
	getch(); gotoxy(30,11);
	Delayer("2) Siddhart Nandi - \n");
	Delayer("\t Chief Sound-board Designer.\n");
	Delayer("\t Assistant Syntax designer.\n");
	Delayer("\t Blinking text_effect designer.\n");
	Delayer("\t Chief Level Designer.\n");
	getch(); gotoxy(30,17);
	Delayer("3) Annesha Phukan - \n");
	Delayer("\t Assistant Sound-board Designer.\n");
	Delayer("\t Chief Story-line Developer.\n");
	Delayer("\t Assistant Syntax designer.\n");
	Delayer("\t Assistant Level Designer.\n");
	getch(); gotoxy(30,23);
	Delayer("THANK YOU..........");
	getch(); exit(0);

}


// ********************************************VINES***********************************

void Paths()
{
	for (x=2; x<33; x++) for (y=1; y<20; y++)  BOLD(x,y);
	for (x=2; x<33; x++) for (y=20; y<24; y++) LAND_(x,y);

	for (y=18; y>13; y--) LAND(5,y);   for (x=5; x<11; x++)   LAND(x,14);
	for (y=16; y>13; y--) LAND(10,y);  for (x=10; x<15; x++)  LAND(x,16);
	for (y=18; y>15; y--) LAND(14,y);  for (x=14; x<19; x++)  LAND(x,18);
	for (y=18; y>10; y--) LAND(18,y);  for (x=18; x<24; x++)  LAND(x,11);
	for (y=11; y>8; y--)  LAND(23,y);  for (x=9; x<24; x++)   LAND(x,9);
	for (y=9; y>5; y--)   LAND(9,y);   for (x=6; x<10; x++)   LAND(x,6);
	for (y=12; y>5; y--)  LAND(6,y);   for (x=3; x<7; x++)    LAND(x,12);
	for (y=12; y>3; y--)  LAND(3,y);   for (x=3; x<26; x++)   LAND(x,4);
	for (y=4; y>0; y--)   LAND(25,y);  for (x=10; x<26; x++)  LAND(x,2);  LAND_(13,1);
	for (y=7; y>3; y--)   LAND(12,y);  for (x=12; x<29; x++)  LAND(x,7);
	for (y=7; y>0; y--)   LAND(28,y);  for (x=18; x<25; x++)  LAND(x,14);
	for (y=14; y>10; y--) LAND(24,y);  for (x=24; x<31; x++)  LAND(x,12);
	for (y=12; y>0; y--)  LAND(30,y);  for (x=11; x<19; x++)  LAND(x,13);
	for (y=13; y>8; y--)  LAND(11,y);  for (x=3; x<7; x++)    LAND(x,8);

	BOLD(24,12); BOLD(11,11); BOLD(4,8); BOLD(24,4);
}

void SLV(int &ctrv, int &xs, int &ys)
{
	if (ctrv==1) UP(5,xs,ys);
	else if (ctrv>=2&&ctrv<=6)     RIGHT(5,xs,ys);
	else if (ctrv>=7&&ctrv<=8)     DOWN (5,xs,ys);
	else if (ctrv>=9&&ctrv<=12)    RIGHT(5,xs,ys);
	else if (ctrv>=13&&ctrv<=14)   DOWN (5,xs,ys);
	else if (ctrv>=15&&ctrv<=18)   RIGHT(5,xs,ys);
	else if (ctrv>=19&&ctrv<=25)   UP   (5,xs,ys);
	else if (ctrv>=26&&ctrv<=30)   RIGHT(5,xs,ys);
	else if (ctrv>=31&&ctrv<=32)   UP   (5,xs,ys);
	else if (ctrv>=33&&ctrv<=46)   LEFT (5,xs,ys);
	else if (ctrv>=47&&ctrv<=49)   UP   (5,xs,ys);
	else if (ctrv>=50&&ctrv<=52)   LEFT (5,xs,ys);
	else if (ctrv>=53&&ctrv<=58)   DOWN (5,xs,ys);
	else if (ctrv>=59&&ctrv<=61)   LEFT (5,xs,ys);
	else if (ctrv>=62&&ctrv<=69)   UP   (5,xs,ys);
	else if (ctrv>=70&&ctrv<=78)   RIGHT(5,xs,ys);
	else if (ctrv>=79&&ctrv<=81)   DOWN (5,xs,ys);
	else if (ctrv>=82&&ctrv<=107)  RIGHT(5,xs,ys);
	else if (ctrv>=108&&ctrv<=113) UP   (5,xs,ys);
	ctrv++;
}

int Vines()
{
clrscr();

	char mv; int xv=5, yv=21, xs=30, ys=21, ctrv=1;
	Paths();
	ME(xv,yv); SL(xs,ys);

	gotoxy(34,2); Delayer("SYLVIA: Give me a boost.....");
	fl=getch(); if (fl=='/') exit(0);
	while(xs!=5) { LEFT(5,xs,ys); delay(25); } ys=15;
	ME(xv,yv); SL(xs,ys);
	gotoxy(34,3); Delayer("SYLVIA: Can't you humans jump or something ??");
	gotoxy(34,4); Delayer("YOU   : Huh, funny.....");
  BEEG:
	gotoxy(34,5); Delayer("( Press 'i' to jump onto the vines....");
	fl=getch(); if (fl=='/') exit(0);
	else if (fl=='i') yv=18;
	else goto BEEG;
	LAND_(5,21); ME(xv,yv);
	gotoxy(34,6); Delayer("YOU   : You were saying ?");
	gotoxy(34,7); Delayer("SYLVIA: Huh....easy luck !");
	gotoxy(34,8); Delayer("SYLVIA: Now follow me closely....");
	gotoxy(34,9); Delayer("( Use wasd controls to follow Sylvia )");
	gotoxy(34,10); Delayer("( as she climbs the vines to reach the top.)");
	fl=getch(); if (fl=='/') exit(0);

	while(1)
	{
		SLV(ctrv,xs,ys);
		if (xs==28&&ys==1) LAND(28,1);
		if (xv==28&&yv==1) break;
		if (ctrv==130) { gotoxy(34,12); Delayer("Whats taking you so long...???"); }
		mv=getch();
		if (mv=='w')
			UP(1,xv,yv);
		else if (mv=='a')
			LEFT(1,xv,yv);
		else if (mv=='s')
			DOWN(1,xv,yv);
		else if (mv=='d')
			RIGHT(1,xv,yv);
		else if (mv=='/')
			exit(0);
	}
	gotoxy(34,14); Delayer("SYLVIA: Huh...you finally made it....lets go now....");
	fl=getch(); if (fl=='/') exit(0);
	gotoxy(1,1);
	return ctrv;

getch();
}

// ***************************************************************************************



// *************************************************ALX*******************************



void ALX()
{
	clrscr();
	time_t t;
	int xe, ye, ctre=281;
	for (x=10; x<71; x++) LAND_(x,21);
	for (x=5; x<75; x++) land[x][1]=1;
	land[9][20]=1; land[71][20]=1;
	int lx=20, ly=20, xt, yt;
	ME(lx,ly);
  BEGY:
	while(1)
	{
		if (ctre%281==0)
		{ SPACE(xe,ye); srand((unsigned) time(&t)); xe=12+rand()%65; ye=1+rand()%17; }
		EE(xe,ye);
		if (kbhit())
		{
			xt=lx; yt=ly;
			if (gre==1) break;
			mv=getch();
			if (mv=='a'||mv=='A')
				LEFT(6,lx,ly);
			else if (mv=='d'||mv=='D')
				RIGHT(6,lx,ly);
			else if (mv=='/')
				exit(0);
			else if (mv==']')
				MAP__();
			else if (mv=='i')
			{  yt--; while(stp==0) UP(7,xt,yt); stp=0; }
		}
		ctre++; delay(5);
	}
	cout<<"YOU HIT TARGET......."; getch();

}

//  *********************************************************************************************


// */

void Layoff(int clr)
{
	for (x=1; x<81; x++) { for (y=1; y<24; y++) { gotoxy(x,y); textcolor(WHITE); cprintf("%c",char(219)); } }
	gotoxy(1,1); clrscr();
}

void Layoff_WHITE()
{
	for (x=1; x<81; x++) { for (y=1; y<24; y++) { gotoxy(x,y); textcolor(WHITE); cprintf("%c",char(219)); } }
	gotoxy(1,1); clrscr();
}
void Layoff_FROST()
{
	for (x=1; x<81; x++) { for (y=1; y<24; y++) { gotoxy(x,y); textcolor(WHITE); cprintf("%c",char(219)); } }
	gotoxy(1,1); clrscr();
}

int River_Dale(int);

int MAINSCREEN()
{
clrscr();

	int ctrm=1;
	Layoff_WHITE();
	for (x=1; x<81; x++)
	{ for (y=1; y<24; y++) { gotoxy(x,y); textcolor(15); } }
	char ch;
	int y=12, yy;

	for (int gg=1; gg<11; gg++) M_BOX(gg);
	gotoxy(32,10); Delayer("\t   MAGE_RUNNER");
	gotoxy(32,11); Delayer("\t   ^^^^^^^^^^^");

	ctrm=1; ctra=281;

	gotoxy(36,12);	textcolor(15); cprintf("%s","1.NEW GAME");
	gotoxy(36,13);	textcolor(15); cprintf("%s","2.LOAD GAME");
	gotoxy(36,14);	textcolor(15); cprintf("%s","3.SHOW DATA");
	gotoxy(36,15);	textcolor(15); cprintf("%s","4.MAP");
	gotoxy(36,16);	textcolor(15); cprintf("%s","5.EXIT");
	gotoxy(32,19);  textcolor(15); cprintf("%s","ver2.0.3 (Demo-Beta)");
	gotoxy(32,18);  textcolor(15); cprintf("%s","('j' for piano-fest)");
	gotoxy(35,12);  textcolor(15); cprintf("%c",char(175)); ch=getch();
	while (1)
	{
		if (ctra%281==0) M_BOX(ctrm);

		if (kbhit())
		{
			ch=getch();
			if (ch=='w')
			{
				if (y==12)	{ gotoxy(35,12); cout<<" ";	gotoxy(35,16);	cout<<char(175); y=16;	}
				else if (y==13)	{ gotoxy(35,13); cout<<" ";	gotoxy(35,12);	cout<<char(175); y=12;	}
				else if (y==14)	{ gotoxy(35,14); cout<<" ";	gotoxy(35,13);	cout<<char(175); y=13;	}
				else if (y==15)	{ gotoxy(35,15); cout<<" ";	gotoxy(35,14);	cout<<char(175); y=14;	}
				else if (y==16)	{ gotoxy(35,16); cout<<" ";	gotoxy(35,15);	cout<<char(175); y=15;	}
			}
			else if (ch=='s')
			{
				if (y==16)	{ gotoxy(35,16); cout<<" ";	gotoxy(35,12);	cout<<char(175); y=12;	}
				else if (y==15)	{ gotoxy(35,15); cout<<" ";	gotoxy(35,16);	cout<<char(175); y=16;	}
				else if (y==14)	{ gotoxy(35,14); cout<<" ";	gotoxy(35,15);	cout<<char(175); y=15;	}
				else if (y==13)	{ gotoxy(35,13); cout<<" ";	gotoxy(35,14);	cout<<char(175); y=14;	}
				else if (y==12)	{ gotoxy(35,12); cout<<" ";	gotoxy(35,13);	cout<<char(175); y=13;	}
			}
			else if (ch=='j') JUTE_BOX();
			else if (ch==13)
			{
				if (y==12)      yy=1;
				else if (y==13) yy=2;
				else if (y==14) yy=3;
				else if (y==15) yy=4;
				else if (y==16) yy=5;
				return yy;
			}
		}
		ctra++;
	}
}


void MAP()     //textcolor(GREEN); cprintf("0");
{
clrscr();

//1
	gotoxy(50,1); textcolor(11); cprintf("%c",char(219));
	gotoxy(51,1); textcolor(11); cprintf("%c",char(219)); delay(30);
	gotoxy(52,1); textcolor(11); cprintf("%c",char(219));
	gotoxy(49,1); textcolor(11); cprintf("%c",char(219)); delay(30);
	gotoxy(48,1); textcolor(11); cprintf("%c",char(219));
	gotoxy(47,1); textcolor(11); cprintf("%c",char(219)); delay(30);
	for (c=47; c<53; c++)	cord[c][1]=1;

//2
	gotoxy(17,2); textcolor(11); cprintf("%c",char(219)); cord[17][2]=1;
	gotoxy(18,2); textcolor(11); cprintf("%c",char(219)); delay(30); cord[18][2]=1;
	gotoxy(49,2); textcolor(11); cprintf("%c",char(219)); cord[49][2]=1;
	gotoxy(50,2); textcolor(11); cprintf("%c",char(219)); delay(30); cord[50][2]=1;
	gotoxy(51,2); textcolor(11); cprintf("%c",char(219)); cord[51][2]=1;
	gotoxy(48,2); textcolor(11); cprintf("%c",char(219)); delay(30); cord[48][2]=1;

//3
	for (int a=0; a<4; a++)	{ gotoxy(a+16,3); textcolor(11); cprintf("%c",char(219)); delay(10);}
	for (c=16; c<20; c++)	cord[c][3]=1;
	gotoxy(32,3); textcolor(11); cprintf("%c",char(219)); cord[32][3]=1;
	gotoxy(33,3); textcolor(11); cprintf("%c",char(219)); delay(30); cord[33][3]=1;
	gotoxy(49,3); textcolor(11); cprintf("%c",char(219)); cord[49][3]=1;
	gotoxy(50,3); textcolor(11); cprintf("%c",char(219)); delay(30); cord[50][3]=1;
	gotoxy(51,3); textcolor(11); cprintf("%c",char(219)); cord[51][3]=1;
	gotoxy(52,3); textcolor(11); cprintf("%c",char(219)); delay(30); cord[52][3]=1;

//4
	gotoxy(2,4); textcolor(11); cprintf("%c",char(219)); cord[2][4]=1;
	for (int b=-4; b<12; b++)	{ gotoxy(b+17,4); textcolor(GREEN); cprintf("%c",char(219)); delay(10);}
	for (c=-4; c<12; c++)	cord[c+17][4]=1;
	gotoxy(13,4); textcolor(11); cprintf("%c",char(219)); cord[13][4]=1;
	gotoxy(27,4); textcolor(11); cprintf("%c",char(219)); cord[27][4]=1;
	gotoxy(32,4); textcolor(11); cprintf("%c",char(219)); cord[32][4]=1;
	gotoxy(28,4); textcolor(11); cprintf("%c",char(219)); cord[28][4]=1;
	gotoxy(48,4); textcolor(11); cprintf("%c",char(219)); delay(30); cord[48][4]=1;

//5
	for (int c=3; c<33; c++) { gotoxy(c,5); textcolor(GREEN); cprintf("%c",char(219)); delay(10);}
	for (c=3; c<33; c++)	cord[c][5]=1;
	gotoxy(65,5); textcolor(11); cprintf("%c",char(219)); cord[65][5]=1;
	gotoxy(78,5); textcolor(11); cprintf("%c",char(219)); delay(10); cord[78][5]=1;
	gotoxy(79,5); textcolor(11); cprintf("%c",char(219)); delay(30); cord[79][5]=1;
	gotoxy(32,5); textcolor(8); cord[32][5]=1;

//6
	for (d=2; d<37; d++) { gotoxy(d,6); textcolor(GREEN); cprintf("%c",char(219)); delay(30);}
	for (c=65; c<78; c++) { gotoxy(c,6); textcolor(GREEN); cprintf("%c",char(219)); delay(10);}
	for (c=2; c<37; c++)	cord[c][6]=1;
	for (c=65; c<78; c++)	cord[c][6]=1;
	for (d=6; d<30; d++) { gotoxy(d,6); textcolor(10); cprintf("%c",char(219)); delay(30);}
	for (c=66; c<78; c++) { gotoxy(c,6); textcolor(8); cprintf("%c",char(219)); delay(10);}
	gotoxy(35,6); textcolor(7); cprintf("%c",char(219)); cord[35][6]=1;
	gotoxy(34,6); textcolor(7); cprintf("%c",char(219)); cord[34][6]=1;
	gotoxy(33,6); textcolor(7); cprintf("%c",char(219)); cord[33][6]=1;
	gotoxy(32,6); textcolor(7); cprintf("%c",char(219)); cord[32][6]=1;
	gotoxy(32,6); textcolor(7); cord[32][6]=1;
	gotoxy(4,6); textcolor(8); cprintf("%c",char(219));

//7
	for (c=2; c<36; c++) { gotoxy(c,7); textcolor(GREEN); cprintf("%c",char(219)); delay(10);}
	for (c=63; c<79; c++) { gotoxy(c,7); textcolor(GREEN); cprintf("%c",char(219)); delay(10);}
	for (c=2; c<36; c++)	cord[c][7]=1;
	for (c=63; c<79; c++)	cord[c][7]=1;
	for (d=5; d<32; d++) { gotoxy(d,7); textcolor(10); cprintf("%c",char(219)); delay(30);}
	for (c=67; c<71; c++) { gotoxy(c,7); textcolor(8); cprintf("%c",char(219)); delay(10);}
	for (c=72; c<78; c++) { gotoxy(c,7); textcolor(10); cprintf("%c",char(219)); delay(10);}
	gotoxy(33,7); textcolor(7); cprintf("%c",char(219));
	gotoxy(34,7); textcolor(7); cprintf("%c",char(219));
	gotoxy(35,7); textcolor(7); cprintf("%c",char(219));
	gotoxy(36,7); textcolor(7); cprintf("%c",char(219));
	gotoxy(28,7); textcolor(7); cprintf("%c",char(219));
	gotoxy(29,7); textcolor(7); cprintf("%c",char(219));
	gotoxy(30,7); textcolor(7); cprintf("%c",char(219));
	gotoxy(31,7); textcolor(7); cprintf("%c",char(219));
	gotoxy(43,7); textcolor(RED); cprintf("%c",char(219)); cord[43][7]=1;
	gotoxy(32,7); textcolor(8); cprintf("%c",char(219));
	gotoxy(45,7); textcolor(GREEN); cprintf("%c",char(219)); delay(30); cord[45][7]=1;
	gotoxy(4,7); textcolor(8); cprintf("%c",char(219));

//8
	for (c=2; c<33; c++) { gotoxy(c,8); textcolor(GREEN); cprintf("%c",char(219)); delay(10);}
	for (c=64; c<78; c++) { gotoxy(c,8); textcolor(GREEN); cprintf("%c",char(219)); delay(10);}
	gotoxy(64,8); textcolor(7); cprintf("%c",char(219)); cord[30][8]=1;
	gotoxy(65,8); textcolor(7); cprintf("%c",char(219)); cord[30][8]=1;
	gotoxy(78,8); textcolor(7); cprintf("%c",char(219)); cord[30][8]=1;
	for (c=42; c<49; c++) { gotoxy(c,8); textcolor(RED); cprintf("%c",char(219)); delay(10);}
	for (c=2; c<33; c++)	cord[c][8]=1;
	for (c=64; c<78; c++)	cord[c][8]=1;
	for (c=42; c<49; c++)	cord[c][8]=1;
	for (d=5; d<30; d++) { gotoxy(d,8); textcolor(10); cprintf("%c",char(219)); delay(30);}
	gotoxy(30,8); textcolor(7); cprintf("%c",char(219)); cord[30][8]=1;
	gotoxy(31,8); textcolor(7); cprintf("%c",char(219)); cord[31][8]=1;
	gotoxy(4,8); textcolor(8); cprintf("%c",char(219));
	gotoxy(20,8); textcolor(BLUE); cprintf("%c",char(219));

//9
	for (c=3; c<33; c++) { cord[c][9]=1; gotoxy(c,9); textcolor(GREEN); cprintf("%c",char(219)); delay(10);}
	gotoxy(43,9); textcolor(GREEN); cprintf("%c",char(219)); delay(10); cord[43][9]=1;
	for (c=68; c<73; c++) { cord[c][9]=1; gotoxy(c,9); textcolor(GREEN); cprintf("%c",char(219)); delay(10);}
	for (c=43; c<47; c++) { cord[c][9]=1; gotoxy(c,9); textcolor(RED); cprintf("%c",char(219)); delay(10);}
	gotoxy(68,9); textcolor(7); cprintf("%c",char(219)); cord[30][8]=1;
	gotoxy(45,9); textcolor(8); cprintf("%c",char(219)); cord[30][8]=1;
	gotoxy(69,9); textcolor(7); cprintf("%c",char(219)); cord[30][8]=1;
	gotoxy(72,9); textcolor(7); cprintf("%c",char(219)); cord[30][8]=1;
	gotoxy(30,9); textcolor(7); cprintf("%c",char(219)); cord[30][9]=1;
	gotoxy(31,9); textcolor(7); cprintf("%c",char(219)); cord[31][9]=1;
	gotoxy(4,9); textcolor(8); cprintf("%c",char(219));
	gotoxy(5,9); textcolor(8); cprintf("%c",char(219));
	gotoxy(20,9); textcolor(BLUE); cprintf("%c",char(219));
	for (d=10; d<28; d++) { gotoxy(d,9); textcolor(10); cprintf("%c",char(219)); delay(30);}

//10
	for (c=4; c<36; c++) { cord[c][10]=1; gotoxy(c,10); textcolor(GREEN); cprintf("%c",char(219)); delay(10);}
	for (c=42; c<45; c++) { cord[c][10]=1; gotoxy(c,10); textcolor(RED); cprintf("%c",char(219)); delay(10);}
	gotoxy(67,10); textcolor(7); cprintf("%c",char(219)); cord[67][10]=1;
	gotoxy(45,10); textcolor(RED); cprintf("%c",char(219)); delay(30); cord[45][10]=1;
	gotoxy(31,10); textcolor(7); cord[31][10]=1;
	gotoxy(19,10); textcolor(BLUE); cprintf("%c",char(219));
	gotoxy(20,10); textcolor(BLUE); cprintf("%c",char(219));
	gotoxy(21,10); textcolor(BLUE); cprintf("%c",char(219));
	gotoxy(22,10); textcolor(BLUE); cprintf("%c",char(219));
	gotoxy(23,10); textcolor(BLUE); cprintf("%c",char(219));
	for (d=12; d<24; d++) { gotoxy(d,10); textcolor(10); cprintf("%c",char(219)); delay(30);}

//11
	gotoxy(2,11); textcolor(GREEN); cprintf("%c",char(219)); cord[2][11]=1;
	gotoxy(3,11);	textcolor(GREEN); cprintf("%c",char(219)); delay(30); cord[3][11]=1;
	for (c=6; c<29; c++) { cord[c][11]=1; gotoxy(c,11); textcolor(GREEN); cprintf("%c",char(219)); delay(10);}
	gotoxy(35,11); textcolor(7); cprintf("%c",char(219)); cord[35][11]=1;
	gotoxy(78,11); textcolor(7); cprintf("%c",char(219)); delay(30); cord[78][11]=1;
	gotoxy(43,11); textcolor(GREEN); cprintf("%c",char(219)); cord[43][11]=1;
	gotoxy(44,11); textcolor(GREEN); cprintf("%c",char(219)); delay(30); cord[44][11]=1;
	gotoxy(20,11); textcolor(BLUE); cprintf("%c",char(219));
	gotoxy(21,11); textcolor(BLUE); cprintf("%c",char(219));

//12
	for (c=3; c<28; c++) { cord[c][12]=1; gotoxy(c,12); textcolor(GREEN); cprintf("%c",char(219)); delay(10);}
	for (c=76; c<79; c++) { cord[c][12]=1; gotoxy(c,12); textcolor(7); cprintf("%c",char(219)); delay(10);}
	gotoxy(20,12); textcolor(BLUE); cprintf("%c",char(219));

//13
	gotoxy(2,13); textcolor(7); cprintf("%c",char(219)); cord[2][13]=1;
	gotoxy(3,13); textcolor(7); cprintf("%c",char(219)); delay(30); cord[3][13]=1;
	gotoxy(4,13); textcolor(7); cprintf("%c",char(219)); delay(30); cord[4][13]=1;
	gotoxy(7,13); textcolor(7); cprintf("%c",char(219)); cord[7][13]=1;
	gotoxy(26,13); textcolor(7); cprintf("%c",char(219)); delay(30); cord[26][13]=1;
	gotoxy(27,13); textcolor(7); cprintf("%c",char(219)); cord[27][13]=1;
	gotoxy(28,13); textcolor(7); cprintf("%c",char(219)); delay(30); cord[28][13]=1;
	gotoxy(54,13); textcolor(7); cprintf("%c",char(219)); cord[54][13]=1;
	gotoxy(55,13); textcolor(7); cprintf("%c",char(219)); delay(30); cord[55][13]=1;
	gotoxy(75,13); textcolor(7); cprintf("%c",char(219)); cord[75][13]=1;

//14
	gotoxy(7,14); textcolor(7); cprintf("%c",char(219)); cord[7][14]=1;
	gotoxy(63,14); textcolor(7); cprintf("%c",char(219)); delay(30); cord[63][14]=1;
	gotoxy(19,14); textcolor(7); cprintf("%c",char(219)); cord[19][14]=1;
	gotoxy(21,14); textcolor(7); cprintf("%c",char(219)); delay(30); cord[21][14]=1;
	for (c=53; c<57; c++) { cord[c][14]=1; gotoxy(c,14); textcolor(GREEN); cprintf("%c",char(219)); delay(10);}
	gotoxy(53,14); textcolor(7); cprintf("%c",char(219)); delay(30);
	gotoxy(56,14); textcolor(7); cprintf("%c",char(219)); delay(30);

//15
	for (c=52; c<64; c++) { cord[c][15]=1; gotoxy(c,15); textcolor(GREEN); cprintf("%c",char(219)); delay(10);}
	for (c=18; c<23; c++) { cord[c][15]=1; gotoxy(c,15); textcolor(7); cprintf("%c",char(219)); delay(10);}
	gotoxy(52,15); textcolor(7); cprintf("%c",char(219)); delay(30);
	gotoxy(63,15); textcolor(7); cprintf("%c",char(219)); delay(30);
	gotoxy(62,15); textcolor(7); cprintf("%c",char(219)); delay(30);
	gotoxy(77,15); textcolor(7); cprintf("%c",char(219)); cord[77][15]=1;
	gotoxy(78,15); textcolor(7); cprintf("%c",char(219)); delay(30); cord[78][15]=1;

//16
	gotoxy(3,16); textcolor(GREEN); cprintf("%c",char(219)); cord[c][16]=1;
	gotoxy(3,16); textcolor(7); cprintf("%c",char(219)); cord[79][17]=1;
	gotoxy(40,16); textcolor(7); cprintf("%c",char(219)); cord[79][17]=1;
	gotoxy(40,16); textcolor(7); cprintf("%c",char(219)); delay(30); cord[40][16]=1;
	for (c=53; c<61; c++) { cord[c][16]=1; gotoxy(c,16); textcolor(7); cprintf("%c",char(219)); delay(10);}
	gotoxy(53,16); textcolor(7); cprintf("%c",char(219)); delay(30);
	gotoxy(60,16); textcolor(7); cprintf("%c",char(219)); delay(30);
	for (c=15; c<25; c++) { cord[c][16]=1; gotoxy(c,16); textcolor(GREEN); cprintf("%c",char(219)); delay(10);}
	gotoxy(78,16); textcolor(GREEN); cprintf("%c",char(219)); cord[78][16]=1;

//17
	gotoxy(3,17); textcolor(GREEN); cprintf("%c",char(219)); cord[3][17]=1;
	gotoxy(4,17); textcolor(GREEN); cprintf("%c",char(219)); delay(10); cord[4][17]=1;
	gotoxy(38,17); textcolor(GREEN); cprintf("%c",char(219)); cord[38][17]=1;
	gotoxy(39,17); textcolor(GREEN); cprintf("%c",char(219)); delay(10); cord[39][17]=1;
	gotoxy(54,17); textcolor(7); cprintf("%c",char(219)); cord[54][17]=1;
	gotoxy(55,17); textcolor(7); cprintf("%c",char(219)); delay(10); cord[55][17]=1;
	gotoxy(77,17); textcolor(GREEN); cprintf("%c",char(219)); cord[77][17]=1;
	gotoxy(78,17); textcolor(GREEN); cprintf("%c",char(219)); delay(10); cord[78][17]=1;
	gotoxy(79,17); textcolor(GREEN); cprintf("%c",char(219)); cord[79][17]=1;
	gotoxy(33,17); textcolor(7); cprintf("%c",char(219)); cord[79][17]=1;
	gotoxy(10,17); textcolor(7); cprintf("%c",char(219)); cord[79][17]=1;
	for (c=10; c<21; c++) { cord[c][17]=1; gotoxy(c,17); textcolor(GREEN); cprintf("%c",char(219)); delay(10);}
	for (c=24; c<33; c++) { cord[c][17]=1; gotoxy(c,17); textcolor(GREEN); cprintf("%c",char(219)); delay(10);}
	for (c=12; c<18; c++) { gotoxy(c,17); textcolor(10); cprintf("%c",char(219)); delay(10);}
	for (c=26; c<32; c++) { gotoxy(c,17); textcolor(10); cprintf("%c",char(219)); delay(10);}

//18
	for (c=4; c<43; c++) { cord[c][18]=1; gotoxy(c,18); textcolor(GREEN); cprintf("%c",char(219)); delay(10);}
	for (c=6; c<40; c++) { cord[c][19]=1; gotoxy(c,18); textcolor(10); cprintf("%c",char(219)); delay(30);}
	for (c=74; c<81; c++) { cord[c][18]=1; gotoxy(c,18); textcolor(GREEN); cprintf("%c",char(219)); delay(10);}
	for (c=76; c<81; c++) { cord[c][18]=1; gotoxy(c,18); textcolor(8); cprintf("%c",char(219)); delay(10);}

//19
	for (c=6; c<46; c++) { cord[c][19]=1; gotoxy(c,19); textcolor(GREEN); cprintf("%c",char(219)); delay(30);}
	for (c=20; c<41; c++) { cord[c][19]=1; gotoxy(c,19); textcolor(8); cprintf("%c",char(219)); delay(30);}
	for (c=74; c<81; c++) { cord[c][19]=1; gotoxy(c,19); textcolor(GREEN); cprintf("%c",char(219)); delay(30);}
	gotoxy(72,19); textcolor(7); cprintf("%c",char(219)); cord[72][19]=1;
	for (c=75; c<81; c++) { cord[c][19]=1; gotoxy(c,19); textcolor(8); cprintf("%c",char(219)); delay(30);}

//20
	for (c=7; c<32; c++) { cord[c][20]=1; gotoxy(c,20); textcolor(8); cprintf("%c",char(219)); delay(30);}
	for (c=73; c<80; c++) { cord[c][20]=1; gotoxy(c,20); textcolor(GREEN); cprintf("%c",char(219)); delay(30);}
	for (c=75; c<80; c++) { cord[c][20]=1; gotoxy(c,20); textcolor(8); cprintf("%c",char(219)); delay(30);}

//WATER
	for (c=1; c<81; c++)
	{
		for (d=1; d<21; d++)
		{
			if (cord[c][d]!=1)
			{   gotoxy(c,d); textcolor(BLUE); cprintf("%c",char(219)); delay(5);	}
		}
	}

//Nomenclature
	gotoxy(1,1); textcolor(WHITE); cprintf("1.Titanium Crib");
	for (c=1; c<16; c++)	cord[c][1]=1;
	gotoxy(54,1); textcolor(WHITE); cprintf("2.Frost Sands");
	for (c=54; c<67; c++)	cord[c][1]=1;
	gotoxy(49,9); textcolor(WHITE); cprintf("3.Redland");
	for (c=49; c<58; c++)	cord[c][9]=1;
	gotoxy(67,4); textcolor(WHITE); cprintf("4.Linustasia");
	for (c=67; c<79; c++)	cord[c][4]=1;
	gotoxy(53,12); textcolor(WHITE); cprintf("5.Dazemberg");
	for (c=53; c<64; c++)	cord[c][12]=1;
	gotoxy(1,21); textcolor(WHITE); cprintf("6.AlphaGard");
	for (c=1; c<12; c++)	cord[c][21]=1;
	gotoxy(58,21); textcolor(WHITE); cprintf("7.Starkgaryen Hills"); delay(200);
	for (c=58; c<77; c++)	cord[c][21]=1;
	gotoxy(1,22);
	Delayer("THIS IS THE MAP OF GALACTRA, YOUR HOME-PLANET ! CHOOSE YOUR CONTINENT: ");


getch();
}

void GoodBye()
{
clrscr();

	gotoxy(36,13); cout<<"BYE-BYE!!";

getch();
exit(0);
}



// Continental Briefing
void Titanium()
{
clrscr();

	Delayer("\t   Ahh.... the vast land of Titanium Crib is home to\n");
	Delayer("\t   about 180 million Humans, 12 million Zorks, and only a \n");
	Delayer("\t   handfull of other races. This Human-dominated continent\n");
	Delayer("\t   is ruled by Aryan Salcedo IV. Infact, the Great Mage\n");
	Delayer("\t   Tournament to be held in the city of Ureka is in the \n");
	Delayer("\t   north-eastern province of this very continent. That means\n");
	Delayer("\t   you don't have to pass through the inter-continental\n");
	Delayer("\t   Gatekeeper - Sir Javelin, who can be pretty annoying at times!\n");
	GM.level=9;
	Update();
	fl=getch();
	if (fl=='/') exit(0);


}
void Frost()
{
clrscr();

	Delayer("\t   These frozen lands are very hostile to their inhabitants.\n");
	Delayer("\t   Thats what makes them more susceptible to harsh conditions\n");
	Delayer("\t   Many mages who are born here are most probably predominantly\n");
	Delayer("\t   Ice mages, with a few exceptions of course. These lands are\n");
	Delayer("\t   dominated by a large population of Polars, with a small fraction of\n");
	Delayer("\t   Humans and Elves. Only the city of Polaris stands a running \n");
	Delayer("\t   monarch in this continent, and all the rest are just villages\n");
	Delayer("\t   and nomadic settlements.\n");
	fl=getch();
	if (fl=='/') exit(0);

}
void Redland()
{
clrscr();

	Delayer("\t   Once an epitome of the Golden Quazark rule, this continent\n");
	Delayer("\t   now lies barren with only a handful of Zorks and Quazarks\n");
	Delayer("\t   coexisting in temporary peace. The mainlands are scarred with\n");
	Delayer("\t   volcanic residue of the Great Quazark-Titanium war, which\n");
	Delayer("\t   overthrew the existing treacherous Quazark reign, which caused\n");
	Delayer("\t   havoc throughout the seven continents of Mother_Galactra. Only \n");
	Delayer("\t   a handful of Quazarks remain, but these Quazarks are not to\n");
	Delayer("\t   be taken lightly, as Quazarks are born with the highest Content\n");
	Delayer("\t   of Wizardrix, which makes good mages. They are the strongest\n");
	Delayer("\t   Fire mages, and also excellent with the sword!\n");
	fl=getch();
	if (fl=='/') exit(0);

}
void Linustasia()
{
clrscr();

	Delayer("     This continent has a high population of Elf (about 60 million), and traces\n");
	Delayer("     of polars who migrated  long while back during the great Polaris\n");
	Delayer("     Disasters, which were a series of devastating earthquakes, draughts and\n");
	Delayer("     volcanic outbursts, that took the lives of about 2 million in just\n");
	Delayer("     a span of 3 months. Elves here follow democracy, with King Jonas as their\n");
	Delayer("     ruling president.(He's called king for traditional reasons).\n");
	fl=getch();
	if (fl=='/') exit(0);

}
void Dazemberg()
{
clrscr();

	Delayer("     Dazemberg is the currect hub of wizardry education in the whole planet.\n");
	Delayer("     Young students aiming to be mages come from various parts of the planet\n");
	Delayer("     to complete their education here. Wizards and other participants from these\n");
	Delayer("     parts are extremely talented in psychic powers and stone element.\n");
	Delayer("     Catalan Dorain is the current President of this Domocracy. This is the \n");
	Delayer("     only continent that didn't participate in the great Titanium-Redland Wars.\n");
	fl=getch();
	if (fl=='/') exit(0);

}
void Alphagard()
{
clrscr();

	Delayer("     With a staggering population of 156 million Zorks and a few million humans,\n");
	Delayer("     this continent produces the best Tech_Mages and Thunder_Mages.\n");
	Delayer("     The Wizards from this continent played an important role in bringing down \n");
	Delayer("     the Redland Dictatorship. The great tournaments held every year \n");
	Delayer("     in Titanium Crib are funded almost entirely by rich Zork capitalists \n");
	Delayer("     and sponsored by Zork Tech groups and companies, that made trillions of \n");
	Delayer("     Mesos out of the Redland-Titanium wars. (Meso-universal currency) \n");
	fl=getch();
	if (fl=='/') exit(0);

}
void Starkgaryen()
{
clrscr();

	Delayer("     Said to have been rules by the Starks, an extinct race of advanced tech\n");
	Delayer("     said to have been wiped out due to civil wars and various rebellions lead\n");
	Delayer("     by Ornlu, Yerko and the Furore society of Mages: known as the horsemen of \n");
	Delayer("     apocalypse. Yerko is said to have aged out, Furores were all executed after\n");
	Delayer("     the Redland-Titanium wars, and Ornlu is a 10 foot large dire wolf, still \n");
	Delayer("     lurking around forrets and villages of Titanium Crib. \n");
	fl=getch();
	if (fl=='/') exit(0);

}

//MAIN_GAME
int Act_I(int cont)
{
clrscr();

	if (cont!=1)
	{
		int Score=0;
		if (cont==101)	goto LVL_1;
		if (cont==102)	goto LVL_2;
		if (cont==66)	goto GateKeeper;
		if (cont==103)	goto LVL_3;
		if (cont==104)	goto NATHAN;
		if (cont==105)	goto LVL_5;
		if (cont==9)	goto LVL_9;
		if (cont==10)	goto LVL_10;

	  LVL_1:
		cout<<"\n\n\t"<<GM.Show_Name();	Delayer(", The tournament's about to begin....\n");
		Delayer("\tGet your Sorcery equipments ready, when you're ready....just\n");
		Delayer("\tput your hands over the teleportation flame, and within seconds,\n");
		Delayer("\tyou'll find yourself infront of the gates to Titanium Crib.\n");
		getch();
	  Teleportation:
		Delayer("(Press 'y' to put your hands over the teleportation flame)");
		fl=getch();
		if (fl=='y'||fl=='Y') {	cout<<"\n\nSWISH_SWISH_SWOOSH_SWOOSH !!";	getch();	}
		else if (fl=='/') exit(0);
		else
			goto Teleportation;

	  GateKeeper:
		clrscr();
		Delayer("Sir_Javelin: Who there wishes to enter the Great city of Ureka?\n");
		Delayer("             Answer me, or you SHALL_NOT_PASS !!\n");
		cout<<GM.Show_Name()<<": \n";
		fl=getch();
		if (fl=='/') exit(0);
		cout<<"(A) My name is "<<GM.Show_Name()<<"\t(B) My name is none of your concern...";
		cout<<"\n(C) MAA NAME'S JEFFF.....\n";
		cin>>Q[0];
		if (Q[0]=='A'||Q[0]=='a')
		{	cout<<"OK....."<<GM.Show_Name()<<"\n";	GM.Scr_Add_Five();	   }
		else if (Q[0]=='b'||Q[0]=='B')
		{	cout<<"That was unwise, young mage...\n";  GM.Scr_Sub_Five();  }
		Delayer("Sir_Javelin: U shall only pass if your answers to the\n");
		Delayer("             following questions are satisfactory....");
		GM.level=2;
		Update();
		fl=getch();
		if (fl=='/') exit(0);
	  LVL_2:


	//QUIZ
		clrscr();

		Delayer("1.The Great Annual Mage Tournament is being held in which of the following   \tcities?");
		Delayer("\n(A)Domos\t(B)Ureka\t(C)Polaris\t(D)Bogota\n");
		cin>>Q[1];
		if (Q[1]=='B'||Q[1]=='b')	Score+=4;
		else if (Q[1]=='/') exit(0);

		Delayer("2.Which is the smallest continent in Galactra?");
		Delayer("\n(A)Titanium_Crib\t(B)Redland\t(C)Alphagard\t(D)Frost_Sands\n");
		cin>>Q[2];
		if (Q[2]=='D'||Q[2]=='d')	Score+=4;
		else if (Q[2]=='/') exit(0);

		Delayer("3.Who is the current monarch of Titanium_Crib?");
		Delayer("\n(A)Aryan Salcedo IV\t(B)King Jonas V\t(C)Gladorius II\t(D)King Maharshala\n");
		cin>>Q[3];
		if (Q[3]=='A'||Q[3]=='a')	Score+=4;
		else if (Q[3]=='/') exit(0);

		Delayer("4.Which of the following is a Zork-dominant continent....");
		Delayer("\n(A)Titanium_Crib\t(B)Alphagard\t(C)Dazemberg\t(D)Redland\n");
		cin>>Q[4];
		if (Q[4]=='B'||Q[4]=='b')	Score+=4;
		else if (Q[4]=='/') exit(0);

		Delayer("5.Which Quazark dictator was overthrown after the Great Titanium\n");
		Delayer("  -Redland wars just a few years back.");
		Delayer("\n(A)Catalan Dorain\t(B)Mamedove III\n(C)Ignis Furore\t(D)King Jonas V\n");
		cin>>Q[5];
		if (Q[5]=='C'||Q[5]=='c')	Score+=4;
		else if (Q[5]=='/') exit(0);

		Delayer("6.Beneath these walls, which of the following Zork-dominant\n");
		Delayer("  villages would you come across?");
		Delayer("\n(A)Hogsmede\t(B)Village_Tantra\n(C)Darpa_Village\t(D)Medelin\n");
		cin>>Q[6];
		if (Q[6]=='C'||Q[6]=='c')	Score+=4;
		else if (Q[6]=='/') exit(0);

		Delayer("7.The name of the forest directly below the fortified coastal");
		Delayer("  walls of the city of Ureka is?");
		Delayer("\n(A)DeadDagger_Woods\t(B)Ureka_Forest\n(C)Nottingham_Forest\t(D)Navada_Woods\n");
		cin>>Q[7];
		if (Q[7]=='A'||Q[7]=='a')	Score+=4;
		else if (Q[7]=='/') exit(0);

		Delayer("8.Name of the recently erected active volcano in the middle");
		Delayer("  of Continent Redland is....");
		Delayer("\n(A)Mount Vesuvius\t(B)Mount Furore\n(C)Havoc Mountain\t(D)Mount Exodus\n");
		cin>>Q[8];
		if (Q[8]=='D'||Q[8]=='d')	Score+=4;
		else if (Q[8]=='/') exit(0);

		Delayer("9.Which of the following races is the best when it comes to\n");
		Delayer("  Technological Advancement?");
		Delayer("\n(A)Humans\t(B)Quazarks\n(C)Zorks\t(D)Elves\n");
		cin>>Q[9];
		if (Q[9]=='C'||Q[9]=='c')	Score+=4;
		else if (Q[9]=='/') exit(0);

		Delayer("10.Which of the following races is the best when it comes to\n");
		Delayer("  Pure Wizardry Skills?");
		Delayer("\n(A)Ogres\t(B)Quazarks\n(C)Humans\t(D)Elves\n");
		cin>>Q[10];
		if (Q[10]=='B'||Q[10]=='b')	Score+=4;
		else if (Q[10]=='/') exit(0);
		getch();

		clrscr();
		Delayer("Sir_Javelin: Hmm.....You've answered "); cout<<Score/4;
		Delayer(" of your answers correctly....\n");
		Delayer("             H E N C E.......\n");
		if (Score<20)
		{
			Delayer("             Y O U   S H A L L   N O T   P A S S !! \n\n\t");
			fl=getch();
			if (fl=='/') exit(0);
			clrscr();
			Delayer("\t   It seems you could't enter the city to join the \n");
			Delayer("\t   Tournament, atleast not legally.... Its not GAME\n");
			Delayer("\t   OVER YET! We can sneak through the eastern side\n");
			Delayer("\t   of the gate and slip into the narrow path which\n");
			Delayer("\t   will lead us to the eastern coastal gates of the city\n");
			Delayer("\t   There's a way in through there, many Smugglers use that passage\n");
			Delayer("\t   (Press anything to Try to enter the city illegally...)\n\n");
			fl=getch();
			if (fl=='/') exit(0);
			clrscr();
			Delayer("\t                      *DeadDagger_Woods*              \n");
			Delayer("\t   To get to the Eastern Coastal, you are now passing through\n");
			Delayer("\t   the DeadDagger_Woods. After walking for a while, you hear a bash\n");
			Delayer("\t   from the base of the coastal walls a few metres away. There's a \n");
			Delayer("\t   teenage girl, trying to climb up the coastal walls, which are\n");
			Delayer("\t   about 30 metres tall. She is fair and blonde with a long\n");
			Delayer("\t   ponytail. Her clothes are that of a male fighter - light\n");
			Delayer("\t   copper armour with a long pant made of cheap fibre.\n");
			Delayer("\t   She had a bow and a quiver with arrows, and also carries two\n");
			Delayer("\t   daggers on her waist. After looking for a while, you realize \n");
			Delayer("\t   that, although her attempts of climbing up the wall are futile,\n");
			Delayer("\t   she just isn't giving up! You then approach her to give her a hand. \n\n");
			fl=getch();
			GM.Activate_Sylvia();
			GM.level=3;
			Update();
			if (fl=='/') exit(0);
		  LVL_3:
			Delayer("SYLVIA: Stop right there, before you make force my Daggers!\n");
			Delayer("YOU:    Oh don't mind me! I was just trying to get into the Crib.\n");
			Delayer("SYLVIA: Sir_Javelin didn't let you in either, huh? Good....\n");
			Delayer("SYLVIA: you can be of aid to me, just don't do anything stupid...\n");
			Delayer("(A)Right....don't push it, princess\t(B)Ok, as long as you follow the same....\t\n(C)Of Coarse.... consider me your Slave\t(D)uhmm.... how 'bout NO!\n");
			cin>>Q[11];
			if (Q[11]=='B'||Q[11]=='b')
			{
				GM.Scr_Add_Five();
				Delayer("SYLVIA: Great! we're a team now....Give me a Lift, so I can grab\n");
				Delayer("SYLVIA: onto that ledge, I'll pull you up from there...\n");
			}
			else if (Q[11]=='A'||Q[11]=='a'||Q[11]=='D'||Q[11]=='d')
			{
				GM.Scr_Sub_Five(); GM.Min_Sylvia();
				Delayer("SYLVIA: Yaa, like you've got a better chance without me.....\n");
				Delayer("YOU:    Touche....But we're not friends...so act professional.\n");
				Delayer("SYLVIA: WILL DO,KING-ATITUDE! Now, gimme a Boost so I can grab onto that ledge.\n");
			}
			else if (Q[11]=='C'||Q[11]=='c')
			{
				GM.Scr_Sub_Ten(); GM.Min_Sylvia(); GM.Min_Sylvia(); GM.Min_Sylvia();
				Delayer("SYLVIA: ButterCups like you are gonna come and go....Don't\n");
				Delayer("SYLVIA: EVER think that I'll give into your fake Loyalty display.\n");
				Delayer("SYLVIA: NOW, gimme a Boost so I can grab onto that ledge.\n");
			}
			else if (Q[11]=='/') exit(0);
			GM.level=17;
			Update();
			return 17;

		getch();
		}
		else if (Score>=20)
		{
		  NATHAN:
			Delayer("             Y O U   S H A L L   P A S S !! \n\n\t");
			fl=getch();
			if (fl=='/') exit(0);
			clrscr();
			Delayer("\t                           *Darpa_Village*              \n");
			Delayer("\t   You have witfully passed the gates of Titanium Crib! CONGRATS!!\n");
			Delayer("\t   You are now passing through Darpa Village, which lies on your path \n");
			Delayer("\t   to the tournament. This village is a Zork-dominated village, with a\n");
			Delayer("\t   handful of Quazarks.\n");
			Delayer("\t   A few metres ahead, you stubble upon a group of Zorks.\n");
			Delayer("\t   They're all armed with crossbows, fire-swords and Camouflage-attires.\n");
			Delayer("\t   You take out your dagger in nervousness, preparing for the worst.\n");
			Delayer("\t   Just then, a medium-sized Zork approaches you. He drops his\n");
			Delayer("\t   sword and crossbow, signalling you he means no harm..... \n\n");
			fl=getch();
			if (fl=='/') exit(0);
			Delayer("NATHAN: Calm down human, we're all friends here. We don't mean no harm....\n");
			Delayer("YOU:    Well, armed Zorks in a tournament as dangerous as this,\n");
			Delayer("        I'll need more than just a 'We mean no harm'. Are you all in the tournament?\n");
			Delayer("NATHAN: NO, just me. And trust me, the tournament hasn't even started yet.\n");
			Delayer("YOU   : Fair enough. So, why this gathering??\n");
			Delayer("NATHAN: Its good you're here, we could use your help.....\n");
			fl=getch();
			if (fl=='/') exit(0);
			GM.Activate_Nathan();
			GM.level=5;
			Update();
			if (fl=='/') exit(0);

		  LVL_5:
			clrscr();
			Delayer("NATHAN: We have a job for you, take it as your...uhmm....\n");
			Delayer("        Tournament warm-up.....don't worry, I'll owe one later.\n");
			Delayer("YOU   : Yaa OK.... gotta test some of my spells anyway....\n");
			Delayer("NATHAN: Yyeeaaa uhmm.... we don't need your aggression. We want\n");
			Delayer("        to execute this mission with minimum casualties, even \n");
			Delayer("        for our enemies. Force only comes as our last resort.\n");
			Delayer("YOU   : What do you want me to do then??\n");
			Delayer("NATHAN: We want your stealth skills. We Zorks, with our attatched\n");
			Delayer("        equipments are the last thing you need when it comes \n");
			Delayer("        down to pure stealth. You humans are excellent at it\n");
			Delayer("        ....or so I've heard. So, are you up for it??\n");
			Delayer("\t(A) Any money Hot-Shot?? I don't come free.....\n");
			Delayer("\t(B) Yaa I'm up for it, but I'd sure as hell want to know what I'm walking into...\n");
			Delayer("\t(C) OKEY_DOKEY....NO PROBLEM !! THE CHAMP IS HERE....\n");
			cin>>Q[12];
			if (Q[12]=='A'||Q[12]=='a')
			{
				GM.Scr_Sub_Five(); GM.Min_Nathan();
				Delayer("NATHAN: Like I said, I'd owe you one. If that doesn' satisfy you...\n");
				Delayer("      : I'd pay you in gold coins....How bout that??\n");
				Delayer("YOU   : That sounds like a deal....OK Amigo, Lets go....\n");
			}
			else if (Q[12]=='B'||Q[12]=='b')
			{
				GM.Scr_Add_Five(); GM.Plus_Nathan();
				Delayer("NATHAN: Great!! Ofcourse we'll brief you on our way....\n");
				Delayer("      : Just be careful, the job demands high-concentration...\n");
				Delayer("YOU   : Sounds challenging, I'm up for it....\n");
			}
			else if (Q[12]=='C'||Q[12]=='c')
			{
				GM.Scr_Sub_Five();
				Delayer("NATHAN: Great!! You sound too confident, hot-shot...\n");
				Delayer("      : You'll have to be briefed first, you know that, right??\n");
				Delayer("YOU   : It'll be easy-peasy, I've done a lot of these in my country...\n");
				Delayer("NATHAN: Just be careful, the job demands high-concentration...\n");
			}
			else if (Q[12]=='/') exit(0);
			GM.level=6;
			Update();
			return 4;


		getch();
		}
	}
	else
	{
	  LVL_9:
		ORNLU();
		GM.level=10;
		Update();

	  LVL_10:
		clrscr();
		GM.Activate_Buna();
		Delayer("\t  **********************UREKA_CITY********************\n");
		Delayer("\t  You have reached the city of Ureka, The capital of this continent !\n");
		Delayer("\t  There is still time to kill, you are a day early....\n");
		Delayer("\t  Ofcourse! You say, as you notice the bar down the alley.\n");
		Delayer("\t  It looks welcoming..... \n");
		fl=getch();
		if (fl=='/') exit(0);
		Delayer("\t  Inside the bar, you see dark Polar sitting right next to you.\n");
		Delayer("\t  You can say he is kind of an introvert, as he seems to be fuzzing\n");
		Delayer("\t  around, trying to break the ice. He's about 7 feet tall, and has \n");
		Delayer("\t  a scar on his shoulder. Seeing his failed attempts to start a\n");
		Delayer("\t  conversation, you take the initiative, and begin with that scar...\n");
		fl=getch();
		if (fl=='/') exit(0);

		clrscr();
		Delayer("YOU  : There is a story behind that scar, I want to hear it....\n");
		Delayer("BUNA : Oh you mean this one up here (pointing to his shoulder)?\n");
		Delayer("       I was riding up the hill from the west, yes I'm a Western Polar,\n");
		Delayer("       I stumbled upon a bunch of no good Quazarks trying to bully\n");
		Delayer("       a poor little Elf. The elf was tough, but the Quazarks are, well...\n");
		Delayer("       QUAZARKS ! Just as they were about to end the elf, I hammered in\n");
		Delayer("       and cracked one of them skulls open...HAHAA! They tried their\n");
		Delayer("       spells, but it only slowed me down. I beat the others up till\n");
		Delayer("       They ran away...HAHAA (sips beer) The elf paid me, so now I'm here...\n");
		Delayer("       Ohh the scar, I got it as I bruised past this damn piece of wood\n");
		Delayer("       for a door.... HAHAA !! what about you?? whats your story?\n");
		fl=getch();
		if (fl=='/') exit(0);

		Delayer("YOU       : Well me? I.....\n");
		Delayer("( You are interrupted by a big-drunk Zork who pushed you away....\n");
		Delayer("DRUNK_ZORK: Ge ...Get out of my seat be...before I do it myself\n");
		Delayer("( As you give in to the big man's orders, A big hand punches the drunk )\n");
		Delayer("BUNA      : Thats no way to talk to a participant! AARRGGHH\n");
		Delayer("( The two of them fight like Two dinosaurs over food !! )\n");
		Delayer("(A) HELP_OUT BUNA                 (B) WATCH THE SHOW\n");
		cin>>Q[12];
		if (Q[12]=='A'||Q[12]=='a')
		{
			GM.Scr_Add_Five(); GM.Plus_Buna();
			Delayer("YOU   : I'm swooping in too, whoever you are...HAHAA....\n");
			Delayer("BUNA  : Plenty of room for punches friend, just land one! \n");
			Delayer("ZORK  : AARRGGHHH...OUCH AAHHH!! STOP IT !! I YIELD!!...\n");
		}
		if (Q[12]=='B'||Q[12]=='b')
		{
			GM.Scr_Sub_Five(); GM.Min_Buna();
			Delayer("BUNA  : You want to join in the fun, huh amigo??\n");
			Delayer("YOU   : YYEEAA uhmm... I'll just, be the lookout \n");
			Delayer("      : just in case the owner comes in....\n");
			Delayer("BUNA  : suit yourself, but you're missing in on a lot of fun !!\n");
			Delayer("ZORK  : AARRGGHHH...OUCH AAHHH!! STOP IT !! I YIELD!!...\n");
		}
		Delayer("BUNA  : Lets get out of here, I had a fight here once before...\n");
		Delayer("      : the owner will recognize me.... \n");
		Delayer(" ( Both of you leave the bar, and head for the Coastal walls )\n");
		fl=getch();
		if (fl=='/') exit(0);
		GM.level=11;
		Update();
		return 11;
	}

}

int Act_II(int con)
{
clrscr();

	int nat_scr, nt_scr, scr_vn;
	if (con==4)      goto LVL_6;
	else if (con==5) goto LVL_7;
	else if (con==6) goto LVL_8;
	else if (con==11) goto LVL_11;
	else if (con==12) goto LVL_12;
	else if (con==13) goto LVL_13;
	else if (con==17) goto LVL_17;
	else if (con==18) goto LVL_18;


  LVL_17:
	scr_vn=Vines();
	if (scr_vn<125) GM.Scr_Add_Ten();
	GM.level=18;
	Update();

  LVL_18:
	clrscr();
	Delayer("******************************UREKA_CITY******************************\n");
	Delayer("SYLVIA: HUH....we made it, and we're a day early !! \n");
	Delayer("<    >: Stop right there.....you can't just sneak into this city like this...\n");
	Delayer("SYLVIA: well I just did, and who might you be....tough guy ? \n");
	Delayer("BUNA  : The name's Buna, and I'm going to take you to the authorities.....\n");
	Delayer("YOU   : Now, now... lets all discuss it through, we mean no harm.......\n");
	Delayer("SYLVIA: I don't think he has the guts..... \n");
	Delayer("BUNA  : Don't make me hurt you ponytail.....I can be.....\n");
	Delayer("( He is interrupted by a kick to the face.......)\n");
	Delayer("SYLVIA: Don't ever call me that..... \n");
	Delayer("BUNA  : Ohh....ITS ON PRINCESS......AAARRGHHH !!\n");
	Delayer("( Both charge at each other like two Caveliers with lances! )\n");
	Delayer("( Buna's a 7 feet tall black-furred Polar....so he seems to )\n");
	Delayer("( have the advantage, but no....its Sylvia who is actually landing the blows!)\n");
	Delayer("(A) Order popcorn from the adjacent store (B) Stop them\n");
	GM.Activate_Buna();
	fl=getch(); if (fl=='/') exit(0);
	else if (fl=='a'||fl=='A')
	{
		GM.Min_Sylvia();
		Delayer("( Both fight till they have blood on their faces.... )\n");
		Delayer("( Sylvia finally holds Buna in a submissive position )\n");
		Delayer("BUNA  : I, I yield....I YIELD !!\n");
		Delayer("SYLVIA: yea.... get up big guy......(Sylvia helps Buna get up.)\n");
		Delayer("BUNA  : You may join the tournament, do whatever you like \n");
		Delayer("        just stay out of my way.....girl.\n");
		Delayer("YOU   : Hey hey wait, I got a proposal.....We all should team up!!\n");
		Delayer("SYLVIA: Are you kidding me.....\n");
		Delayer("YOU   : Hear me out, Lets go to that bar, We'll discuss there....\n");
	}
	else if (fl=='b'||fl=='B')
	{
		GM.Plus_Sylvia(); GM.Plus_Sylvia(); GM.Plus_Buna();
		Delayer("YOU   : wait...stop (You stand right between them)\n");
		Delayer("( Sylvia stops, but Buna couldn't stop his momentum )\n");
		Delayer("( and crashes into you, injuring your elbow...\n");
		Delayer("BUNA  : You shouldn't have.....are you alright?\n");
		Delayer("SYLVIA: Of course he's not....lets take him to that bar...\n");
		Delayer("        get him some bandages there....\n");
		Delayer("BUNA  : I'm coming too.... Its all your fault, you know that right\n");
		Delayer("YOU   : OHH BOTH OF YOU, SHUT UP......I've got something important to say. \n");
		Delayer("        I'm thinking of assembling a team you two seem perfect for it!\n");
	}
	fl=getch(); if (fl=='/') exit(0);
	clrscr();
	Delayer("**********************************BAR*********************************\n");
	Delayer("SYLVIA: This team thing, you were joking, right? \n");
	Delayer("YOU   : NOPE.....\n");
	Delayer("BUNA  : You know the rules for teams are different, right?\n");
	Delayer("        I mean, we have double the tasks, with more difficulty.....\n");
	Delayer("YOU   : YES.....\n");
	Delayer("SYLVIA: Not to mention, we all gotta share the same prize money...\n");
	Delayer("YOU   : I'm here to be an official mage, not for the money....You can \n");
	Delayer("        have my share of the money..... \n");
	Delayer("SYLVIA: That is not what I meant.....\n");
	Delayer("YOU   : So, are you guys in this, or not? \n");
	Delayer("BUNA  : The hell.....I'M IN, What good am I alone anyway...\n");
	Delayer("YOU   : Sylvia...? \n");
	Delayer("SYLVIA: This is all new to me, I mean, I never even talked to anyone in this\n");
	Delayer("        Tornament, let alone make a team.....\n");
	Delayer("YOU   : no harm in trying new things.....\n");
	Delayer("SYLVIA: Fine, I'll ride along, but that doesn't make us friends....\n");
	Delayer("        nor do I have to follow orders or something.....\n");
	Delayer("YOU   : Its a deal then.... lets start our adventure from... any suggestions?\n");
	Delayer("SYLVIA: Lets buy some tech from the Zorks in Darpa village....\n");
	Delayer("YOU   : To DARPA THEN.... LETS GO..!!\n");
	Delayer("( And just like that, your little 'squad' is now heading towards DARPA.\n");
	GM.Plus_Sylvia(); GM.Plus_Buna();
	fl=getch(); if (fl=='/') exit(0);
	GM.level=12;
	GM.coast=1;
	Update();
	goto LVL_12;

	getch(); exit(0);

  LVL_6:
	nat_scr=Princess_Heather();
	GM.Plus_Nathan();
	cout<<nat_scr; getch();
	if (nat_scr==0)      { GM.Scr_Add_Ten(); GM.Scr_Add_Ten(); GM.Scr_Add_Ten(); }
	else if (nat_scr<=3) { GM.Scr_Add_Ten(); }
	else if (nat_scr>3)  { GM.Scr_Add_Five(); }
	GM.level=7;
	Update();

  LVL_7:
	clrscr();
	Delayer("LOCAL_ZORKS: Thank You Mage, these Quazarks are being really mean.\n");
	Delayer("             They took our stockpiles and set our homes on fire.They\n");
	Delayer("             had it coming, thanks to a talented wizard, such as \n");
	Delayer("             yourself.... Here, take this as a token of our gratitude !\n");
	getch();
	Delayer("(YOU HAVE RECEIVED A PHASE CHANGER........)\n");
	Delayer("HEATHER    : This is a Phase Changer, it can change the state of \n");
	Delayer("             matter of the surface it is on. Use it to get through\n");
	Delayer("             any opaque wall or hurdle. Good Luck !!\n");
	Delayer("(A)THANK_YOU PRINCESS (B)YEA_YEA, GIVE THE DAMN STUFF ALREADY... \n");
	cin>>Q[13];
	if (Q[13]=='A'||Q[13]=='a')
	{
		GM.Scr_Add_Five();
		Delayer("HEATHER    : I should be thanking you.... Best of luck for the Tournament !!\n");
		Delayer("YOU        : It was an honour serving you, Princess....\n");
	}
	else if (Q[13]=='B'||Q[13]=='b')
	{
		GM.Scr_Sub_Five();
		Delayer("HEATHER    : Oooo, aren't you the ideal human....Here, take it. Hope I was useful.\n");
		Delayer("YOU        : Thank you ma'am, I'll be taking that...ADIOS !\n");
	}
	fl=getch(); if (fl=='/') exit(0);
	GM.level=8;
	Update();
	goto LVL_8;

  LVL_11:
	clrscr();
	Delayer("\t*************************UREKA_COASTAL WALLS************************\n");
	Delayer("YOU : Ahh, the view! Its magnificent!\n");
	Delayer("BUNA: Not as magnificent as how you beat up that drunk Zork, hahhaa\n");
	Delayer("YOU : HAHAA, right......wait, who's that??\n");
	Delayer("BUNA: I see her too, some blonde trying to get into the tournament....\n");
	Delayer("( Both of you spot Sylvia, the teenage fighter, who's an excellent archer! )\n");
	GM.Activate_Sylvia();
	Delayer("BUNA: I'll put a stop to that...........\n");
	Delayer("YOU : No wait, I myself think the quiz was too hard.... If she wants to\n");
	Delayer("    : join so bad, we shouldn't stop her....\n");
	Delayer("BUNA: You're innocent, the quiz was meant to be tough, to omit out potential terrorists...\n");
	Delayer("(A) Agree Buna's argument      (B)Disagree\n");
	cin>>Q[1];
	if (Q[1]=='A'||Q[1]=='a')
	{
		GM.Plus_Buna(); GM.Min_Sylvia();
		Delayer("BUNA  : You there, turn around and go back the way you came from.....\n");
		Delayer("SYLVIA: Raaiight, and you are, exactly?? lemme guess, no one??\n");
		Delayer("BUNA  : I don't like mockers....Now get out before I become a threat! \n");
		Delayer("YOU   : Hey, don't hit girls, although we may have to once the tournament begins...\n");
		Delayer("BUNA  : I'm not going to hit her..... I'll just give her a scare....\n");
		Delayer("BUNA  : (turns to Sylvia) ARRRGHHHHH......\n");
		Delayer("( Sylvia lands a big blow on Buna's face, Buna traumatized...\n");
		Delayer("( As Buna tries to fight back, Sylvia jump kicks on his face....\n");
		Delayer("( and performs a submissive move......\n");
		Delayer("SYLVIA: How you like me now, big guy?? \n");
		Delayer("BUNA  : I...I yield, I YIELD !! Jesus, girl !! \n");
		Delayer("SYLVIA: (Releases Buna) OK, lets start new, hey you, whats your name?\n");
		Delayer("YOU   : "); Delayer(GM.Show_Name());
		Delayer("SYLVIA: .....and you tough guy??\n");
		Delayer("BUNA  : Go...go to hell... \n");
		Delayer("YOU   : He's Buna, he doesn't like losing, or so I think, I don't know\n");
		Delayer("YOU   : for sure, We just met....\n");
	}
	else if (Q[1]=='B'||Q[1]=='b')
	{
		GM.Min_Buna(); GM.Plus_Sylvia();
		Delayer("BUNA  : You there, turn around and go back the way you came from.....\n");
		Delayer("YOU   : Hey, hey, give her a chance, OK! I know what it feels\n");
		Delayer("        like when you're not given a chance to prove yourself. \n");
		Delayer("BUNA  : I can't just let strangers into this city, on my watch!\n");
		Delayer("YOU   : I say we talk, take care of this in a civilized manner....\n");
		Delayer("BUNA  : OK, but if she's fishy, I blame you!\n");
		Delayer("( Sylvia Climbs onto the city walls, jumps down, lands infront )\n");
		Delayer("YOU   : Why the hard way in, when you can just study a little....\n");
		Delayer("SYLVIA: I'm here to be a mage, not a scholar....\n");
		Delayer("YOU   : I'm "); Delayer(GM.Show_Name());
		Delayer("        by the way, and you??\n");
		Delayer("SYLVIA: huh.... what's with names, we're gonna fight each other anyway...\n");
		Delayer("YOU   : Not, if we make teams, the tournament allows teams...\n");
		Delayer("SYLVIA: Sylvia, its Sylvia, whats that guy's name....?\n");
		Delayer("BUNA  : oh uhmm....Bu, Buna. Its Buna.\n");
	}
	else if (Q[1]=='/') exit(0);
	getch();

	clrscr();
	Delayer("YOU   : So Sylvia, what brings you here, Whats your story....\n");
	Delayer("BUNA  : Ahh c'mon, we don't have time to make friends now\n");
	Delayer("        We should be professional.....\n");
	Delayer("SYLVIA: Why do you want it, why are you trying to make friends?\n");
	Delayer("        Are you new to this tournament? We don't make friends here.\n");
	Delayer("(A) Ask for back-story anyway.    (B)Let the matter slide.\n");
	cin>>Q[1];
	if (Q[1]=='A'||Q[1]=='a')
	{
		Delayer("YOU   : I'm, just trying to make conversation, alright.\n");
		Delayer("        The tournaments a day later....\n");
		Delayer("        I say, we be on our way to, lets say west, look for an adventure,\n");
		Delayer("        while we all tell our stories on the way.....\n");
		Delayer("BUNA  : Well that won't hurt..... I'm in.\n");
		Delayer("SYLVIA: You two, with that much of innocence are gonna be the first ones\n");
		Delayer("        to get eliminated, I tell you....This tournaments dangerous! \n");
		Delayer("        TAKE IT SERIOUSLY....!! \n");
		Delayer(" ( BOTH YOU AND BUNA GIVE HER THE PLAIN FACE LOOK ) \n");
		Delayer("SYLVIA: Alright Fine!!.... Here goes......\n");
		GM.Plus_Sylvia(); GM.Plus_Buna(); GM.Plus_Sylvia();
	}
	Delayer("\n\n( Your little group advances towards Darpa_Village )\n");
	fl=getch();
	if (fl=='/') exit(0);
	GM.level=12;
	Update();

  LVL_12:
	clrscr();
	Delayer("( As your group walks through the dense trees, just a )\n");
	Delayer("( few hours before you reach Darpa, you come accross a )\n");
	Delayer("( bunch of Zorks, armed with crossbows and fire-swords.)\n");
	Delayer("( A medium sized Zork without weapons approaches you...)\n");
	fl=getch(); if (fl=='/') exit(0);
	Delayer("NATHAN: Thank god....we need your help...\n");
	Delayer("SYLVIA: Whats the matter?\n");
	Delayer("NATHAN: Our Zork princess Heather has been kidnapped by a bunch of Quazarks....\n");
	Delayer("      : She's being held Hostage in the black house over there....\n");
	Delayer("SYLVIA: We need to help them guys......\n");
	Delayer("BUNA  : It may be a trap, can't risk it....\n");
	Delayer("SYLVIA: ZORKS DON'T LIE, and the tournament hasn't even begun yet....\n");
	Delayer("      : This is the Adventure you were looking for, "); Delayer(GM.Show_Name());
	Delayer("\nYOU   : She's right Buna, we need to....\n");
	Delayer("( A LARGE BLAST INTERRUPTS YOU, A BUNCH OF QUAZARKS ARE HEADING YOUR WAY )\n");
	Delayer("SYLVIA: Buna and I along with these Zorks can handle them, you go\n");
	Delayer("      : Save the princess......GO !");
	fl=getch(); if (fl=='/') exit(0);

	nt_scr=Princess_Heather();
	GM.Plus_Nathan(); GM.Plus_Sylvia();
	cout<<nt_scr; getch();
	if (nt_scr==0)      { GM.Scr_Add_Ten(); GM.Scr_Add_Ten(); GM.Scr_Add_Ten(); }
	else if (nt_scr<=3) { GM.Scr_Add_Ten(); }
	else if (nt_scr>3)  { GM.Scr_Add_Five(); }
	GM.level=13;
	Update();

  LVL_13:
	clrscr();
	Delayer("( You come back with the princess to see a bunch of dead Quazarks and Zorks....)\n");
	Delayer("( Buna, Sylvia and Nathan are perfectly fine....)\n");
	Delayer("YOU     : Are you guys alright? It must've gotten pretty messy here... \n");
	Delayer("SYLVIA  : You bet...(turns to princess and bows) Princess....\n");
	Delayer("( Buna and Nathan bow down too )\n");
	Delayer("HEATHER : You don't have to, these innocent Zorks died because \n");
	Delayer("          of me....\n");
	Delayer("NATHAN  : They died honourably, princess. \n");
	Delayer("HEATHER : I, I need to thank you all for such an act of bravery.\n");
	Delayer("          Here, take this as a token of my gratitude....\n");
	fl=getch(); if (fl=='/') exit(0);
	Delayer("(YOU HAVE RECEIVED A PHASE CHANGER........)\n");
	Delayer("HEATHER    : This is a Phase Changer, it can change the state of \n");
	Delayer("             matter of the surface it is on. Use it to get through\n");
	Delayer("             any opaque wall or hurdle. Good Luck !!\n");
	fl=getch(); if (fl=='/') exit(0);
	Delayer("( you all thank the princess and go towards Ureka )\n");
	Delayer("( Nathan comes running in from the back.... )\n");
	getch();

	clrscr();
	fl=getch(); if (fl=='/') exit(0);
	Delayer("NATHAN  : (breathes heavily), yo,you know I'm in the tournament too, right \n");
	Delayer("NATHAN  : can I come along too? I can be of great help.... \n");
	Delayer("YOU     : well, more the better....ride along, ZORK!\n");
	Delayer("( with that, your little group just got a little bigger )\n");
	Delayer("( Now you all head back to Ureka city to get your first set of tasks! )\n");
	fl=getch(); if (fl=='/') exit(0);
	GM.Activate_Nathan(); GM.level=14;
	Update();
	return 14;

  LVL_8:
	clrscr();
	Delayer("NATHAN: It seems we both are headed towards Ureka now......\n");
	Delayer("YOU   : yea....this forrest gives me the creeps, though....\n");
	Delayer("( DISTANT SCREAMING VOICE )\n");
	Delayer("NATHAN: What was that......\n");
	Delayer("YOU   : Someone in trouble maybe....lets go find out!\n");
	fl=getch(); if (fl=='/') exit(0);

	clrscr();
	Delayer("************************************ORNLU_FOREST********************************\n");
	Delayer("( You reach the location only to find an unconcious body of a\n");
	Delayer("  female Quazark......and another Quazark just standing there...\n");
	Delayer("YOU   : Don't just stand there....DO SOMETHING!!\n");
	Delayer("RAVEN : AAHH, I'm Raven, you must be....."); Delayer(GM.Show_Name()); cout<<".\n";
	Delayer("YOU   : How did you know my name.....\n");
	Delayer("RAVEN : Time is linear to me, I'm 600 years old, I'm one of the \n");
	Delayer("        survivors of the third Havoc...and blah blah blah.... \n");
	Delayer("        We can talk later, lets first get to work. \n");
	Delayer("        I want you to Frost this girl. So I can slow down her \n");
	Delayer("        heart's perception of time, so as to break into her body\n");
	Delayer("        and take her powers.....\n");
	Delayer("NATHAN: WOW........he talks !\n");
	Delayer("YOU   : NO I WON'T, you should leave her alone.....\n");
	Delayer("RAVEN : You don't know what she is. We, we are good friends,\n");
	Delayer("        you may not know this now, but we're a team.\n");
	Delayer("        All you gotta do now is listen to me....Do as I say.....\n");
	Delayer("YOU   : Thats your best approach to convince me? not happening...\n");
	Delayer("RAVEN : You leave me no choice.....\n");
	fl=getch(); if (fl=='/') exit(0);

	ALX();
	clrscr();
	GM.Activate_Alexis();
	Delayer("RAVEN : AARRRLLLCCC.....YOU HAVN'T SEEN THE LAST OF ME....\n");
	Delayer("NATHAN: yeaa....you better run.....\n");
	Delayer("( Female Quazark slowly gets up, body still weak.....)\n");
	Delayer("ALEXIS: Thanks for saving me, again....."); Delayer(GM.Show_Name()); cout<<"...\n";
	Delayer("YOU   : Am I famous here or something...how do all of you...\n");
	Delayer("        ......wait, what do you mean, 'again'...???\n");
	Delayer("ALEXIS: There are infinite sets of timelines created on the decisions you make.\n");
	Delayer("        In the one I'm in, you saved my life countless times.... we are Mages.\n");
	Delayer("YOU   : WHATT...Really?? I, I'm a Mage....\n");
	Delayer("ALEXIS: Depends on you and your choices, in Raven's timeline, you are an evil\n");
	Delayer("        Quazark.....corrupting Galactra from the shadows...\n");
	Delayer("YOU   : WHO, ME?? How did that happen.....\n");
	Delayer("ALEXIS: LONG STORY SHORT....YOUR LIFE JUST GOT A LOT MORE INTERESTING !\n");
	fl=getch(); if (fl=='/') exit(0);
	GM.level=21;
	Update();
	return 21;

}


void Act_III(int con)
{
clrscr();

	int rv_scr;
	if (con==14) { if (GM.coast==1) goto LVL_19; else goto LVL_14; }
	else if (con==15) goto LVL_15;
	else if (con==16) goto LVL_16;
	else if (con==19) goto LVL_19;
	else if (con==20) goto LVL_20;
	else if (con==21) goto CREDITS;


  LVL_19:

	clrscr();
	Delayer("On your way to city Ureka, you and your little 'team' all decided to \n");
	Delayer("camp the night, to start fresh in the morning....\n");
	fl=getch(); if (fl=='/') exit(0);
	Delayer("\n********************************CAMPING*******************************\n\n");
	Delayer("NATHAN: .......and then the old fat zork fell off his chair....HAAHAA !!\n");
	Delayer("BUNA  : HAAHAAHAAA......OOuuu that was hilarious, especially the tree part!\n");
	Delayer("YOU   : Nice one there, Nathan.\n");
	Delayer("SYLVIA: Am I the only one taking this tournament seriously?? You know how many\n");
	Delayer("        wolves reside in this forrest....you all will get yourselves KILLED!\n");
	Delayer("BUNA  : Chill out Sylvy, or are you new to the word? HAHAA...\n");
	Delayer("SYLVIA: Ohh tough boy, you call me that one more time, and I...\n");
	Delayer("YOU   : sshhhh.....I hear something from the bushes.\n");
	Delayer("NATHAN: yea, my radar's beeping too. We aren't alone. Keep it quiet...\n");
	Delayer("(You take out your dagger,Nathan his sword,Sylvia her bow and Buna his knucles)\n");
	fl=getch(); if (fl=='/') exit(0);
	Delayer("<    >: Stop, don't, I, don't shoot...I, I got urgent news....\n");
	Delayer("BUNA  : and how do we know its not a trap.....\n");
	Delayer("<    >: Because I know everything about you all.... and I'm here to help.\n");
	Delayer("SYLVIA: Help? I've seen these tricks before last year....what's your story...\n");
	Delayer("<    >: Same as any other girl, Sylvia, trying to run away from prejudices,\n");
	Delayer("        joining this tournament to prove a point, help the weak from bullies.\n");
	Delayer("SYLVIA: How, how'd you know....my.....\n");
	Delayer("ALEXIS: The same way I know Nathan's, Buna's and "); Delayer(GM.Show_Name()); Delayer("'s names.....\n");
	Delayer("NATHAN: I don't get this at all....are you using some kind of spell?\n");
	Delayer("ALEXIS: We'll have plenty of time to talk later... \nbut right now, we need to leave....\n");
	Delayer("ALEXIS: ORNLU THE WOLF IS HERE, IN UREKA_COUNTY !!\n");
	Delayer("BUNA  : Ornlu the who ??\n");
	Delayer("NATHAN: Ornlu the wolf, destroyer of the third civilizatoin!!\n");
	Delayer(" ( ORNLU THE WOLF HOWLS !! )\n");
	fl=getch(); if (fl=='/') exit(0);
	Delayer("ALEXIS: There's no time, we need to....\n");
	Delayer("( Ornlu the wolf crashes in and grabs your leg with its fangs...)\n");
	Delayer("ALEXIS: "); Delayer(GM.Show_Name()); Delayer("...!!!");
	Delayer("BUNA  : NNOOOOO.....\n");
	Delayer("(You start fainting due to the intense pain....You pass out....)");
	fl=getch(); if (fl=='/') exit(0);
	GM.level=20;
	Update();


  LVL_20:

	clrscr();
	Delayer("(Next morning you wake up, only to find yourself in a prison...)\n");
	Delayer("YOU: Am I not dead?? Why am I here? Where am I? Where's the beast?\n");
	Delayer("YOU: OHH no, I'm going to be late for the tournament!! How do I get out?\n");
	Delayer("(Many hawling sounds made outside...You look out through the window)\n");
	Delayer("YOU: Are those....ORNLU'S followers.....RED_WOLVES..!! I gotta run !\n");
	Delayer("     But, but how the hell do I get out of this cell ?\n");
	Delayer("(Too many questions in your mind.....but you have a solution....USE IT!)\n");
	Delayer("(Press 'p' to use Phase Changer....)\n");
	fl=getch();
	if (fl=='/') exit(0);
	else if (fl=='p'||fl=='P') rv_scr=River_Dale(12); getch();
	if (rv_scr>50) GM.Scr_Add_Ten();
	else if (rv_scr>100) { GM.Scr_Add_Ten(); GM.Scr_Add_Ten(); }
	else if (rv_scr>125) { GM.Scr_Add_Ten(); GM.Scr_Add_Ten(); GM.Scr_Add_Ten(); }
	else if (rv_scr>150) { GM.Scr_Add_Ten(); GM.Scr_Add_Ten(); GM.Scr_Add_Ten(); GM.Scr_Add_Ten(); }

	clrscr();
	Delayer("********************************UREKA_CITY**********************************\n");
	Delayer("SYLVIA: "); Delayer(GM.Show_Name()); Delayer("...!!!\n");
	Delayer("NATHAN: You're ALIVE!! thank god, where were you...??\n");
	Delayer("BUNA  : ( BUNA GIVES A BIG HARD HUG......) BUUDDDYY !!\n");
	Delayer("ALEXIS: We were searching all night, we thought if you survived, you'd \n");
	Delayer("        come to Ureka.... So we all hoped for the best and came here.\n");
	Delayer("YOU   : How did you know I may survive, I mean, Ornlu took me...\n");
	Delayer("ALEXIS: There are secrets you are not ready to hear yet....Ornlu took \n");
	Delayer("        you, and not us for a reason.....\n");
	fl=getch(); if (fl=='/') exit(0);

	Delayer("SYLVIA: Yaa, Alexis told us everything, how she knew about every- \n");
	Delayer("        thing, why Ornlu wanted you.... \n");
	Delayer("BUNA  : I didn't believe her, untill now, You're not who you are...\n");
	Delayer("YOU   : You, you guys are confusing me!! wha, what am I ??\n");
	Delayer("ALEXIS: You were't food, "); Delayer(GM.Show_Name()); cout<<"\n";
	Delayer("        Ornlu's participating, he wanted you as his partner...\n");
	Delayer("YOU   : Why was he trying to be my partner? \n");
	Delayer("        I'm just a farmer from a poor family!\n");
	Delayer("ALEXIS: No, YOU don't know much about yourself......\n");
	Delayer("        Your name is ...."); Delayer(GM.Show_Name()); Delayer(" Furore !\n");
	Delayer("YOU   : Furo....Fu, but I..... \n");
	Delayer("ALEXIS: Yes.....YOU'RE A QUAZARK ! \n");
	fl=getch(); if (fl=='/') exit(0);
	GM.level=21;
	Update();
	goto CREDITS;





  LVL_14:
	Delayer("On your way to city Ureka, you and your little 'team' all decided to \n");
	Delayer("camp the night, to start fresh in the morning....\n");
	fl=getch(); if (fl=='/') exit(0);
	Delayer("\n********************************CAMPING*******************************\n\n");
	Delayer("NATHAN: .......and then the old fat zork fell off his chair....HAAHAA !!\n");
	Delayer("BUNA  : HAAHAAHAAA......OOuuu that was hilarious, especially the tree part!\n");
	Delayer("YOU   : Nice one there, Nathan.\n");
	Delayer("SYLVIA: Am I the only one taking this tournament seriously?? You know how many\n");
	Delayer("        wolves reside in this forrest....you all will get yourselves KILLED!\n");
	Delayer("BUNA  : Chill out Sylvy, or are you new to the word? HAHAA...\n");
	Delayer("SYLVIA: Ohh tough boy, you call me that one more time, and I...\n");
	Delayer("YOU   : sshhhh.....I hear something from the bushes.\n");
	Delayer("NATHAN: yea, my radar's beeping too. We aren't alone. Keep it quiet...\n");
	Delayer("(You take out your dagger, Nathan his sword, Sylvia her bow, and Buna his knucles)\n");
	fl=getch(); if (fl=='/') exit(0);
	Delayer("<    >: Stop, don't, I, don't shoot...I, I got urgent news....\n");
	Delayer("YOU   : wait, I, recognize that voice.....\n");
	Delayer("ALEXIS: ......"); Delayer(GM.Show_Name()); cout<<"\n";
	if (GM.Alexis==0)
	{
		GM.Activate_Alexis(); GM.Min_Alexis();
		Delayer("YOU   : Alexis! YOU'RE ALIVE....?? HOW ?\n");
		Delayer("ALEXIS: I'll explain everything, but first, you need to pay attention!\n");
	}
	else
	{
		Delayer("YOU   : Alexis! Boy am I glad to see you .....\n");
		Delayer("ALEXIS: There's no time for chit-chat, you need to pay attention!\n");
	}
	Delayer("SYLVIA: You two know each other? Why is everyone here making friends!?\n");
	Delayer("BUNA  : Cuz they ain't you, dummy!!...\n");
	Delayer("SYLVIA: OH ITS ON, BIG_GUY AARGHH.....\n");
	Delayer("( NATHAN creates a force-field between them with his tech )\n");
	Delayer("NATHAN: Didn't you hear the lady, she's got something important to say...\n");
	Delayer("ALEXIS: ORNLU THE WOLF IS HERE, IN UREKA_COUNTY !!\n");
	Delayer("BUNA  : Ornlu the who ??\n");
	Delayer("NATHAN: Ornlu the wolf, destroyer of the third civilizatoin!!\n");
	Delayer(" ( ORNLU THE WOLF HOWLS !! )\n");
	fl=getch(); if (fl=='/') exit(0);
	Delayer("ALEXIS: There's no time, we need to....\n");
	Delayer("( Ornlu the wolf crashes in and grabs your leg with its fangs...)\n");
	Delayer("ALEXIS: "); Delayer(GM.Show_Name()); Delayer("...!!!");
	Delayer("BUNA  : NNOOOOO.....\n");
	Delayer("(You start fainting due to the intense pain....You pass out....)");
	fl=getch(); if (fl=='/') exit(0);
	GM.level=15;
	Update();

  LVL_15:
	int scr_rv;
	clrscr();
	Delayer("(Next morning you wake up, only to find yourself in a prison...)\n");
	Delayer("YOU: Am I not dead?? Why am I here? Where am I? Where's the beast?\n");
	Delayer("YOU: OHH no, I'm going to be late for the tournament!! How do I get out?\n");
	Delayer("(Many hawling sounds made outside...You look out through the window)\n");
	Delayer("YOU: Are those....ORNLU'S followers.....RED_WOLVES..!! I gotta run !\n");
	Delayer("     But, but how the hell do I get out of this cell ?\n");
	Delayer("(Too many questions in your mind.....but you have a solution....USE IT!)\n");
	Delayer("(Press 'p' to use Phase Changer....)\n");
	fl=getch();
	if (fl=='/') exit(0);
	else if (fl=='p'||fl=='P') scr_rv=River_Dale(12); getch();
	if (scr_rv>50) GM.Scr_Add_Ten();
	else if (scr_rv>100) { GM.Scr_Add_Ten(); GM.Scr_Add_Ten(); }
	else if (scr_rv>125) { GM.Scr_Add_Ten(); GM.Scr_Add_Ten(); GM.Scr_Add_Ten(); }
	else if (scr_rv>150) { GM.Scr_Add_Ten(); GM.Scr_Add_Ten(); GM.Scr_Add_Ten(); GM.Scr_Add_Ten(); }

	GM.level=16;
	Update();

   LVL_16:
	clrscr();
	Delayer("********************************UREKA_CITY**********************************\n");
	Delayer("SYLVIA: "); Delayer(GM.Show_Name()); Delayer("...!!!\n");
	Delayer("NATHAN: You're ALIVE!! thank god, where were you...??\n");
	Delayer("BUNA  : ( BUNA GIVES A BIG HARD HUG......) BUUDDDYY !!\n");
	Delayer("ALEXIS: We were searching all night, we thought if you survived, you'd \n");
	Delayer("        come to Ureka.... So we all hoped for the best and came here.\n");
	Delayer("YOU   : How did you know I may survive, I mean, Ornlu took me...\n");
	Delayer("ALEXIS: There are secrets you are not ready to hear yet....Ornlu took \n");
	Delayer("        you, and not us for a reason, the same reason why Raven didn't\n");
	Delayer("        kill you....\n");
	fl=getch(); if (fl=='/') exit(0);

	Delayer("SYLVIA: Yaa, Alexis told us, everything, how she survived, how she \n");
	Delayer("        came to know about you, why Ornlu wanted you.... \n");
	Delayer("BUNA  : I didn't believe her, untill now, You're not who you are...\n");
	Delayer("YOU   : You, you guys are confusing me!! wha, what am I ??\n");
	Delayer("ALEXIS: You were't food, "); Delayer(GM.Show_Name()); cout<<"\n";
	Delayer("        Ornlu's participating, he wanted you as his partner...\n");
	Delayer("YOU   : whats with these people and trying to be my partner, \n");
	Delayer("        Don't they know who I am? I'm just a farmboy from a poor family!\n");
	Delayer("ALEXIS: No, YOU don't know much about yourself......\n");
	Delayer("        Your name is ...."); Delayer(GM.Show_Name()); Delayer(" Furore !\n");
	Delayer("YOU   : Furo....Fu, but I..... \n");
	Delayer("ALEXIS: Yes.....YOU'RE A QUAZARK ! \n");
	fl=getch(); if (fl=='/') exit(0);
	GM.level=21;
	Update();

  CREDITS:
	CREDITS();

getch();
}


void main()
{
clrscr();

	int silo;
	int choice=MAINSCREEN();
	if (choice==5)
		GoodBye();
	else if (choice==4)
	{	MAP();	getch();   exit(0);	}
	else if (choice==1)
	{
	clrscr();

		SaveFiles.open("SAVDAT", ios::ate | ios::binary);
		ReadSaveFiles.open("SAVDAT", ios::in | ios::binary);
		SaveFiles.seekp(0, ios::end);
		int loc=SaveFiles.tellp();
		cout<<"  TELLP()="<<loc;
		getch();
			GM.sl=(loc/sizeof(GM))+1;
			GM.score=0; GM.level=1;
			GM.Sylvia=0; GM.Buna=0; GM.Nathan=0; GM.Alexis=0;
			GM.Get_Name();
			SaveFiles.write((char*)&GM, sizeof(GM));
			ReadSaveFiles.seekg(loc);
			ReadSaveFiles.read((char*)&GM, sizeof(GM));
			cout<<"\nFile no.#"<<GM.sl<<" Created! ";
			getch();
			GM.Show();

		ReadSaveFiles.close();
		SaveFiles.close();
	}
	else if (choice==3)
	{
	clrscr();
		SaveFiles.open("SAVDAT", ios::ate | ios::binary);
		ReadSaveFiles.open("SAVDAT", ios::in | ios::binary);
		ReadSaveFiles.seekg(0);
		while(!ReadSaveFiles.eof())
		{
			ReadSaveFiles.read((char*)&GM, sizeof(GM));
			GM.Show();
		}
		ReadSaveFiles.close();
		SaveFiles.close();
		getch(); 	exit(0);
	}
	else if (choice==2)
	{
	clrscr();

		ReadSaveFiles.open("SAVDAT", ios::in | ios::binary);
		int lvl=0;
		char ctr_name[50];
		cout<<"Enter Name: ";
		gets(ctr_name);
		ReadSaveFiles.seekg(0);
		while(!ReadSaveFiles.eof())
		{
			ReadSaveFiles.read((char*)&GM, sizeof(GM));
			if (strcmpi(GM.Show_Name(),ctr_name)==0)
			{  lvl=GM.level; break;	}
		}
		GM.Show();
		ReadSaveFiles.close();
		if (lvl==1)
		{	feed[1]=Act_I(101); feed[2]=Act_II(feed[1]); }
		else if (lvl==2)
		{	feed[1]=Act_I(102); feed[2]=Act_II(feed[1]); }
		else if (lvl==3)
		{	feed[1]=Act_I(103); feed[2]=Act_II(feed[1]); }
		else if (lvl==4)
		{	feed[1]=Act_I(107); feed[2]=Act_II(feed[1]); }
		else if (lvl==5)
		{	feed[1]=Act_I(105); feed[2]=Act_II(feed[1]); }
		else if (lvl==6)
		{	feed[2]=Act_II(4); clrscr(); cout<<"\n\t"<<feed[2]; getch(); exit(0); }
		else if (lvl==7)
		{	feed[2]=Act_II(5); clrscr(); cout<<"\n\t"<<feed[2]; getch(); exit(0); }
		else if (lvl==8)
		{	feed[2]=Act_II(6); clrscr(); getch(); exit(0); }
		else if (lvl==9)
		{	feed[1]=Act_I(9); Act_II(feed[1]); getch(); exit(0); }
		else if (lvl==10)
		{	feed[1]=Act_I(10); Act_II(feed[1]); getch(); exit(0); }
		else if (lvl==11)
		{	feed[2]=Act_II(11); getch(); exit(0); }
		else if (lvl==12)
		{	feed[2]=Act_II(12); getch(); exit(0); }
		else if (lvl==13)
		{	feed[2]=Act_II(13); clrscr(); cout<<feed[2]; getch(); exit(0); }
		else if (lvl==14)
		{	Act_III(14); clrscr(); getch(); exit(0); }
		else if (lvl==15)
		{	Act_III(15); clrscr(); getch(); exit(0); }
		else if (lvl==16)
		{	Act_III(16); clrscr(); getch(); exit(0); }
		else if (lvl==17)
		{	feed[2]=Act_II(17); clrscr(); getch(); exit(0); }
		else if (lvl==18)
		{	feed[2]=Act_II(18); clrscr(); getch(); exit(0); }
		else if (lvl==19)
		{	Act_III(19); clrscr(); getch(); exit(0); }
		else if (lvl==20)
		{	Act_III(20); clrscr(); getch(); exit(0); }
		else if (lvl==21)
		{	Act_III(21); clrscr(); getch(); exit(0); }

	getch();
	}


New_Game:
	int cont;
	clrscr();
	Delayer("\tTHIS IS JUST A DEMO VERSION, THE STORY LINE IS NOT COMPLETE HERE\n");
	Delayer("\tIT KEEPS YOU IN SUSPENSE AS DESIGNED (IF PAID ATTENTION TO).\n");
	Delayer("\tFOR NOW< JUST RIDE ALONG AND ENJOY THE TEXT ADVENTURE TILL WHEREVER\n");
	Delayer("\tIT TAKES YOU TO. \nTHE GAME WAS DESIGNED BY THE STUDENTS OF DPS-DULIAJAN.\n");
	getch();

	clrscr();
		if (GM.level==1)
	{
		MAP();
		cin>>cont;
		if (cont==1)
			Titanium();
		else if (cont==2)
			Frost();
		else if (cont==3)
			Redland();
		else if (cont==4)
			Linustasia();
		else if (cont==5)
			Dazemberg();
		else if (cont==6)
			Alphagard();
		else if (cont==7)
			Starkgaryen();
		else if (cont==69)
		{	feed[1]=Act_I(cont);	getch();	exit(0);	}
		else if (cont==-69)
			exit(0);
	}
		cout<<"\n\tdoin feed_1....."; getch();
		feed[1]=Act_I(cont);
		feed[2]=Act_II(feed[1]);   getch();
		Act_III(feed[2]); getch();
		clrscr();
		CREDITS();
}

//**************************OBSTACLE_RACE****************************
//  /*

int finalscore;
int by[5], b=0, ay[5], a=0, ctr=0;
int gmr=0;

void LINER()
{
	for (x=1; x<80; x++)
	{	gotoxy(x,21); cout<<" ";   }
}

void BOAT_1(int &);
void BOAT_2(int &);
void BOAT_3(int &);
void BOAT_4(int &);
void BOAT_5(int &);

//  /*
void ARR_1(int &aay)
{
	gotoxy(42,aay);	textcolor(GREEN); cprintf("%c",char(219)); aay-=3;
	if (aay>4)
	{
		gotoxy(42,aay+3);	textcolor(GREEN); cprintf("%c",char(219));
		gotoxy(42,aay);	textcolor(RED); cprintf("%c",char(15));
		land[42][aay+3]=1;
		land[42][aay]=-2;
	}
	else
		aay=17;
}
//  */

void ARR_2(int &aay)
{
	gotoxy(43,aay);	textcolor(GREEN); cprintf("%c",char(219)); aay++;
	if (aay<17)
	{
		gotoxy(43,aay-1);	textcolor(GREEN); cprintf("%c",char(219));
		gotoxy(43,aay);	textcolor(RED); cprintf("%c",char(15));
		land[43][aay-1]=1;
		land[43][aay]=-2;
	}
	else
		aay=4;
}
void ARR_3(int &aay)
{
	gotoxy(44,aay);	textcolor(GREEN); cprintf("%c",char(219)); aay-=2;
	if (aay>4)
	{
		gotoxy(44,aay);	textcolor(RED); cprintf("%c",char(15));
		land[44][aay+2]=1;
		land[44][aay]=-2;
	}
	else
		aay=17;
}
void ARR_4(int &aay)
{
	gotoxy(45,aay);	textcolor(GREEN); cprintf("%c",char(219)); aay+=4;
	if (aay<17)
	{
		gotoxy(45,aay);	textcolor(RED); cprintf("%c",char(15));
		land[45][aay-4]=1;
		land[45][aay]=-2;
	}
	else
		aay=4;
}
void ARR_5(int &aay)
{
	gotoxy(46,aay);	textcolor(GREEN); cprintf("%c",char(219)); aay-=2;
	if (aay>4)
	{
		gotoxy(46,aay);	textcolor(RED); cprintf("%c",char(15));
		land[46][aay+2]=1;
		land[46][aay]=-2;
	}
	else
		aay=17;
}
void ARROW(int a)
{
	if (a!=0)
	{
		gotoxy(42,18); textcolor(RED); cprintf("%c",char(1)); land[42][18]=-2;
		gotoxy(43,3); textcolor(RED); cprintf("%c",char(1)); land[43][3]=-2;
		gotoxy(44,18); textcolor(RED); cprintf("%c",char(1)); land[44][18]=-2;
		gotoxy(45,3); textcolor(RED); cprintf("%c",char(1)); land[45][3]=-2;
//		ARR_1(ay[0]);
		ARR_2(ay[1]);
		ARR_3(ay[2]);
		ARR_4(ay[3]);
	}
}
void BOAT(int b)
{
  if (b==0)
  {
	for (y=3; y<19; y++)	land[31][y]=2;
	for (y=3; y<19; y++)	land[32][y]=2;
	for (y=3; y<19; y++)	land[33][y]=2;
	for (y=3; y<19; y++)	land[34][y]=2;
	for (y=3; y<19; y++)	land[35][y]=2;
	BOAT_1(by[0]);
	BOAT_2(by[1]);
	BOAT_3(by[2]);
	BOAT_4(by[3]);
	BOAT_5(by[4]);
  }
  else if (b==1)
  {
	for (y=3; y<19; y++)	land[31][y]=4;
	for (y=3; y<19; y++)	land[32][y]=2;
	for (y=3; y<19; y++)	land[33][y]=2;
	for (y=3; y<19; y++)	land[34][y]=2;
	for (y=3; y<19; y++)	land[35][y]=2;
	BOAT_2(by[1]);
	BOAT_3(by[2]);
	BOAT_4(by[3]);
	BOAT_5(by[4]);
  }
  else if (b==2)
  {
	for (y=3; y<19; y++)	land[31][y]=2;
	for (y=3; y<19; y++)	land[32][y]=4;
	for (y=3; y<19; y++)	land[33][y]=2;
	for (y=3; y<19; y++)	land[34][y]=2;
	for (y=3; y<19; y++)	land[35][y]=2;
	BOAT_1(by[1]);
	BOAT_3(by[2]);
	BOAT_4(by[3]);
	BOAT_5(by[4]);
  }
  else if (b==3)
  {
	for (y=3; y<19; y++)	land[32][y]=2;
	for (y=3; y<19; y++)	land[33][y]=4;
	for (y=3; y<19; y++)	land[31][y]=2;
	for (y=3; y<19; y++)	land[34][y]=2;
	for (y=3; y<19; y++)	land[35][y]=2;
	BOAT_2(by[1]);
	BOAT_1(by[2]);
	BOAT_4(by[3]);
	BOAT_5(by[4]);
  }
  else if (b==4)
  {
	for (y=3; y<19; y++)	land[33][y]=2;
	for (y=3; y<19; y++)	land[34][y]=4;
	for (y=3; y<19; y++)	land[31][y]=2;
	for (y=3; y<19; y++)	land[32][y]=2;
	for (y=3; y<19; y++)	land[35][y]=2;
	BOAT_2(by[1]);
	BOAT_3(by[2]);
	BOAT_1(by[3]);
	BOAT_5(by[4]);
  }
  else if (b==5)
  {
	for (y=3; y<19; y++)	land[34][y]=2;
	for (y=3; y<19; y++)	land[35][y]=4;
	for (y=3; y<19; y++)	land[31][y]=2;
	for (y=3; y<19; y++)	land[32][y]=2;
	for (y=3; y<19; y++)	land[33][y]=2;
	BOAT_2(by[1]);
	BOAT_3(by[2]);
	BOAT_1(by[3]);
	BOAT_4(by[4]);
  }
}
void BOAT_1(int &bby)
{
	gotoxy(31,bby);	textcolor(BLUE); cprintf("%c",char(219)); bby++;
	if (bby>=19)	bby=3;
	gotoxy(31,bby);	textcolor(BROWN); cprintf("%c",char(219));
	land[31][bby-1]=2;
	land[31][bby]=3;
}
void BOAT_2(int &bby)
{
	gotoxy(32,bby);	textcolor(BLUE); cprintf("%c",char(219)); bby+=5;
	if (bby>=19)	bby=3;
	gotoxy(32,bby);	textcolor(BROWN); cprintf("%c",char(219));
	land[32][bby-5]=2;
	land[32][bby]=3;
}
void BOAT_3(int &bby)
{
	gotoxy(33,bby);	textcolor(BLUE); cprintf("%c",char(219)); bby+=7;
	if (bby>=19)	bby=3;
	gotoxy(33,bby);	textcolor(BROWN); cprintf("%c",char(219));
	land[33][bby-7]=2;
	land[33][bby]=3;
}
void BOAT_4(int &bby)
{
	gotoxy(34,bby);	textcolor(BLUE); cprintf("%c",char(219)); bby+=2;
	if (bby>=19)	bby=3;
	gotoxy(34,bby);	textcolor(BROWN); cprintf("%c",char(219));
	land[34][bby-2]=2;
	land[34][bby]=3;
}
void BOAT_5(int &bby)
{
	gotoxy(35,bby);	textcolor(BLUE); cprintf("%c",char(219)); bby+=3;
	if (bby>=19)	bby=3;
	gotoxy(35,bby);	textcolor(BROWN); cprintf("%c",char(219));
	land[35][bby-3]=2;
	land[35][bby]=3;
}
void LAVA()
{
	LINER();
	gotoxy(3,21); textcolor(RED); cprintf("%s","WATCH_OUT_FOR_THE_LAVA !!");
	gotoxy(66,17); textcolor(GREEN);
	cprintf("%c",char(219)); land[66][17]=1;
	gotoxy(67,17); textcolor(GREEN);
	cprintf("%c",char(219)); land[67][17]=1;
	gotoxy(67,16); textcolor(GREEN);
	cprintf("%c",char(219)); land[67][16]=1;
	gotoxy(67,15); textcolor(GREEN);
	cprintf("%c",char(219)); land[67][15]=1;
	gotoxy(67,14); textcolor(GREEN);
	cprintf("%c",char(219)); land[67][14]=1;
	gotoxy(68,14); textcolor(GREEN);
	cprintf("%c",char(219)); land[68][14]=1;
	gotoxy(69,14); textcolor(GREEN);
	cprintf("%c",char(219)); land[69][14]=1;
	gotoxy(69,13); textcolor(GREEN);
	cprintf("%c",char(219)); land[69][13]=1;
	gotoxy(69,12); textcolor(GREEN);
	cprintf("%c",char(219)); land[69][12]=1;
	gotoxy(70,12); textcolor(GREEN);
	cprintf("%c",char(219)); land[70][12]=1;
	gotoxy(71,12); textcolor(GREEN);
	cprintf("%c",char(219)); land[71][12]=1;
	gotoxy(72,12); textcolor(GREEN);
	cprintf("%c",char(219)); land[72][12]=1;
	gotoxy(72,13); textcolor(GREEN);
	cprintf("%c",char(219)); land[72][13]=1;
	gotoxy(73,13); textcolor(GREEN);
	cprintf("%c",char(219)); land[73][13]=1;

}
void Cage()
{
	for (x=4; x<13; x++) { gotoxy(x,7); textcolor(16); cprintf("%c",char(219)); }
	for (x=4; x<13; x++) { gotoxy(x,13); textcolor(16); cprintf("%c",char(219)); }
	for (y=8; y<13; y++) { gotoxy(4,y); textcolor(16); cprintf("%c",char(219)); }
	for (y=8; y<13; y++) { gotoxy(12,y); textcolor(16); cprintf("%c",char(219)); }
}


void UP(int &xc, int &yc)
{
	if (land[xc][yc-1]==2)
	{
		LINER();
		gotoxy(4,21); textcolor(11); cprintf("%s","SPLASH !!");
		getch(); ctr-=60; gmr=1;
	}
	if (land[xc][yc-1]==-1)
	{
		LINER();
		gotoxy(4,21); textcolor(RED); cprintf("%s","LAVA_TO_DAA_FACE !!");
		getch(); ctr-=25; gmr=1;
	}
	if (land[xc][yc-1]==-2)
	{
		LINER();
		gotoxy(4,21); textcolor(WHITE); cprintf("%s","DEATH_BY_PROJECTILE !!");
		getch(); ctr+=42; gmr=1;
	}
	if (land[xc][yc-1]!=2&&land[xc][yc-1]!=0)
	{
		yc--;  if (land[xc][yc+1]==1)	LAND_(xc,yc+1);
		else if (land[xc][yc+1]==2||land[xc][yc+1]==4)		WATER(xc,yc+1);
		ME(xc,yc);
	}
}
void LEFT(int &xc, int &yc)
{
	if (land[xc-1][yc]==2)
	{
		LINER();
		gotoxy(4,21); textcolor(11); cprintf("%s","SPLASH !!");
		getch(); ctr+=60; gmr=1;
	}
	if (land[xc-1][yc]==-1)
	{
		LINER();
		gotoxy(4,21); textcolor(RED); cprintf("%s","LAVA_TO_DAA_FACE !!");
		getch(); ctr+=25; gmr=1;
	}
	if (land[xc-1][yc]==-2)
	{
		LINER();
		gotoxy(4,21); textcolor(WHITE); cprintf("%s","DEATH_BY_PROJECTILE !!");
		getch(); ctr+=42; gmr=1;
	}
	if (land[xc-1][yc]!=2&&land[xc-1][yc]!=0)
	{
		if (land[xc-1][yc]==3)
		{
			if (xc-1==31)	b=1;
			else if (xc-1==32)	b=2;
			else if (xc-1==33)	b=3;
			else if (xc-1==34)	b=4;
			else if (xc-1==35)	b=5;
		}
		xc--;  if (land[xc+1][yc]==1)	LAND_(xc+1,yc);
		else if (land[xc+1][yc]==2||land[xc+1][yc]==4)		WATER(xc+1,yc);
		ME(xc,yc);
	}
}
void DOWN(int &xc, int &yc)
{
	if (land[xc][yc+1]==2)
	{
		LINER();
		gotoxy(4,21); textcolor(11); cprintf("%s","SPLASH !!");
		getch(); ctr+=60; gmr=1;
	}
	if (land[xc][yc+1]==-2)
	{
		LINER();
		gotoxy(4,21); textcolor(WHITE); cprintf("%s","DEATH_BY_PROJECTILE !!");
		getch(); ctr+=42; gmr=1;
	}
	if (land[xc][yc+1]==-1)
	{
		LINER();
		gotoxy(4,21); textcolor(RED); cprintf("%s","LAVA_TO_DAA_FACE !!");
		getch(); ctr+=25; gmr=1;
	}
	if (land[xc][yc+1]!=2&&land[xc][yc+1]!=0)
	{
		yc++;  if (land[xc][yc-1]==1)	LAND_(xc,yc-1);
		else if (land[xc][yc-1]==2||land[xc][yc-1]==4)		WATER(xc,yc-1);
		ME(xc,yc);
	}
}
void RIGHT(int &xc, int &yc)
{
	if (land[xc+1][yc]==2)
	{
		LINER();
		gotoxy(4,21); textcolor(11); cprintf("%s","SPLASH !!");
		getch(); ctr+=60; gmr=1;
	}
	if (land[xc+1][yc]==-1)
	{
		LINER();
		gotoxy(4,21); textcolor(RED); cprintf("%s","LAVA_TO_DAA_FACE !!");
		getch(); ctr+=25; gmr=1;
	}
	if (land[xc+1][yc]==-2)
	{
		LINER();
		gotoxy(4,21); textcolor(WHITE); cprintf("%s","DEATH_BY_PROJECTILE !!");
		getch(); ctr+=42; gmr=1;
	}
	if (xc+1==37)
	{
		LINER();  ctr-=40;
		gotoxy(4,21); textcolor(RED); cprintf("%s","ENEMIES_IN_SIGHT !!");
	}
	if (xc+1==75)
	{
		LINER();
		gotoxy(4,21);  textcolor(WHITE); cprintf("%s","CONGRATS !!");
		getch(); gmr=2;
	}
	if (xc+1==65)
	{
		for (x=66; x<74; x++)
		{
			for (y=3; y<19; y++)
			{
				gotoxy(x,y); textcolor(RED);
				cprintf("%c",char(219)); land[x][y]=-1;
			}
		}
		ctr-=50;
		LAVA();

	}
	if (xc+1==37)	a=1;
	if (land[xc+1][yc]!=2&&land[xc+1][yc]!=0)
	{
		if (land[xc+1][yc]==3)
		{
			if (xc+1==31)	b=1;
			else if (xc+1==32)	b=2;
			else if (xc+1==33)	b=3;
			else if (xc+1==34)	b=4;
			else if (xc+1==35)	b=5;
		}
		xc++;  if (land[xc-1][yc]==1)	LAND_(xc-1,yc);
		else if (land[xc-1][yc]==2||land[xc-1][yc]==4)		WATER(xc-1,yc);
		ME(xc,yc);
	}
}


int River_Dale(int skp)
{
clrscr();

  BEGG:
	if (skp==1)
	{
	clrscr();

		cout<<"GOING TO END IT...."; getch();
		clrscr();
		return ctr;

	}
	else
	{
	clrscr();

		int xc=8, yc=10;	char mov;
		for (y=0; y<5; y++)	by[y]=3;
		ay[0]=17; ay[1]=4; ay[2]=17; ay[3]=4; ay[4]=17;
		for (y=3; y<19; y++)
		{
			for (x=3; x<77; x++)
				land[x][y]=0;
		}
		for (y=3; y<19; y++)
		{
			gotoxy(75,y); textcolor(11); cprintf("%c",char(219));
			for (x=3; x<77; x++)
			{ gotoxy(x,y); LAND_(x,y); }
			for (x=31; x<36; x++)
			{ gotoxy(x,y); WATER(x,y); }
		}
		gotoxy(75,6); textcolor(WHITE); cprintf("%c",'F');
		gotoxy(75,7); textcolor(WHITE); cprintf("%c",'I');
		gotoxy(75,8); textcolor(WHITE); cprintf("%c",'N');
		gotoxy(75,9); textcolor(WHITE); cprintf("%c",'I');
		gotoxy(75,10); textcolor(WHITE); cprintf("%c",'S');
		gotoxy(75,11); textcolor(WHITE); cprintf("%c",'H');
		gotoxy(75,12); textcolor(WHITE); cprintf("%c",' ');
		gotoxy(75,13); textcolor(WHITE); cprintf("%c",'L');
		gotoxy(75,14); textcolor(WHITE); cprintf("%c",'I');
		gotoxy(75,15); textcolor(WHITE); cprintf("%c",'N');
		gotoxy(75,16); textcolor(WHITE); cprintf("%c",'E');

		ME(xc,yc);

		gotoxy(3,21); textcolor(RED); cprintf("%s","CROSS_THE_RIVER BEFORE THE RED_WOLVES CATCH UP!!");
		while(gmr!=1||gmr!=2)
		{
			if (gmr==1) break;
			if (gmr==2) break;
			BOAT(b);
			ARROW(a);
			Cage();
			mov=getch();
			ctr++; mv++;
			if (mov=='w')
				UP(xc,yc);
			else if (mov=='a')
				LEFT(xc,yc);
			else if (mov=='s')
				DOWN(xc,yc);
			else if (mov=='d')
				RIGHT(xc,yc);
			else if (mov=='/')
				exit(0);
			if (mv%3==0)
			{
				for (y=3; y<21; y++)
				{ gotoxy(mx,y); textcolor(4); cprintf("%c",char(15)); land[mx][y]=-2; }
				mx++;
				if (mx-1==xc)
				{
					LINER(); gotoxy(4,21); textcolor(RED);
					cprintf("%s","DEATH BY RED_WOLVES !!"); ctr+=30; gmr=1;
				}
			}
		}
		if (gmr==1)
		{
			clrscr(); textcolor(15); Delayer("You couldn't save yourself, try again !!");
			mx=3; ctr=0; gmr=0; getch(); goto BEGG;
		}
		ctr=300-ctr;
		return ctr;
	}


//getch();
}


//  */