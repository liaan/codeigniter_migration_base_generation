codeigniter_migration_base_generation
=====================================

Create a Base Migration File from current DB

Creates a file under migrations called 001_create_base.php


To use:
Enable migrations and set version to 1;

in controller:

function make_base(){
    $this->load->library('VpxMigration');

    /*  export all tables */
      $this->vpxmigration->generate();
    /* OR export 1 table */
    $this->vpxmigration->generate('table');

}

