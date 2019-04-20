---
title:  "DICEBOT WIN SCRIPT FOR YOLODICE, PRIMEDICE, STAKE, Nitrogames"
date:   2013-11-10 10:18:00
description: DICEBOT WIN SCRIPT FOR YOLODICE, PRIMEDICE, STAKE, Nitrogames
---




### SCRIPT (COPY & PASTE)


```
chance = 95
base =   (balance/280000)
base2 = (balance/280000)
nextbet = base
prof = 0
stage = 2
stopnow = false
prof2 = 0
phase = 1
lowest = 99
bethigh = false
lossstreak = 1
biggest = 0
counter = 0
lossess = 0
first = true
phase = 1
buffer = 0
bigprof = 0
counter2 = 0
losers = 0

function dobet()
	counter2 += 1
	prof += currentprofit
	if phase == 1 then
		if win then
			first = true
			lossess = 0
			base = (balance/380000)
			nextbet = base/2
			chance = 33
			stage = 3
			prof = 0
			counter = 0
		else
			lossess += 1
			counter += 1
			if (counter+1) >= stage then
				stage += 1
				counter = 0
			end
			chance = (99/stage)
			nextbet = (((prof+(base*(currentstreak-1)))/((99/chance)-1))*-1) 
			if currentstreak <= -22  then
				if first == true then
					first = false
					buffer = prof/33
					stage = 3
					chance = (99/stage)
					nextbet = buffer*-1
					phase = 2
					counter = 1
					prof2 = buffer
				end
			end
		end
	else
		prof2 += currentprofit
		if win then
			stage = 3
			chance = (99/stage)
			nextbet = buffer*-1
			prof2 = buffer
		else
			counter += 1
			if counter >= stage then
				stage += 1
				counter = 0
			end
			chance = (99/stage)
			nextbet = ((prof2/((99/chance)-1))*-1)/1.05
		end
		if prof >= base*60 then
			phase = 1
			first = true
			lossess = 0
			nextbet = base
			chance = 33			                                stage = 3
			prof = 0
			counter = 0
		end
	end
	
	if nextbet <= base2 then
		nextbet = base2
	end
	if stopnow == true and win then
		stop()
	end

	if balance >= biggest then
		biggest = balance
	end
	
	if prof <= bigprof then
		bigprof = prof
	end
	
	if currentstreak <= losers then
		losers = currentstreak
	end

	if currentstreak < -25  then
                prof = 0
	end


	if counter2 > 100   then
                counter2 = 1
		print("")
		print("")
		print("Biggest Loss: "..bigprof)
		print("Big  Balance: "..biggest)
		print("Balance: "..balance)
		print("Most Losses: "..losers)
		print("Losses: "..prof)
		print("Modephase : "..phase)
	end	

end
```
