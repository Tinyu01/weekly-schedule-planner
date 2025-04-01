# Weekly Schedule Planner - Documentation

## Overview

The Weekly Schedule Planner is a console-based Java application designed to help users track their weekly schedule. The application presents a menu of days of the week, and based on the user's selection, displays the corresponding activities or tasks for that day. The application also features a special sub-menu for Monday that offers breakfast options with customized responses.

## Code Structure

The application consists of a single Java class named `Main` with the `main` method serving as the entry point. The program uses the `Scanner` class to collect user input from the console.

### Main Components

1. **Scanner Initialization**: Creates a Scanner object to read user input from the console.
2. **Day Selection**: Displays a menu of days of the week and prompts the user to select a day.
3. **Schedule Display**: Uses a switch statement to display the schedule for the selected day.
4. **Monday Sub-menu**: If Monday is selected, displays a sub-menu for breakfast options.
5. **Response Generation**: Based on the user's breakfast selection, displays a customized response.

## Implementation Details

### Class Structure

```java
public class Main {
    public static void main(String[] args) {
        // Program implementation
    }
}
```

### Variables

- `keyboard`: A Scanner object used to read user input from the console.
- `dayOfTheWeek`: An integer variable that stores the day of the week selected by the user (1-7).
- `subChoice`: An integer variable that stores the breakfast option selected by the user (only for Monday).

### Main Menu

The application displays a menu with the following options:
1. MONDAY
2. TUESDAY
3. WEDNESDAY
4. THURSDAY
5. FRIDAY
6. SATURDAY
7. SUNDAY

### Monday Sub-menu

If the user selects Monday (option 1), the application displays a sub-menu for breakfast options:
1. Yes, I had my breakfast
2. No, I would like one

### Response Logic

Based on the user's breakfast selection, the application displays one of the following responses:
- If option 1 is selected: "Good. Now you have a catchup meeting at 9AM. Prepare your notes."
- If option 2 is selected: "Let us divert on Highway 54 and have a Burger on the drive in."
- If any other option is selected: "NO such choice available."

## Workflow

1. The application starts and displays the main menu.
2. The user enters a number from 1-7 to select a day of the week.
3. The application displays the schedule for the selected day.
4. If Monday is selected, the application displays a sub-menu for breakfast options.
5. The user enters a number (1 or 2) to select a breakfast option.
6. The application displays a customized response based on the user's selection.
7. The application ends.

## Error Handling

The application includes basic error handling for invalid day selections. If the user enters a number outside the range of 1-7, the application displays an "Invalid day of the week" message.

For the Monday sub-menu, if the user enters a number other than 1 or 2, the application displays a "NO such choice available" message.

## Future Enhancements

Potential future enhancements for the application include:
- Adding more detailed schedules for each day of the week
- Implementing sub-menus for all days of the week
- Adding the ability to save and load schedules from a file
- Implementing a GUI for a more user-friendly experience
- Adding task prioritization and reminders