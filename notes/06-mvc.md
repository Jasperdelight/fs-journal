# MVC

router => controller
appstate = stores all the data ( in the class ObservableAppState {} global variables ect.
new keyword builds out a new class of what was declared


1 Change router

2 set data in appState

3 set up controller that changes data (usually singleton) (starts with EXPORT class)=> constructor() {acts like functions that load on page)}(CoinsController)

4 change router controller to new controller made (IMPORT)(CoinsController)

5 the functions of chagning the data in the addcoin() function is not done by controller but by the SERVICE

6 Make (coins) Service (singleton) (going to be a class) THEN at bottom of page you export the const coinsService = new CoinService()

7 go back to function in coinController to call the CoinsService


8 bring in appState to (coins) Service (going to be a data type your pulling from appstate, then altering in the SERVICE)
AppState.coins++

9  SHOULD BE SET UP:  VIEW => CONTROLLER => SERVICE = MODEL(AppState)

10 Controller private functions go outside export I.E addcoins is exported but _drawcoins is hidden

11 New model File for new data. I.E coins app data and gachamon data can use an object as a parameter for constructor I.E. 
	constructor(data){
	this.name = data.name
	this.rarity = rarity.name}											

12 Back to Appstate to add gachamon to data. (import)
	gachamons = {													SERVICE IS WHERE YOU WRITE RULES
		new Gachamon=({name:'mikey", emoji: "", rarity: 'rare'})

13 Make Gachamon Controller to update values. START with export (export class GachamonsController) constructor to make sure its connecting.

14 Go back to Router and add the second controller

15 Every service starts with class then exporting as const then go back controller to

16 Getters go on model, always return something

Make functions on Controller. Then decalre it in Service

On event in controller constructor AppState.on('coins", _drawCoins) (whenever anything in coins changes, run the function of drawcoins)


Emit (manually trigger an event, then the event listener will fire)



