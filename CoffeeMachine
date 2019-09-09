package machine;
import java.util.Scanner;

public class CoffeeMachine {
          public static void main(String[] args) {
            int water = 400;
            int milk = 540;
            int beans = 120;
            int dCups = 9;
            int money = 550;
            int cups = 1;
            boolean running;

            Scanner myScanner = new Scanner(System.in);

            do {
                running = true;
                System.out.println("Write action (buy, fill, take, remaining, exit):");
                String action = myScanner.nextLine();
                switch (action){
                    case "buy":
                        System.out.println("What do you want to buy? 1 - espresso, 2 - latte, 3 - cappuccino: 3, back - to main menu:");
                        String drink = myScanner.nextLine();
                        switch (drink) {
                            case "1":
                                if (((cups * 250) > water)){
                                    System.out.println("Sorry, not enough water!");
                                } else if (((cups * 16) > beans)) {
                                    System.out.println("Sorry, not enough beans!");
                                } else {
                                    System.out.println("I have enough resources, making you a coffee!");
                                    water = water - (cups * 250);
                                    beans = beans - (cups * 16);
                                    money = money + (cups * 4);
                                    dCups = dCups - 1;
                                }
                                break;
                            case "2":
                                if (((cups * 350) > water)) {
                                    System.out.println("Sorry, not enough water!");
                                } else if (((cups * 75) > milk)) {
                                    System.out.println("Sorry, not enough milk!");
                                } else if (((cups * 20) > beans)) {
                                    System.out.println("Sorry, not enough beans!");
                                } else {
                                    System.out.println("I have enough resources, making you a coffee!");
                                    water = water - (cups * 350);
                                    milk = milk - 75;
                                    beans = beans - (cups * 20);
                                    money = money + (cups * 7);
                                    dCups = dCups - 1;
                                }
                                break;
                            case "3":
                                if (((cups * 200) > water)) {
                                    System.out.println("Sorry, not enough water!");
                                } else if (((cups * 100) > milk)) {
                                    System.out.println("Sorry, not enough milk!");
                                } else if (((cups * 12) > beans)) {
                                    System.out.println("Sorry, not enough beans!");
                                } else {
                                    System.out.println("I have enough resources, making you a coffee!");
                                    water = water - (cups * 200);
                                    milk = milk - (cups * 100);
                                    beans = beans - (cups * 12);
                                    money = money + (cups * 6);
                                    dCups = dCups - 1;
                                }
                                break;
                            case "back":
                        }
                        break;
                    case "fill":
                        System.out.println("Write how many ml of water do you want to add:");
                        water = water + myScanner.nextInt();
                        System.out.println("Write how many ml of milk do you want to add:");
                        milk = milk + myScanner.nextInt();
                        System.out.println("Write how many grams of coffee beans do you want to add:");
                        beans = beans + myScanner.nextInt();
                        System.out.println("Write how many disposable cups of coffee do you want to add:");
                        dCups = dCups + myScanner.nextInt();

                        break;

                    case "take":
                        System.out.println("I gave you " + money);
                        money = money - money;
                        break;

                    case "remaining":
                        System.out.println("The coffee machine has:"
                                +"\n"+ water + " of water"
                                +"\n"+ milk + " of milk"
                                +"\n"+ beans + " of coffee beans"
                                +"\n"+ dCups + " of disposable cups"
                                +"\n$"+ money + " of money"
                                +"\n");
                        break;

                    case "exit":
                        running = false;
                        break;
                }

            } while (running);
        }
    }


