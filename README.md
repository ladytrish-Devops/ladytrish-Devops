-#!/bin/bash

# Prompt the user to enter a number
echo "Enter a number:"
read number

# Check if the number is positive, negative, or zero
if [ $number -gt 0 ]; then
    echo "The number is positive."
elif [ $number -lt 0 ]; then
    echo "The number is negative."
else
    echo "The number is zero."
fi




#!/bin/bash

# Check if an argument is provided
if [ $# -eq 0 ]; then
    echo "Usage: $0 {start|stop|restart|status}"
    exit 1
fi

case "$1" in
    start)
        echo "Starting the service..."
        # Commands to start the service
        ;;
    stop)
        echo "Stopping the service..."
        # Commands to stop the service
        ;;
    restart)
        echo "Restarting the service..."
        # Commands to restart the service
        ;;
    status)
        echo "Checking the status of the service..."
        # Commands to check the status of the service
        ;;
    *)
        echo "Usage: $0 {start|stop|restart|status}"
        exit 1
        ;;
esac

exit 0
ls
