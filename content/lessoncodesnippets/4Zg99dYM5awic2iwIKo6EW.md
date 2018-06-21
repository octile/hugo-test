+++
curl = "export CPA_TOKEN='<cpa_token>';\nexport SPACE_ID='<space_id>';"
dotNet = "var httpClient = new HttpClient();\nvar client = new ContentfulClient(httpClient, \"\", \"<cpa_token>\", \"<space_id>\", usePreviewApi: true);"
java = "final CDAClient client =\n \u00a0\u00a0\u00a0CDAClient\n \u00a0\u00a0\u00a0\u00a0\u00a0\u00a0\u00a0.builder()\n \u00a0\u00a0\u00a0\u00a0\u00a0\u00a0\u00a0.setToken(\"<cpa_token>\")\n \u00a0\u00a0\u00a0\u00a0\u00a0\u00a0\u00a0.preview()\n \u00a0\u00a0\u00a0\u00a0\u00a0\u00a0\u00a0.setSpace(\"<space_id>\")\n \u00a0\u00a0\u00a0\u00a0\u00a0\u00a0\u00a0.build();"
javaAndroid = "final CDAClient client =\n \u00a0\u00a0\u00a0CDAClient\n \u00a0\u00a0\u00a0\u00a0\u00a0\u00a0\u00a0.builder()\n \u00a0\u00a0\u00a0\u00a0\u00a0\u00a0\u00a0.setToken(\"<cpa_token>\")\n \u00a0\u00a0\u00a0\u00a0\u00a0\u00a0\u00a0.preview()\n \u00a0\u00a0\u00a0\u00a0\u00a0\u00a0\u00a0.setSpace(\"<space_id>\")\n \u00a0\u00a0\u00a0\u00a0\u00a0\u00a0\u00a0.build();"
javascript = "const contentful = require('contentful')\nconst client = contentful.createClient({\n \u00a0space: '<space_id>',\n \u00a0accessToken: '<cpa_token>',\n \u00a0host: 'preview.contentful.com'\n})"
php = "$client = new \\Contentful\\Delivery\\Client(\n    '<cpa_token>',\n    '<space_id>',\n    true\n);"
python = "import contentful\n\nclient = contentful.Client('<space_id>', '<cpa_token>', api_url='preview.contentful.com')"
ruby = "require ‘contentful’\n\nclient = Contentful::Client.new(\n \u00a0space: '<space_id>',\n \u00a0access_token: '<cpa_token>',\n \u00a0dynamic_entries: :auto,\n \u00a0api_url: 'preview.contentful.com',\n \u00a0raise_errors: true\n)"
swift = "var configuration = ClientConfiguration()\nconfiguration.previewMode = true\n\n// Retain the client as a property on a type you define so that \n// the client's asynchronous network callbacks are executed.\nlet client = Client(spaceId: \"<space_id>\", accessToken: \"<cpa_token>\")"
title = "Fetch draft content > code"
+++
