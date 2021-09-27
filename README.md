# JsonFile-2-Memcache-Loader
This tool, ships data to a specified memcache servers
Author: Hud Seidu Daannaa
    README.md
    =========
    This tool, ships data to a specified memcache servers in settings.ini,
    Data is send in parallel, hence this is done to produce availability and
    redundency. a folder is created during operation of the program, which heps
    to save the applications state. the absence of that folder, will trigger the application
    to start all over again (as a new start).
    IMPORTANT: All commands or flags, initiated, will apply to all servers.
    the application takes a file as input. this file should contain data of the
    form:
    'key':'value' # hence the key, values should be strings.
    HENCE, THIS TOOL, TAKES JSON AS INPUT, THIS MEANS TO SEND DATA INTO MEMCACHE,
    TH TEXT FILE LOADED SHOULD BE JSON. OF THE FORM:
        {'name':'hud'}
        {'age':'x~2'}
    //the above format should be the content of the text file ...

    form the settings.ini file, you can specify the key (document_key_field) to 
    use within the documents in the file

    to run tool:
    chmod +x x1.py
    ./x1.py or

    python ./x1.py

    NOTE: use --help to view flags
