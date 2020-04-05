# Record-Manager

-->Steps to run this project:
    1.Open command prompt and go to project directory

    2.Type ls command to check if we are in the right directory

    3.Run "make clean " command to clear the .o files

    4.Run "make" command to compile the project

    5.Run "make run" to execute the project

    6.Run "make test_expr" to compile test expression related files

    7.Run "make run_expr" to to run test_expr.c files

-->Table and manager functions
    1.initRecordManager ()
        to initialize the record manager

    2.shutdownRecordManager()
        shuts down the record manager and deallocated the the resources allocated to it

    3.createTable()
        Opens a table and then creates a page file, opens page file, writes the block containing the table in the page file and closes it

    4.openTable()
        Creates a table with name and schema as specified in the parameter

    5.closeTable()
        Closes the table as pointed by the parameter

    6.deleteTable()
        Deletes the table that is specified as a parameter

    7.getNumTuples()
        returns the number of tuples for the specified table

-->Handeling records functions
    1.insertRecord()
        Inserts a record in a table

    2.deleteRecord()
        Deletes the record of the table

    3.updateRecord()
        Updates the records of the table using the given parameter record and table

    4.getRecord()
        Retrives the record using the id.

-->Scan functions
    1.startScan()
        Starts the scan by retriveing the data from the data structure

    2.next()
        Returns the next tuple that satisfies the condition

    3.closeScan()
        Closes the sacn operation.Also deallocate the space

-->Schema functions
    1.getRecordSize()
        Returns the size of the record in the schema specified.

    2.freeSchema()
        Removes the schema

    3.createSchema()
        Creates a new schema using the specifications given in the parameter

-->Attribute function()
    1.createRecord()
        Creates a new record in the schema that is specified in the parameter

    2.attrOffset()
        Sets the offset from the intial position (in bytes)

    3.freeRecord()
        De-allocated the memory space that is allocated to the record

    4.getAttr()
        Retrives the attribute from the given record

    5.setAttr()
        Set the attribute for the record in the specified schema
