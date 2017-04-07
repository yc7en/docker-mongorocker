docker-mongorocker fork
=======================

Just the original docker with some features for customization.

set `$MONGO["servers"][$i]["mongo_auth"] = true;` in `config.php`. So login with user your admin user/pass. 

Usually mongoDB is installed without admin as default. You should add admin user/pass first. You can try mongo command as follows:

	use admin
	db.createUser({user:"root",pwd:"root123",roles:["userAdminAnyDatabase"]}) 

Then you can use root/root123 to login.

