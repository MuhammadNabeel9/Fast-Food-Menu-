#include<iostream>
#include<fstream>
using namespace std;
int main() 
{
	string pizza, hotwings, juice, drink, pasta, customer, cellphone,c,d,e;
	char a, b, u;
	a = 'y';
	b = 'n';

	cout<<"                      HELLO AND WELCOME TO CHEEZIOUS FAST FOOD! WE ARE HERE TO MAKE YOUR EXPERIENCE EXTRAORDINARY:  "<<endl;
	ofstream write;
	write.open("DATA.txt",ios::out);
	
	cout<<"                                                WELCOME TO CUSTOMER DETAILS:            "<<endl;
	
	cout<<"                                                Enter Order Number = ";
	getline(cin,customer);
	write<<"Order Number = "<<customer<<endl;
	
	cout<<"                       Enter Name Of Customer = ";
	getline(cin,customer);
	cout<<"                       Enter Phone Number Of Customer = ";
	getline(cin,cellphone);
	write<<"Name = "<<customer<<endl;
	write<<"Phone number = "<<cellphone<<endl;
   	A:
	cout<<"                   THE MENUE OF CHEEZIOUS FAST FOOD ARE FOLLOWING:"<<endl;
	cout<<"                                     (PIZZA'S Category):           "<<endl;
	cout<<"                   SMALL(SIZE PRICE)       MEDIUM(SIZE PRICE)      LARGE(SIZE PRICE)   "<<endl;
	cout<<"1-CHICKEN FAJITA         550/RS                 1000/RS                  1400/RS       "<<endl;
	cout<<"2-CHICKEN SUPREME        550/RS                 1000/RS                  1400/RS       "<<endl;
	cout<<"3-TANDORI PIZZA          550/RS                 1000/RS                  1400/RS       "<<endl;
	cout<<"4-CHICKEN LOVER          550/RS                 1000/RS                  1400/RS       "<<endl;
	cout<<"5-BEEF PIZZA             700/RS                 1200/RS                  1600/RS       "<<endl;
	cout<<"6-CHEEZIOUS SPECIAL      700/RS                 1200/RS                  1600/RS       "<<endl;
	cout<<"                                      (PASTA'S Category):                              "<<endl;
	cout<<"                           HALF(SIZE PRICE)        FULL(SIZE PRICE)                    "<<endl;
	cout<<"7-VEG PENNE PASTA               450/RS                 750/RS                          "<<endl;
	cout<<"8-CHICKEN PENNE PASTA           450/RS                 750/RS                          "<<endl;
	cout<<"9-SPICY PENNE PASTA             450/RS                 750/RS                          "<<endl;
	cout<<"10-BBQ PENNE PASTA               450/RS                 750/RS                         "<<endl;
	cout<<"11-CHEEZY PENNE PASTA            550/RS                 900/RS                         "<<endl;
	cout<<"                                      (HOTWINGS/JUICES/DRINKS)                         "<<endl;
	cout<<"                           12-HOTWINGS(PRICE)      8-HOTWINGS(PRICE)                   "<<endl;
	cout<<"12-HOTWINGS                      550/RS                  400/RS                        "<<endl;
	cout<<"                                       JUICES(PRICES)                                  "<<endl;
	cout<<"                            SMALL(SIZE)               LARGE(SIZE)                      "<<endl;
	cout<<"13-NESTLE JUICE                  60/RS                   200/RS                        "<<endl;
	cout<<"14-APPLE JUICE                   60/RS                   200/RS                        "<<endl;
	cout<<"15-COCONUT WATER                 100/RS                  250/RS                        "<<endl;
	cout<<"16-LEMON JUICE                   60/RS                   200/RS                        "<<endl;
	cout<<"                                       DRINKES(PRICES)                                 "<<endl;
	cout<<"                               HALF(LITER)          ONE(LITER)       ONE&HALF(LITER)   "<<endl;
	cout<<"17-SPRITE                         70/RS               150/RS              250/RS       "<<endl;
	cout<<"18-FANTA                          60/RS               140/RS              230/RS       "<<endl;
	cout<<"19-STING                          120/RS                                               "<<endl;
	cout<<"20-PEPSI                          50/RS               120/RS              220/RS       "<<endl;
    
	int n,n1,n2,p1=0,p2=0,p3=0,p4=0,p5=0,p6=0,p7=0,p8=0,p9=0,p10=0,p11=0,p12=0,p13=0,p14=0,p15=0,p16=0,p17=0,p18=0,p19=0,p20=0,p21=0,p22=0,p23=0,p24=0,p25=0,p26=0,p27=0,p28=0,p29=0,p30=0,p31=0,p32=0,p33=0,p34=0,p35=0,p36=0,p37=0,p38=0,p39=0,p40=0,p41=0,p42=0,p43=0,p44=0,p45=0,p46=0,p47=0,p48=0;
	P:
	cout<<endl;
	cout<<"                         KINDLY PLACE YOUR ORDER AND ENJOY YOUR MEAL:                "<<endl;
	cout<<endl;
	N:
	cout<<" Enter Item No from 1 to 20 = ";
	cin>>n;
	switch(n) {
		case 1:
			cout<<"You Have Selected CHICKEN FAJITA PIZZA "<<endl;
			cout<<"Which Size you want 1(small) 2(medium) 3(large) = ";
			cin>>n1;
			if (n1>3 || n1<1 || n1==0)
			{
				cout<<"Ivalid Choice ";
				goto P;
			}
			
			else if(n1==1) 
			{
				cout<<"Enter The Quantity Of Item You Would like to order = ";
				cin>>n2;
				cout<<"You Have Ordered "<<n2<<" Small CHICKEN FAJITA PIZZA ";
				cout<<"At Price Of = "<<550*n2;
				p1=550*n2;
				write<<"You Have Ordered "<<n2<<" Small CHICKEN FAJITA PIZZA AT Price of = "<<p1<<endl;
			}
			else if(n1 == 2)
			{
				cout<<"Enter The Quantity Of Item You Would like to order = ";
				cin>>n2;
				cout<<"You Have Ordered "<<n2<<" Medium CHICKEN FAJITA PIZZA ";
				cout<<"At Price Of = "<<1000*n2;
				p2=1000*n2;
				write<<"You Have Ordered "<<n2<<" Medium CHICKEN FAJITA PIZZA AT Price of = "<<p2<<endl;
            }
			else if(n1==3)
			{
				cout<<"Enter The Quantity Of Item You Would like to order = ";
				cin>>n2;
				cout<<"You Have Ordered "<<n2<<" Large CHICKEN FAJITA PIZZA ";
				cout<<"At Price Of = "<<1400*n2;
				p3=1400*n2;
				write<<"You Have Ordered "<<n2<<" Large CHICKEN FAJITA PIZZA AT Price of = "<<p3<<endl;
            }
			break;    
			case 2:
				cout<<"You Have Selected CHICKEN SUPREME PIZZA "<<endl;
				cout<<"Which Size you want 1(small) 2(medium) 3(large) = ";
				cin>>n1;
				if (n1>3 || n1<1 || n1==0)
			{
				cout<<"Ivalid Choice ";
				goto P;
			}
				
				else if(n1==1)
				{
					cout<<"Enter The Quantity Of Item You Would like to order = ";
					cin>>n2;
					cout<<"You Have Ordered "<<n2<<" Small CHICKEN SUPREME PIZZA ";
					cout<<"At Price Of = "<<550*n2;
					p4=550*n2;
					write<<"You Have Ordered "<<n2<<" Small CHICKEN SUPREME PIZZA AT Price of = "<<p4<<endl;
            	}
				else if(n1==2)
				{
					cout<<"Enter The Quantity Of Item You Would like to order = ";
					cin>>n2;
					cout<<"You Have Ordered "<<n2<<" Medium CHICKEN SUPREME PIZZA ";
					cout<<"At Price Of = "<<1000*n2;
					p5=1000*n2;
					write<<"You Have Ordered "<<n2<<" Medium CHICKEN SUPREME PIZZA AT Price of = "<<p5<<endl;
            	}
				else if(n1==3)
				{
					cout<<"Enter The Quantity Of Item You Would like to order = ";
					cin>>n2;
					cout<<"You Have Ordered " <<n2<<" Large CHICKEN SUPREME pizza ";
					cout<<"At Price Of = "<<1400*n2;
					p6=1400*n2;
					write<<"You Have Ordered "<<n2<<" Large CHICKEN SUPREME PIZZA AT Price of = "<<p6<<endl;
            	}
            	break;
        		case 3:
					cout<<"You Have Selected TANDORI PIZZA " << endl;
					cout<<"Which Size you want 1(small) 2(medium) 3(large) = ";
					cin>>n1;
					if (n1>3 || n1<1 || n1==0)
					{
						cout<<"Ivalid Choice ";
						goto P;
						}
					
					else if(n1==1)
				{
					cout<<"Enter The Quantity Of Item You Would like to order = ";
					cin>>n2;
					cout<<"You Have Ordered "<<n2<<" Small TANDORI PIZZA ";
					cout<<"At Price Of = "<<550*n2;
					p7=550*n2;
					write<<"You Have Ordered "<<n2<<" Small TANDORI PIZZA AT Price of = "<<p7<<endl;
            	}
				else if(n1==2)
				{
					cout<<"Enter The Quantity Of Item You Would like to order = ";
					cin>>n2;
					cout<<"You Have Ordered "<<n2<<" Medium TANDORI PIZZA ";
					cout<<"At Price Of = "<<1000*n2;
					p8=1000*n2;
					write<<"You Have Ordered "<<n2<<" Medium TANDORI PIZZA AT Price of = "<<p8<<endl;
				}
				else if(n1==3)
				{
					cout<<"Enter The Quantity Of Item You Would like to order = ";
					cin>>n2;
					cout<<"You Have Ordered "<<n2<<" Large TANDORI PIZZA ";
					cout<<"At Price Of = "<<1400*n2;
					p9=1400*n2;
					write<<"You Have Ordered "<<n2<<" Large TANDORI PIZZA AT Price of = "<<p9<<endl;
				}
				break;
				case 4:
					cout<<"You Have Selected CHICKEN LOVER PIZZA " << endl;
            		cout<<"Which Size you want 1(small) 2(medium) 3(large) = ";
            		cin>>n1;
            		if (n1>3 || n1<1 || n1==0)
					{
						cout<<"Ivalid Choice ";
						goto P;
						}
            		
            		else if(n1==1)
					{
						cout<<"Enter The Quantity Of Item You Would like to order = ";
            			cin>>n2;
                		cout<<"You Have Ordered "<<n2<<" Small CHICKEN LOVER PIZZA ";
                		cout<<"At Price Of = " <<550*n2;
                		p10=550*n2;
                		write<<"You Have Ordered "<<n2<<" Small CHICKEN LOVER PIZZA AT Price of = "<<p10<<endl;
            		}
					else if(n1==2)
					{
						cout<<"Enter The Quantity Of Item You Would like to order = ";
            			cin>>n2;
                		cout<<"You Have Ordered "<<n2<<" Medium CHICKEN LOVER PIZZA ";
                		cout<<"At Price Of = "<<1000*n2;
                		p11=1000 * n2;
                		write<<"You Have Ordered "<<n2<<" Medium CHICKEN LOVER PIZZA AT Price of = "<<p11<<endl;
            		}
					else if(n1==3)
					{
						cout<<"Enter The Quantity Of Item You Would like to order = ";
            			cin>>n2;
                		cout<<"You Have Ordered "<<n2<<" Large CHICKEN LOVER PIZZA ";
                		cout<<"At Price Of = "<<1400*n2;
                		p12=1400*n2;
                		write<<"You Have Ordered "<<n2<<" Large CHICKEN LOVER PIZZA AT Price of = "<<p12<<endl;
            		}
            		break;
            		case 5:
						cout<<"You Have Selected BEEF PIZZA "<<endl;
						cout<<"Which Size you want 1(small) 2(medium) 3(large) = ";
						cin>>n1;
						if (n1>3 || n1<1 || n1==0)
						{
							cout<<"Ivalid Choice ";
							goto P;
						}
						
						else if(n1==1)
						{
							cout<<"Enter The Quantity Of Item You Would like to order = ";
							cin>>n2;
							cout<<"You Have Ordered "<< n2 <<" Small BEEF PIZZA ";
							cout<<"At Price Of = "<<700*n2;
							p13=700*n2;
							write<<"You Have Ordered "<<n2<<" Small BEEF PIZZA AT Price of = "<<p13<<endl;
						}
						else if(n1==2)
						{
							cout<<"Enter The Quantity Of Item You Would like to order = ";
							cin>>n2;
							cout<<"You Have Ordered "<< n2 <<" Medium BEEF PIZZA ";
							cout<<"At Price Of = "<<1200*n2;
							p14=1200*n2;
							write<<"You Have Ordered "<<n2<<" Medium BEEF PIZZA AT Price of = "<<p14<<endl;
						}
						else if(n1==3)
						{
							cout<<"Enter The Quantity Of Item You Would like to order = ";
							cin>>n2;
							cout<<"You Have Ordered "<< n2 <<" Large BEEF PIZZA ";
							cout<<"At Price Of = "<<1600*n2;
							p15=1600*n2;
							write<<"You Have Ordered "<<n2<<" Large BEEF PIZZA AT Price of = "<<p15<<endl;
						}
						break;
						case 6:
							cout<<"You Have Selected CHEEZIOUS SPECIAL "<<endl;
							cout<<"Which Size you want 1(small) 2(medium) 3(large) = ";
							cin>>n1;
							if (n1>3 || n1<1 || n1==0)
						{
							cout<<"Ivalid Choice ";
							goto P;
						}
						
							else if(n1==1)
							{
								cout<<"Enter The Quantity Of Item You Would like to order = ";
								cin>>n2;
								cout<<"You Have Ordered "<< n2 <<" Small CHEEZIOUS SPECIAL PIZZA ";
								cout<<"At Price Of = "<<700*n2;
								p16=700*n2;
								write<<"You Have Ordered "<<n2<<" Small CHEEZIOUS SPECIAL PIZZA AT Price of = "<<p16<<endl;
							}
							else if(n1==2)
							{
								cout<<"Enter The Quantity Of Item You Would like to order = ";
								cin>>n2;
								cout<<"You Have Ordered "<< n2 <<" Medium CHEEZIOUS SPECIAL PIZZA ";
								cout<<"At Price Of = "<<1200*n2;
								p17=1200*n2;
								write<<"You Have Ordered "<<n2<<" Medium CHEEZIOUS SPECIAL PIZZA AT Price of = "<<p17<<endl;
							}
							else if(n1==3)
							{
								cout<<"Enter The Quantity Of Item You Would like to order = ";
								cin>>n2;
								cout<<"You Have Ordered "<< n2 <<" Large CHEEZIOUS SPECIAL PIZZA ";
								cout<<"At Price Of = "<<1600*n2;
								p18=1600*n2;
								write<<"You Have Ordered "<<n2<<" Large CHEEZIOUS SPECIAL PIZZA AT Price of = "<<p18<<endl;
							}
								break;
								case 7:
								cout<<"You Have Selected VEG PENNE PASTA "<<endl;
								cout<<"Which Size you want 1(Half) 2(Full) = ";
								cin>>n1;
								if (n1>2 || n1<1 || n1==0)
							{
								cout<<"Ivalid Choice ";
								goto P;
							}
								
								else if(n1==1)
								{
									cout<<"Enter The Quantity Of Item You Would like to order = ";
									cin>>n2;
									cout<<"You Have Ordered "<< n2 <<" Half VEG PENNE PASTA ";
									cout<<"At Price Of = "<<450*n2;
									p19=450*n2;
									write<<"You Have Ordered "<<n2<<" Half VEG PENNE PASTA AT Price of = "<<p19<<endl;
								}
								else if(n1==2)
								{
									cout<<"Enter The Quantity Of Item You Would like to order = ";
									cin>>n2;
									cout<<"You Have Ordered "<< n2 <<" Full VEG PENNE PASTA ";
									cout<<"At Price Of = "<<750*n2;
									p20=750*n2;
									write<<"You Have Ordered "<<n2<<" Full VEG PENNE PASTA AT Price of = "<<p20<<endl;
								}
								break;
								case 8:
									cout<<"You Have Selected CHICKEN PENNE PASTA "<<endl;
									cout<<"Which Size you want 1(Half) 2(Full) = ";
									cin>>n1;
									if (n1>2 || n1<1 || n1==0)
									{
										cout<<"Ivalid Choice ";
										goto P;
									}
									
									else if(n1==1)
									{
										cout<<"Enter The Quantity Of Item You Would like to order = ";
										cin>>n2;
										cout<<"You Have Ordered "<< n2 <<" Half CHICKEN PENNE PASTA ";
										cout<<"At Price Of = "<<450*n2;
										p21=450*n2;
										write<<"You Have Ordered "<<n2<<" Half CHICKEN PENNE PASTA AT Price of = "<<p21<<endl;
									}
									else if(n1==2)
									{
										cout<<"Enter The Quantity Of Item You Would like to order = ";
										cin>>n2;
										cout<<"You Have Ordered "<< n2 <<" Full CHICKEN PENNE PASTA ";
										cout<<"At Price Of = "<<750*n2;
										p22=750*n2;
										write<<"You Have Ordered "<<n2<<" Full CHICKEN PENNE PASTA AT Price of = "<<p22<<endl;
									}
									break;
									case 9:
										cout<<"You Have Selected SPICY PENNE PASTA "<<endl;
										cout<<"Which Size you want 1(Half) 2(Full) = ";
										cin>>n1;
										if (n1>2 || n1<1 || n1==0)
										{
											cout<<"Ivalid Choice ";
											goto P;
										}
										
										else if(n1==1)
										{
											cout<<"Enter The Quantity Of Item You Would like to order = ";
											cin>>n2;
											cout<<"You Have Ordered "<< n2 <<" Half SPICY PENNE PASTA ";
											cout<<"At Price Of = "<<450*n2;
											p23=450*n2;
											write<<"You Have Ordered "<<n2<<" Half SPICY PENNE PASTA AT Price of = "<<p23<<endl;
										}
										else if(n1==2)
										{
											cout<<"Enter The Quantity Of Item You Would like to order = ";
											cin>>n2;
											cout<<"You Have Ordered "<< n2 <<" Full SPICY PENNE PASTA ";
											cout<<"At Price Of = "<<750*n2;
											p24=750*n2;
											write<<"You Have Ordered "<<n2<<" Full SPICY PENNE PASTA AT Price of = "<<p24<<endl;
										}
										break;
										case 10:
											cout<<"You Have Selected BBQ PENNE PASTA "<<endl;
											cout<<"Which Size you want 1(Half) 2(Full) = ";
											cin>>n1;
											if (n1>2 || n1<1 || n1==0)
											{
												cout<<"Ivalid Choice ";
												goto P;
											}
											
											else if(n1==1)
											{
												cout<<"Enter The Quantity Of Item You Would like to order = ";
												cin>>n2;
												cout<<"You Have Ordered "<< n2 <<" Half BBQ PENNE PASTA ";
												cout<<"At Price Of = "<<450*n2;
												p25=450*n2;
												write<<"You Have Ordered "<<n2<<" Half BBQ PENNE PASTA AT Price of = "<<p25<<endl;
											}
											else if(n1==2)
											{
												cout<<"Enter The Quantity Of Item You Would like to order = ";
												cin>>n2;
												cout<<"You Have Ordered "<< n2 <<" Full BBQ PENNE PASTA ";
												cout<<"At Price Of = "<<750*n2;
												p26=750*n2;
												write<<"You Have Ordered "<<n2<<" Full BBQ PENNE PASTA AT Price of = "<<p26<<endl;
											}
											break;
											case 11:
												cout<<"You Have Selected CHEEZY PENNE PASTA "<<endl;
												cout<<"Which Size you want 1(Half) 2(Full) = ";
												cin>>n1;
												if (n1>2 || n1<1 || n1==0)
												{
													cout<<"Ivalid Choice ";
													goto P;
												}
												
												else if(n1==1)
												{
													cout<<"Enter The Quantity Of Item You Would like to order = ";
													cin>>n2;
													cout<<"You Have Ordered "<< n2 <<" Half CHEEZY PENNE PASTA ";
													cout<<"At Price Of = "<<550*n2;
													p27=550*n2;
													write<<"You Have Ordered "<<n2<<" Half CHEEZY PENNE PASTA AT Price of = "<<p27<<endl;
												}
												else if(n1==2)
												{
													cout<<"Enter The Quantity Of Item You Would like to order = ";
													cin>>n2;
													cout<<"You Have Ordered "<< n2 <<" Full CHEEZY PENNE PASTA ";
													cout<<"At Price Of = "<<900*n2;
													p28=900*n2;
													write<<"You Have Ordered "<<n2<<" Full CHEEZY PENNE PASTA AT Price of = "<<p28<<endl;
												}
												break;
												case 12:
													cout<<"You Have Selected HOTWINGS "<<endl;
													cout<<"Which Size you want 1(12-HOTWINGS) 2(8-HOTWINGS) = ";
													cin>>n1;
													if (n1>2 || n1<1 || n1==0)
													{
														cout<<"Ivalid Choice ";
														goto P;
													}
													
													else if(n1==1)
													{
														cout<<"Enter The Quantity Of Item You Would like to order = ";
														cin>>n2;
														cout<<"You Have Ordered "<< n2 <<" 12-HOTWINGS HOTWINGS ";
														cout<<"At Price Of = "<<550*n2;
														p29=550*n2;
														write<<"You Have Ordered "<<n2<<" 12-HOTWINGS HOTWINGS AT Price of = "<<p29<<endl;
													}
													else if(n1==2)
													{
														cout<<"Enter The Quantity Of Item You Would like to order = ";
														cin>>n2;
														cout<<"You Have Ordered "<< n2 <<" 8-HOTWINGS HOTWINGS ";
														cout<<"At Price Of = "<<400*n2;
														p30=400*n2;
														write<<"You Have Ordered "<<n2<<" 8-HOTWINGS HOTWINGS AT Price of = "<<p30<<endl;
													}
													break;
													case 13:
														cout<<"You Have Selected NESTLE JUICE "<<endl;
														cout<<"Which Size you want 1(small) 2(large) = ";
														cin>>n1;
														if (n1>2 || n1<1 || n1==0)
														{
															cout<<"Ivalid Choice ";
															goto P;
														}
														
														else if(n1==1)
														{
															cout<<"Enter The Quantity Of Item You Would like to order = ";
															cin>>n2;
															cout<<"You Have Ordered "<< n2 <<" Small NESTLE JUICE ";
															cout<<"At Price Of = "<<60*n2;
															p31=60*n2;
															write<<"You Have Ordered "<<n2<<" Small NESTLE JUICE AT Price of = "<<p31<<endl;
														}
														else if(n1==2)
														{
															cout<<"Enter The Quantity Of Item You Would like to order = ";
															cin>>n2;
															cout<<"You Have Ordered "<< n2 <<" Large NESTLE JUICE ";
															cout<<"At Price Of = "<<200*n2;
															p32=200*n2;
															write<<"You Have Ordered "<<n2<<" Large NESTLE JUICE AT Price of = "<<p32<<endl;
														}
														break;
														case 14:
															cout<<"You Have Selected APPLE JUICE "<<endl;
															cout<<"Which Size you want 1(small) 2(large) = ";
															cin>>n1;
															if (n1>2 || n1<1 || n1==0)
															{
																cout<<"Ivalid Choice ";
																goto P;
															}
															
															else if(n1==1)
															{
																cout<<"Enter The Quantity Of Item You Would like to order = ";
																cin>>n2;
																cout<<"You Have Ordered "<< n2 <<" Small APPLE JUICE ";
																cout<<"At Price Of = "<<60*n2;
																p33=60*n2;
																write<<"You Have Ordered "<<n2<<" Small APPLE JUICE AT Price of = "<<p33<<endl;
															}
															else if(n1==2)
															{
																cout<<"Enter The Quantity Of Item You Would like to order = ";
																cin>>n2;
																cout<<"You Have Ordered "<< n2 <<" Large APPLE JUICE ";
																cout<<"At Price Of = "<<200*n2;
																p34=200*n2;
																write<<"You Have Ordered "<<n2<<" Large APPLE JUICE AT Price of = "<<p34<<endl;
																}
															break;
															case 15:
																cout<<"You Have Selected COCONUT WATER "<<endl;
																cout<<"Which Size you want 1(small) 2(large) = ";
																cin>>n1;
																if (n1>2 || n1<1 || n1==0)
																{
																	cout<<"Ivalid Choice ";
																	goto P;
																}
																
																else if(n1==1)
																{
																	cout<<"Enter The Quantity Of Item You Would like to order = ";
																	cin>>n2;
																	cout<<"You Have Ordered "<< n2 <<" Small COCONUT WATER ";
																	cout<<"At Price Of = "<<100*n2;
																	p35=100*n2;
																	write<<"You Have Ordered "<<n2<<" Small COCONUT WATER AT Price of = "<<p35<<endl;
																}
																else if(n1==2)
																{
																	cout<<"Enter The Quantity Of Item You Would like to order = ";
																	cin>>n2;
																	cout<<"You Have Ordered "<< n2 <<" Large COCONUT WATER ";
																	cout<<"At Price Of = "<<250*n2;
																	p36=250*n2;
																	write<<"You Have Ordered "<<n2<<" Large COCONUT WATER AT Price of = "<<p36<<endl;
																}
																break;
																case 16:
																	cout<<"You Have Selected LEMON JUICE "<<endl;
																	cout<<"Which Size you want 1(small) 2(large) = ";
																	cin>>n1;
																	if (n1>2 || n1<1 || n1==0)
																	{
																		cout<<"Ivalid Choice ";
																		goto P;
																	}
																	
																	else if(n1==1)
																	{
																		cout<<"Enter The Quantity Of Item You Would like to order = ";
																		cin>>n2;
																		cout<<"You Have Ordered "<< n2 <<" Small LEMON JUICE ";
																		cout<<"At Price Of = "<<60*n2;
																		p37=60*n2;
																		write<<"You Have Ordered "<<n2<<" Small LEMON JUICE AT Price of = "<<p37<<endl;
																	}
																	else if(n1==2)
																	{
																		cout<<"Enter The Quantity Of Item You Would like to order = ";
																		cin>>n2;
																		cout<<"You Have Ordered "<< n2 <<" Large LEMON JUICE ";
																		cout<<"At Price Of = "<<200*n2;
																		p38=200*n2;
																		write<<"You Have Ordered "<<n2<<" Large LEMON JUICE AT Price of = "<<p38<<endl;
																	}
																	break;
																	case 17:
																		cout<<"You Have Selected SPRITE "<<endl;
																		cout<<"Which Size you want 1(HALF) 2(ONE) 3(ONE&HALF) = ";
																		cin>>n1;
																		if (n1>3 || n1<1 || n1==0)
																		{
																			cout<<"Ivalid Choice ";
																			goto P;
																		}
																		
																		else if(n1==1)
																		{
																			cout<<"Enter The Quantity Of Item You Would like to order = ";
																			cin>>n2;
																			cout<<"You Have Ordered "<< n2 <<" Half Liter SPRITE ";
																			cout<<"At Price Of = "<<70*n2;
																			p39=70*n2;
																			write<<"You Have Ordered "<<n2<<" Half Liter SPRITE AT Price of = "<<p39<<endl;
																		}
																		else if(n1==2)
																		{
																			cout<<"Enter The Quantity Of Item You Would like to order = ";
																			cin>>n2;
																			cout<<"You Have Ordered "<< n2 <<" One Liter SPRITE ";
																			cout<<"At Price Of = "<<150*n2;
																			p40=150*n2;
																			write<<"You Have Ordered "<<n2<<" One Liter SPRITE AT Price of = "<<p40<<endl;
																		}
																		else if(n1==3)
																		{
																			cout<<"Enter The Quantity Of Item You Would like to order = ";
																			cin>>n2;
																			cout<<"You Have Ordered "<< n2 <<" ONE&HALF Liter SPRITE ";
																			cout<<"At Price Of = "<<250*n2;
																			p41=250*n2;
																			write<<"You Have Ordered "<<n2<<" ONE&HALF Liter SPRITE AT Price of = "<<p41<<endl;
																		}
																		break;
																		case 18:
																			cout<<"You Have Selected FANTA "<<endl;
																			cout<<"Which Size you want 1(HALF) 2(ONE) 3(ONE&HALF) = ";
																			cin>>n1;
																			if (n1>3 || n1<1 || n1==0)
																			{
																				cout<<"Ivalid Choice ";
																				goto P;
																			}
																			
																			else if(n1==1)
																			{
																				cout<<"Enter The Quantity Of Item You Would like to order = ";
																				cin>>n2;
																				cout<<"You Have Ordered "<< n2 <<" Half Liter FANTA ";
																				cout<<"At Price Of = "<<60*n2;
																				p42=60*n2;
																				write<<"You Have Ordered "<<n2<<" HALF Liter FANTA AT Price of = "<<p42<<endl;
																			}
																			else if(n1==2)
																			{
																				cout<<"Enter The Quantity Of Item You Would like to order = ";
																				cin>>n2;
																				cout<<"You Have Ordered "<< n2 <<" One Liter FANTA ";
																				cout<<"At Price Of = "<<140*n2;
																				p43=140*n2;
																				write<<"You Have Ordered "<<n2<<" One Liter FANTA AT Price of = "<<p43<<endl;
																			}
																			else if(n1==3)
																			{
																				cout<<"Enter The Quantity Of Item You Would like to order = ";
																				cin>>n2;
																				cout<<"You Have Ordered "<< n2 <<" ONE&HALF Liter FANTA ";
																				cout<<"At Price Of = "<<230*n2;
																				p44=230*n2;
																				write<<"You Have Ordered "<<n2<<" One&HALF Liter FANTA AT Price of = "<<p44<<endl;
																			}
																			break;
																			case 19:
																				cout<<"You Have Selected STING "<<endl;
																				cout<<"Enter The Quantity Of Item You Would like to order = ";
																				cin>>n2;
																				cout<<"You Have Ordered "<< n2 <<" STING ";
																				cout<<"At Price Of = "<<120*n2;
																				p45=120*n2;
																				write<<"You Have Ordered "<<n2<<" STING AT Price of = "<<p45<<endl;
																				break;
																				case 20:
																					cout<<"You Have Selected PEPSI "<<endl;
																					cout<<"Which Size you want 1(HALF) 2(ONE) 3(ONE&HALF) = ";
																					cin>>n1;
																					if (n1>3 || n1<1 || n1==0)
																					{
																						cout<<"Ivalid Choice ";
																						goto P;
																					}
																					
																					else if(n1==1)
																					{
																						cout<<"Enter The Quantity Of Item You Would like to order = ";
																						cin>>n2;
																						cout<<"You Have Ordered "<< n2 <<" Half Liter PEPSI ";
																						cout<<"At Price Of = "<<50*n2;
																						p46=50*n2;
																						write<<"You Have Ordered "<<n2<<" Half Liter PEPSI AT Price of = "<<p46<<endl;
																					}
																					else if(n1==2)
																					{
																						cout<<"Enter The Quantity Of Item You Would like to order = ";
																						cin>>n2;
																						cout<<"You Have Ordered "<< n2 <<" One Liter PEPSI ";
																						cout<<"At Price Of = "<<120*n2;
																						p47=120*n2;
																						write<<"You Have Ordered "<<n2<<" One Liter PEPSI AT Price of = "<<p47<<endl;
																					}
																					else if(n1==3)
																					{
																						cout<<"Enter The Quantity Of Item You Would like to order = ";
																						cin>>n2;
																						cout<<"You Have Ordered "<< n2 <<" ONE&HALF Liter PEPSI ";
																						cout<<"At Price Of = "<<220*n2;
																						p48=220*n2;
																						write<<"You Have Ordered "<<n2<<" One&HALF Liter PEPSI AT Price of = "<<p48<<endl;
																					}
																					break;
        																			default:
            																			cout << "Invalid Choice ";
    }

	cout<<endl;
	cout<<"You want to order more items Y(Yes) or N(No) = ";
	cin>>u;
	if(u=='y'||u=='Y')
	{
		goto N;
	}
	else if (u=='n'||u=='N')
	{
		cout<<endl;
		cout<<"Thanks For Your Order ";
		cout<<endl;
	}
	else
	{
		cout<<"Invalid choice ";
	}

    cout<<endl;

    int grandTotal=p1+p2+p3+p4+p5+p6+p7+p8+p9+p10+p11+p12+p13+p14+p15+p16+p17+p18+p19+p20+p21+p22+p23+p24+p25+p26+p27+p28+p29+p30+p31+p32+p33+p34+p35+p36+p37+p38+p39+p40+p41+p42+p43+p44+p45+p46+p47+p48;
    cout<<"Your Grand Total = "<<grandTotal<<endl;
    cout<<endl;
    write<<"Your Total Bill = "<<grandTotal<<endl;
    cout<<"           "<<endl;
    cout<<"           "<<endl;
    write<<endl;
    cout<<"Do You Have Another Customer.......? Y(Yes) or N(No) = ";
	cin>>u;
	if(u=='y'||u=='Y')
	{
		cout<<"                                                Enter Order Number = ";
		cin>>c;
		write<<"Order Number = "<<c<<endl;
		cout<<"                       Enter Name Of Customer = ";
		cin>>d;
		cout<<"                       Enter Phone Number Of Customer = ";
		cin>>e;
		write<<"Customer Name = "<<d<<endl;
		write<<"Phone number = "<<e<<endl;
		
		goto A;
	}
	else if (u=='n'||u=='N')
	{
		cout<<endl;
		cout<<"Thanks For Your Order ";
		cout<<endl;
	}
	else
	{
		cout<<"Invalid choice ";
	}
	string ch;
	ifstream file;
	file.open("DATA.txt",ios::in);
	cout<< "      "<<endl;
	while(!file.eof())
	{
		getline(file,ch);
		cout<<ch<<endl;
	}
	
	file.close();
	cout<<"THANKS FOR COMMING TO CHEEZIOUS FAST FOOD! WE HOPE TO SEE YOU AGAIN SOON";
	cout<<endl;
    return 0;
}

