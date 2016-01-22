# Codeigniter
Added Codeigniter.
Change My Route file welcome to error (default_controller)

Added config file in application/config/email_error.php
	change $config['email_from'] & $config['email_to'] to Yours.

added code in base root/system/core/Exceptions.php log_exception() 

		$buffer = $this->show_php_error($severity, $message, $filepath, $line);
		$this->sendEmails("A PHP $severity was encountered",$buffer);

change echo into return in show_php_error()


create Function for send mail sendEmails()

