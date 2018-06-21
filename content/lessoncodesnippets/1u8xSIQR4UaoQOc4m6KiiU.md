+++
curl = "export CDA_TOKEN='<access_token>';\nexport SPACE_ID='<space_id>';"
dotNet = "var httpClient = new HttpClient();\nvar client = new ContentfulClient(httpClient, \"<access_token>\", \"\", \"<space_id>\");"
java = "final CDAClient client =\n    CDAClient\n        .builder()\n        .setToken(\"<access_token>\")\n        .setSpace(\"<space_id>\")\n        .build();\n"
javaAndroid = "final CDAClient client =\n    CDAClient\n        .builder()\n        .setToken(\"<access_token>\")\n        .setSpace(\"<space_id>\")\n        .build();\n"
javascript = "const contentful = require('contentful')\nconst client = contentful.createClient({\n  space: '<space_id>',\n  accessToken: '<access_token>'\n})\n"
php = "$client = new \\Contentful\\Delivery\\Client(\n    '<access_token>',\n    '<space_id>'\n);"
python = "import contentful\n\nclient = contentful.Client('<space_id>', '<access_token>')\n"
ruby = "require ‘contentful’\n\nclient = Contentful::Client.new(\n \u00a0space: '<space_id>',\n \u00a0access_token: '<access_token>',\n \u00a0dynamic_entries: :auto,\n \u00a0raise_errors: true\n)"
swift = "import Contentful\n\nlet client = Client(spaceId: \"<space_id>\", \n                    accessToken: \"<access_token>\")"
title = "SDK basics > SDK initialization - code"
+++
