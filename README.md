# time-converter
A script that converts time


def time_converter():
    while True:
        y = input("Please press 1 if you would like to use the seconds converter, 2 if you want to use the minutes \n"
                  "converter, press 3 to use the hours converter, 4 to use the days converter, 5, to use the years" "converter,\n"
"and 6 to quit ")
        if "1" in y:
            z = input("Would you like to convert minutes, hours, days, or years into seconds? ")
            if "days" in z:
                days = int(input("How many days would you like to convert to seconds? "))
                answer = str(days * 86400)
                print(answer + " seconds")
            elif "minutes" in z:
                minutes = int(input("How many minutes would you like to convert to seconds? "))
                answer = str(minutes * 60)
                print(answer + " seconds")
            elif "hours" in z:
                hours = int(input("How many hours would you like to convert to seconds? "))
                answer = str(hours * 3600)
                print(answer + " seconds")
            elif "years" in z:
                years = int(input("How many years would you like to convert to seconds? "))
                answer = str(years * 31536000)
                print(answer + " seconds")
        elif "2" in y:
            z = input("Would you like to convert seconds, hours, days, or years into minutes? ")
            if "days" in z:
                days = int(input("How many days would you like to convert to minutes? "))
                answer = str(days * 60 * 24)
                print(answer + " minutes")
            elif "seconds" in z:
                seconds = int(input("How many seconds would you like to convert to minutes? "))
                answer = str(seconds / 60)
                print(answer + " minutes")
            elif "hours" in z:
                hours = int(input("How many hours would you like to convert to minutes? "))
                answer = str(hours * 60)
                print(answer + " minutes")
            elif "years" in z:
                years = int(input("How many years would you like to convert to minutes? "))
                answer = str(years * 365 * 60 * 24)
                print(answer + " minutes")
        elif "3" in y:
            z = input("Would you like to convert seconds, minutes, days, or years into hours? ")
            if "days" in z:
                days = int(input("How many days would you like to convert to hours? "))
                answer = str(days * 24)
                print(answer + " hours")
            elif "seconds" in z:
                seconds = int(input("How many seconds would you like to convert to hours? "))
                answer = str(seconds / 3600)
                print(answer + " hours")
            elif "minutes" in z:
                minutes = int(input("How many minutes would you like to convert to hours? "))
                answer = str(minutes / 60)
                print(answer + " hours")
            elif "years" in z:
                years = int(input("How many years would you like to convert to hours? "))
                answer = str(years * 365 * 24)
                print(answer + " hours")
        elif "4" in y:
            z = input("Would you like to convert seconds, minutes, hours, or years into days? ")
            if "hours" in z:
                hours = int(input("How many hours would you like to convert to days? "))
                answer = str(hours / 24)
                print(answer + " days")
            elif "seconds" in z:
                seconds = int(input("How many seconds would you like to convert to days? "))
                answer = str(seconds / 3600 / 24)
                print(answer + " days")
            elif "minutes" in z:
                minutes = int(input("How many minutes would you like to convert to days? "))
                answer = str(minutes / 60 / 24)
                print(answer + " days")
            elif "years" in z:
                years = int(input("How many years would you like to convert to days? "))
                answer = str(years * 365)
                print(answer + " days")
        elif "5" in y:
            z = input("Would you like to convert seconds, minutes, hours, or days into years? ")
            if "hours" in z:
                hours = int(input("How many hours would you like to convert to years? "))
                answer = str(hours / 24 / 365)
                print(answer + " years")
            elif "seconds" in z:
                seconds = int(input("How many seconds would you like to convert to years? "))
                answer = str(seconds / 3600 / 24 / 365)
                print(answer + " years")
            elif "minutes" in z:
                minutes = int(input("How many minutes would you like to convert to years? "))
                answer = str(minutes / 60 / 24 / 365)
                print(answer + " years")
            elif "days" in z:
                years = int(input("How many days would you like to convert to years? "))
                answer = str(years / 365)
                print(answer + " years")
        else:
            break
