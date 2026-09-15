Architecture :-
The system consists of the following architecture :-
1) Market :- The market is defined for NIFTY 50 Total Return Index daily
2) Sharp Fall Definition :-  A daily close <- 2.0%
3) Entry condition :- Market close on signal at 3:25pm
4) Exit condition :-  Fixed holding window of 10 trading days.
5) Test period :- Jan 1,2010-Dec 31,2025
6) Regime Filters :- 200 day simple moving average
7) Frictional Cost :- 0.15 round trip   

Technology Choices :- This project was made fully in HTML to stick with the simplicity of deploying and debugging the code.

Key Assumptions :- 
1.	Tradability assumption: Since users cannot trade directly with the spot Nifty 50. We must assume trades to happen through ETFs or through front-month Nifty Futures. 
2.	Execution Timing :- An assumption is made when building the code to execute trades at the exact closing price or at the next trading day’s open.
3.	Dataset Assumption :- Depending on the dataset assumed i.e whether it is standard NIFTY dataset or NIFTY TRI dataset we assume whether a dividend has been paid out by a company or not.
4.	Overlapping Positions: If there are sharp falls which occur then the code must decide if it is going to execute another trade or whether it should just stick with the current trade until the exit rule is met.

Running the project :-
The project is can be opened with any standard web browser as it completely uses HTML

AI tools used :-
The AI tools mainly used in this are :- Claude & Gemini

Improvements that can be made :- 
Having more assumptions that can be made into the system to make it more realistic.
