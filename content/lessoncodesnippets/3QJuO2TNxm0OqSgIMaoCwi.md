+++
curl = "curl -H 'Authorization: Bearer '$CDA_TOKEN 'https://cdn.contentful.com/spaces/'$SPACE_ID'/entries/'"
dotNet = "var entry = await client.GetEntries<dynamic>();\n\nConsole.WriteLine(entry.ToString());"
java = "final CDAArray all =\n    client\n        .fetch(CDAEntry.class)\n        .all();\n\nSystem.out.println(all);\n"
javaAndroid = "client\n    .observe(CDAEntry.class)\n    .all()\n    .observeOn(AndroidSchedulers.mainThread())\n    .subscribeOn(io.reactivex.schedulers.Schedulers.io())\n    .subscribe(\n        new DisposableSubscriber<CDAArray>() {\n          CDAArray result;\n\n          @Override public void onComplete() {\n            new AlertDialog.Builder(context)\n                .setTitle(\"Contentful\")\n                .setMessage(result.toString())\n                .show();\n          }\n\n          @Override public void onError(Throwable e) {\n            // Handle error case.\n            new AlertDialog.Builder(context)\n                .setTitle(\"Contentful\")\n                .setMessage(\"An error occurred: \" + e.toString())\n                .show();\n          }\n\n          @Override public void onNext(CDAArray array) {\n            // Array received, maybe more to come.\n            result = entry;\n          }\n        }"
javascript = "client.getEntries()\n.then((response) => console.log(response))"
php = "$entries = $client->getEntries();\n\nvar_dump($entries);"
python = "entries = client.entries()\nprint(repr(entries))"
ruby = "entries = client.entries()\nputs(entries)"
swift = "client.fetchEntries() { (result: Result<ArrayResponse<Entry>>) in\n \u00a0\u00a0\u00a0switch result {\n \u00a0\u00a0\u00a0\u00a0\u00a0\u00a0\u00a0case .success(arrayResponse):\n            let entries = arrayResponse.items\n \u00a0\u00a0\u00a0\u00a0\u00a0\u00a0\u00a0\u00a0\u00a0\u00a0\u00a0print(entries)\n \u00a0\u00a0\u00a0\u00a0\u00a0\u00a0\u00a0case .error(let error):\n \u00a0\u00a0\u00a0\u00a0\u00a0\u00a0\u00a0\u00a0\u00a0\u00a0\u00a0print(\"Error \\(error)!\")\n \u00a0\u00a0\u00a0}\n}"
title = "Fetch all entries > code"
+++
