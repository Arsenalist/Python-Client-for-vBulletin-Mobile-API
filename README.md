Python-Client-for-vBulletin-Mobile-API
======================================

Python Client for vBulletin Mobile API

	from vbulletin import Vbulletin
	client_options = {
	    'apikey': 'GETFROMVBULLETIN',
	    'forumurl': 'http://www.raptorsrepublic.com/forums',
	    'clientname': 'someclient',
	    'clientversion': '1',
	    'platformname': '1',
	    'platformversion': '1',
	    'uniqueid': 'someuniqueid'
	}

	v = Vbulletin(client_options)
	v.login('YOURUSERNAME', 'YOURPASSWORD')
	# forum id, subject, message
	v.post_new_thread('13', 'This is a subject.', 'This is a message.')
