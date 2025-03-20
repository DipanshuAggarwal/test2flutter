#Firstly I added the files of JSON data and logo in assets folder 
Then firstly i use to make a top bar where the logo of bank is showing 
   {{centerTitle: true,
        backgroundColor: Colors.white, // Change the top bar color to white
        elevation: 0, // Remove shadow for a clean white look}}
Then i add the json data by code          Future<void> loadData() async {
    try {
      String accountsJson = await rootBundle.loadString('assets/accounts.json');
      final accountsData = json.decode(accountsJson);
      String transactionsJson = await rootBundle.loadString(
        'assets/transactions.json',
      );
      final transactionsData = json.decode(transactionsJson);
This is use to show the json data in the application 
Then i use the logo code Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Row(
          mainAxisAlignment: MainAxisAlignment.center,
          children: [
            Container(
              width: 120, // Set the width for the logo
              height: 120, // Set the height for the logo
              child: Image.asset(
                'assets/bank_logo.png',
                fit: BoxFit.contain,
              ), // Path to your logo
            ),
          ],  


          This tag is use to make the logo at the center top of the application..




# flutter_application_1

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
