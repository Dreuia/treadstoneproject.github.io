---
layout: post
title: "Tracethreat System Architecture."
description: "Tracing threat in device-system"
category: tracethreat
tags: [architecture]
---
{% include JB/setup %}

Server run in scanning mode supports PE files. Core server/client scanning support the Protobuf-message over network. In concept shared-memory contain a file types in PE. Plan to develop fast move the data to other process that manage internal malware quarantine. Now string of file in shared-memory used to scanning steps when scanning algorithm get all string of file to scan virus. Project use memory technique either shared memory or IPC contain string of file and virus signature before start scan a files. That internal memory contain fragment data technique available large file map to memory in millisecond. Boost library provides Boost.Interprocess source code. Interprocess able access pointer and index of memory regions map data to process after it's contain all data which push to data structure. Data structure contained in memory which add  Protobuf and single variable to its.Additional, Introprocess should take care multithread access to data structure.

<iframe src="https://drive.google.com/file/d/0B5Z4numXwfnAY2RLUTRKeXZpQ0k/preview" width="640" height="480"></iframe>

For Tracethreat project, It's main project front-end proceed infected data before send to databaase server(Mongo-RocksDB).


