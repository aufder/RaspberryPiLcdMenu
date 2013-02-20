#! /bin/sh
# /etc/init.d/lcdmenuinit

case "$1" in
  start)
    echo "Starting lcdmenu"
    cd /home/pi/lcdmenu
    sudo /usr/bin/python /home/pi/lcdmenu/lcdmenu.py &
  ;;
  stop)
    echo "Stopping lcdmenu"
    killall python
    ;;
  *)
    echo "Usage: /etc/init.d/lcdmenuinit {start|stop}"
    exit 1
    ;;
esac

exit 0
