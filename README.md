# file-server
simple light-weigt node.js file server.

Provides web api for making basic things with files in directory: observe directory, insert/delete/modify files.

Example usage:
npm file-server serve ./directory --port 1234

Api (example)

-- Gets the file
url: <hostname>/filename
{
  method: 'GET'
}

-- Creates file with name <filename> in path, relative to serving directory
url: <hostname>/path/to/file/filename
{
  method: 'PUT'
}


-- Updates file with name <filename>
url: <hostname>/filename
{
  method: 'UPDATE',
  
}

-- Deletes file
url: <hostname>/filename
{
  method: 'DELETE'
}
