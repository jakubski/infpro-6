# Wersja okienkowa:

Klasy **MainWindow**i **ChatWidget** udost�pniaj� publicznie swoje obiekty *ui* logice komunikatora.

Ka�dy **ChatWindow** obs�uguje komunikacj� z jednym adresem IP. Posiada wska�nik na wid�et, w kt�rym si� ona odbywa oraz adres IP odbiorcy i *TcpSockety* do wysy�ania i odbierania wiadomo�ci. Obiekt mo�e zosta� zainicjowany na dwa sposoby: przez u�ytkownika nawi�zuj�cego po��czenie lub po zaakceptowaniu sygnalizowanego przez *QTcpServer* po��czenia przychodz�cego.

Klasa **Chat** uruchamia serwer odbieraj�cy nowe po��czenia. Tworzy nowe instancj� *Chat Window* wraz z przypisanymi im zak�adkami interfejsu graficznego, przekazuj�c im r�wnie� socket do odczytu wiadomo�ci. Posiada wska�nik na *MainWindow::ui*.