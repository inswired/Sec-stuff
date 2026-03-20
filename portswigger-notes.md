Sql injection-
   Lab 1-goal-"using the WHERE clause to retreive hidden data"
    task-find the hidden products in the websiting  through sql injection in the product category
    solution- adding '+OR+1=1-- at the end of the category portion to the URL to gain access to the hidden listings
    why-
      " ' " ends the string so u can start adding ur own sql commands
      "OR 1=1" means true so it makes the sql command remove the filters and show everything
      "--" means comment so it makes it ignore everything after typing that portion 


   Lab 2- goal- getting acess to a users account through sql injection
      task-logging into the administrators account without using the password
      solution- skipping the password field entirely by commenting it out by adding comment at the end of the username "administrator'--"
      why- after adding a comment at the end of the username we skip rest of the sql commend so we do a search in the database with just the username and skip the password and the ' ebfr closes the previous string so the comment isnt considered past of the searched username
