HaPi
====

Harvest API PHP Interface (HaPi)

Harvest users can use the Harvest API to query and utilize information from their Harvest account in their own applications.  This Open Source library is licensed under the GNU General Public License v3 license.

The current version of the library is 1.1.1. This release contains support for the full Time Tracking and Extended Rest APIs and requires the user to have cURL support. In addition this version of the library contains the HarvestReports object which can be used to perform additional queries like getActiveProjects and getActiveTimers. Please visit the downloads page to download the latest version of the library.

    // require the Harvest API core class 
    require_once( PATH_TO_LIB . '/HarvestAPI.php' );
    
    // register the class auto loader 
    spl_autoload_register( array('HarvestAPI', 'autoload') );
    
    // instantiate the api object 
    $api = new HarvestAPI(); 
    $api->setUser( "user@email.com" ); 
    $api->setPassword( "password" ); 
    $api->setAccount( "account" ); 