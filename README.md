jboss-learning
==============

One JBoss project a day, keep doctor away :-)

## Aero Gear

When building mobile web apps, it is important to have lightweight, 
performant code that gives a great experience to your users no matter
what device they might be using. That is where AeroGear.js comes in. 
This library provides everything from a simple persistence layer to 
a security API and everything in between.

	$.when( save1, save2 ).done( function( s1, s2 ) {
	    var save3, save4;

	    save3 = pipe.save({
	        id: 11223,
	        title: "Updated Task",
	        date: "2012-08-01"
	    },
	    {
	        success: function( data, textStatus, jqXHR ) {
	            ok( true, "PUT - update existing data" );
	        }
	    });

	    save4 = pipe2.save({
	        taskId: 44556,
	        title: "Another Updated Task",
	        date: "2012-08-01"
	    },
	    {
	        success: function( data, textStatus, jqXHR ) {
	            ok( true, "PUT - update existing data with custom record id" );
	        }
	    });

	    $.when( save3, save4 ).done( function( s3, s4 ) {
	        start();
	    });
	});

