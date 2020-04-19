# baby_names

Codelab exercise link: https://codelabs.developers.google.com/codelabs/flutter-firebase/

Learnt to:
- add a firebase cloud package, cloud_firestore 
- create dummy json of snapshot of document and build UI
- Setup firebase:
  - add schema, called project
  - allow access to the project by adding app/web bundle
  - configure app to interact with firebase, add file GoogleService-Info.plist
  - create database
  - create table, called collection, baby
  - create rows, called document, doc_id
- replace dummySnap with data read from firebase, 
  - use StreamBuilder
  - stream: Firestore.instance.collection('baby').snapshots(),

- to write back:
  - onTap: () => record.reference.updateData({'key': new_value})
- now its all linked from front to back
- all sync and update offline and online.
