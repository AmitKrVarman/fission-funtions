# Fission Fuction

This API accepts TYPE FORM request JSON as input and transforms it to return JSON output compliant to Fresh Desk JSON to create a new Ticket

Request Payload
`{
	"event_id": "wLMhymGRLT",
	"event_type": "form_response",
	"form_response": {
		"form_id": "krCLZ1",
		"token": "92340b083bb287c3cbc2aabf9d78eff7",
		"submitted_at": "2017-10-12T11:50:47Z",
		"hidden": {
			"email": "amitkumarvarman@gmail.com"
		},
		"definition": {
			"id": "krCLZ1",
			"title": "TV claim",
			"fields": [{
				"id": "WwzqHPb0K9Wv",
				"title": "Make of the TV",
				"type": "short_text",
				"allow_multiple_selections": false,
				"allow_other_choice": false
			}, {
				"id": "lGCVB9tse6Re",
				"title": "Model number of the TV",
				"type": "short_text",
				"allow_multiple_selections": false,
				"allow_other_choice": false
			}, {
				"id": "63241151",
				"title": "Please upload a detailed image of the damage",
				"type": "file_upload",
				"allow_multiple_selections": false,
				"allow_other_choice": false
			}, {
				"id": "63241330",
				"title": "When did the incident happen?",
				"type": "date",
				"allow_multiple_selections": false,
				"allow_other_choice": false
			}, {
				"id": "XiKbgOrX1OAp",
				"title": "Do you still have the TV in your possession?",
				"type": "yes_no",
				"allow_multiple_selections": false,
				"allow_other_choice": false
			}, {
				"id": "63241939",
				"title": "We have made the following assumptions about your property, you and anyone living with you",
				"type": "legal",
				"allow_multiple_selections": false,
				"allow_other_choice": false
			}, {
				"id": "XdVgAjnucXRP",
				"title": "Was there a theft or a deliberate event by a 3rd party?",
				"type": "yes_no",
				"allow_multiple_selections": false,
				"allow_other_choice": false
			}, {
				"id": "63241542",
				"title": "If you have any other insurance or warranties covering your TV, please advise us of the company name.",
				"type": "short_text",
				"allow_multiple_selections": false,
				"allow_other_choice": false
			}, {
				"id": "63241572",
				"title": "Are you aware of anything else relevant to your claim that you would like to advise us of at this stage?",
				"type": "long_text",
				"allow_multiple_selections": false,
				"allow_other_choice": false
			}, {
				"id": "QYabj3uz2gs9",
				"title": "In as much detail as possible, please provide a full written account of what has happened to your TV, including where it happened.",
				"type": "long_text",
				"allow_multiple_selections": false,
				"allow_other_choice": false
			}, {
				"id": "u2dzBoYFjbRA",
				"title": "Serial number of the TV",
				"type": "short_text",
				"allow_multiple_selections": false,
				"allow_other_choice": false
			}, {
				"id": "63391165",
				"title": "What was the purchase price of the TV?",
				"type": "number",
				"allow_multiple_selections": false,
				"allow_other_choice": false
			}]
		},
		"answers": [{
			"type": "text",
			"text": "Samsung",
			"field": {
				"id": "WwzqHPb0K9Wv",
				"type": "short_text"
			}
		}, {
			"type": "text",
			"text": "QLED 55\"",
			"field": {
				"id": "lGCVB9tse6Re",
				"type": "short_text"
			}
		}, {
			"type": "file_url",
			"file_url": "https://admin.typeform.com/form/results/file/download/krCLZ1/63241151/495c05215011-broken_Vizio_LCD_TV.JPG",
			"field": {
				"id": "63241151",
				"type": "file_upload"
			}
		}, {
			"type": "date",
			"date": "2018-12-12",
			"field": {
				"id": "63241330",
				"type": "date"
			}
		}, {
			"type": "boolean",
			"boolean": true,
			"field": {
				"id": "XiKbgOrX1OAp",
				"type": "yes_no"
			}
		}, {
			"type": "boolean",
			"boolean": true,
			"field": {
				"id": "63241939",
				"type": "legal"
			}
		}, {
			"type": "boolean",
			"boolean": false,
			"field": {
				"id": "XdVgAjnucXRP",
				"type": "yes_no"
			}
		}, {
			"type": "text",
			"text": "no",
			"field": {
				"id": "63241542",
				"type": "short_text"
			}
		}, {
			"type": "text",
			"text": "no",
			"field": {
				"id": "63241572",
				"type": "long_text"
			}
		}, {
			"type": "text",
			"text": "Tv broke... smashed to bits",
			"field": {
				"id": "QYabj3uz2gs9",
				"type": "long_text"
			}
		}, {
			"type": "text",
			"text": "Don't have it",
			"field": {
				"id": "u2dzBoYFjbRA",
				"type": "short_text"
			}
		}, {
			"type": "number",
			"number": 1900,
			"field": {
				"id": "63391165",
				"type": "number"
			}
		}]
	}
}`  
Response JSON

`{"email":"amitkumarvarman@gmail.com","subject":"TV claim","description":" \n Make of the TV : Samsung \n Model number of the TV : QLED 55\" \n Please upload a detailed image of the damage :  \n When did the incident happen? :  \n Do you still have the TV in your possession? :  \n We have made the following assumptions about your property, you and anyone living with you :  \n Was there a theft or a deliberate event by a 3rd party? :  \n If you have any other insurance or warranties covering your TV, please advise us of the company name. : no \n Are you aware of anything else relevant to your claim that you would like to advise us of at this stage? : no \n In as much detail as possible, please provide a full written account of what has happened to your TV, including where it happened. : Tv broke... smashed to bits \n Serial number of the TV : Don't have it \n What was the purchase price of the TV? : ","status":2,"priority":1,"name":"TEST NAME"}`

