<html>

    <header>

    </header>
    
    <body>
    
        <?php echo

            $server = "localhost";
            $username = "usernamehere";
            $password = "passwordhere";
        
            // establishes connection to database
            $connection = mysqli_connect($server, $username, $password);
        
            if (!$connection) {
                die("Something went wrong with the connection to database!");
            }
        
            // replace query with correct SQL code
            $sql_query = mysqli_query("SELECT * FROM table");
        
            if (!$sql_query) {
                die("The SQL query you have entered is invalid!");
            }
        
            // retrieves information from database
            while ($row = mysqli_fetch_assoc($sql_query)) {
                echo $row;
            }
        
            // closes connection to database
            mysqli_close($connection);
    
        ?>
        
        
        <script>
            // must eventually use stringify function to see actual values
            // accesses SQL array on the front end to be used in JavaScript
            let sql_array = <?php echo json_encode($row) ?>
            
        </script>
    
    </body>
    
    <footer>
    
    </footer>

</html>
