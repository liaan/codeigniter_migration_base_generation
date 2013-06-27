#Create a Base Migration File from current DB



When all goes well it will create a file under migrations called 001_create_base.php under your migrations folder


#To use:

1: Enable migrations and set version to 1;

2: In controller:


    function make_base(){

        $his->load->library('VpxMigration');

        // All Tables:

        $this->vpxmigration->generate();

        //Single Table:

        $this->vpxmigration->generate('table');

    }
    
