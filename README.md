# nginx-http-errors

This is a work in progress...

Custom HTTP Error responses in a single file include

Include files in your nginx server conf file.

Add the definitions to your conf file, note that named location can only be listed on the server level of the conf file.

  include http-errors-def.conf;

Add the appropriate file to call the methods (these can be placed at the server level of the config, or can be placed in individual location blocks:

  include http-errors-html.conf;
  include http-errors-json.conf;
