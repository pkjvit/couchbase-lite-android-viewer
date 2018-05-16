# couchbase-lite-android-viewer

**Couchbase Lite Android Viewer** is a sdk tool provide for Couchbase Lite Android 1.4 Applications to view all databases and query on them using smart query templates.

## Functionality
- Show all couchbase databases
- Show all tables of selected database
- Gives a console where you can query on selected table
- Provide *Smart Query Templates* which gives you predefined queries on the fly
- Shows queried data in a page of size 50 rows, for large data you can go particular page on the go using bottom ![Pagination view](https://github.com/pkjvit/PaginationView)

![CbliteViewer](https://github.com/pkjvit/couchbase-lite-android-viewer/blob/master/screenshots/cblite_viewer_250x.gif)

## Requirements

- Android 4.1+
- Android Studio 3.0

## Installation

Add the following in the dependencies section of the application's build.gradle (the one in the app folder).

```
    compile 'com.pkj.wow.cblite.viewer:couchbase-lite-android-viewer:0.1.1-5'
    
    // dependencies
    compile 'com.pkj.wow.paginationview:PaginationView:1.0.2-5'
    compile 'de.codecrafters.tableview:tableview:2.8.0'
    compile 'com.android.support.constraint:constraint-layout:1.0.2'
```

## Usage

To view your all database's it needs couchbase Manager and start will redirect to screen which have all data and sync information regarding manger.

```
// Initialise by passing activity context and couchbase Manager
CbLiteViewer cbLiteViewer = CbLiteViewer.instance(mContext, mManager);
                
// Start will show database screen
cbLiteViewer.start();
```


## Licence
    Copyright 2018 Pankaj Jangid

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
