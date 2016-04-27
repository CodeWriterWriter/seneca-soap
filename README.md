# Project Status :
This plugin is not being supported by the seneca organization,  and is no longer proven to work.
If you are interested in maintaining this project, please contact us via the issue queue.


options
-------

    {
      server: yourServer, // (optional) http server instance
      port: 8004, // (optional) if server is not set, one will be started on this port

    }


Usage
-----

    seneca.act({

        role: 'soap',

        cmd: 'register',

        name: 'myService'

        mappings: {

          apiName1: {
            role: 'myRole',
            cmd : 'myCmd'
          },

          apiName2: {
            role: '...',
            cmd : '...'
          }

        },

        wsdl: fs.readFileSync('./yourWsdl.wsdl')

      }, function(err) {

        // registered

      }
    )
