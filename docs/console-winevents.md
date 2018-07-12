---
title: Console WinEvents
description: The following event constants are used in the event parameter of the WinEventProc callback function. For more information, see WinEvents.
author: bitcrazed
ms.author: richturn
ms.topic: article
ms.prod: console
keywords: console, character mode applications, command line applications, terminal applications, console api
MS-HAID:
- '\_win32\_console\_winevents'
- 'base.console\_winevents'
- 'consoles.console\_winevents'
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/desktop'
ms.assetid: b7078b2d-5508-4e42-bac2-34b70f1856e2
topic_type:
- apiref
api_name:
- EVENT_CONSOLE_CARET
- EVENT_CONSOLE_END_APPLICATION
- EVENT_CONSOLE_LAYOUT
- EVENT_CONSOLE_START_APPLICATION
- EVENT_CONSOLE_UPDATE_REGION
- EVENT_CONSOLE_UPDATE_SCROLL
- EVENT_CONSOLE_UPDATE_SIMPLE
api_location:
- Winuser.h
api_type:
- HeaderDef
---

# Console WinEvents


The following event constants are used in the *event* parameter of the [*WinEventProc*](https://msdn.microsoft.com/en-us/library/windows/desktop/dd373885(v=vs.85).aspx) callback function. For more information, see [WinEvents](https://msdn.microsoft.com/library/windows/desktop/dd373889).

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Constant/value</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span id="EVENT_CONSOLE_CARET"></span><span id="event_console_caret"></span>
<strong>EVENT_CONSOLE_CARET</strong>
0x4001</td>
<td><p>The console caret has moved. The <em>idObject</em> parameter is one or more of the following values: <strong>CONSOLE_CARET_SELECTION</strong> or <strong>CONSOLE_CARET_VISIBLE</strong>.</p>
<p>The <em>idChild</em> parameter is a <a href="coord-str.md"><strong>COORD</strong></a> structure that specifies the cursor&#39;s current position.</p></td>
</tr>
<tr class="even">
<td><span id="EVENT_CONSOLE_END_APPLICATION"></span><span id="event_console_end_application"></span>
<strong>EVENT_CONSOLE_END_APPLICATION</strong>
0x4007</td>
<td><p>A console process has exited. The <em>idObject</em> parameter contains the process identifier of the terminated process.</p></td>
</tr>
<tr class="odd">
<td><span id="EVENT_CONSOLE_LAYOUT"></span><span id="event_console_layout"></span>
<strong>EVENT_CONSOLE_LAYOUT</strong>
0x4005</td>
<td><p>The console layout has changed.</p></td>
</tr>
<tr class="even">
<td><span id="EVENT_CONSOLE_START_APPLICATION"></span><span id="event_console_start_application"></span>
<strong>EVENT_CONSOLE_START_APPLICATION</strong>
0x4006</td>
<td><p>A new console process has started. The <em>idObject</em> parameter contains the process identifier of the newly created process. If the application is a 16-bit application, the <em>idChild</em> parameter is <strong>CONSOLE_APPLICATION_16BIT</strong> and <em>idObject</em> is the process identifier of the NTVDM session associated with the console.</p></td>
</tr>
<tr class="odd">
<td><span id="EVENT_CONSOLE_UPDATE_REGION"></span><span id="event_console_update_region"></span>
<strong>EVENT_CONSOLE_UPDATE_REGION</strong>
0x4002</td>
<td><p>More than one character has changed. The <em>idObject</em> parameter is a <a href="coord-str.md" data-raw-source="[&lt;strong&gt;COORD&lt;/strong&gt;](coord-str.md)"><strong>COORD</strong></a> structure that specifies the start of the changed region. The <em>idChild</em> parameter is a <strong>COORD</strong> structure that specifies the end of the changed region.</p></td>
</tr>
<tr class="even">
<td><span id="EVENT_CONSOLE_UPDATE_SCROLL"></span><span id="event_console_update_scroll"></span>
<strong>EVENT_CONSOLE_UPDATE_SCROLL</strong>
0x4004</td>
<td><p>The console has scrolled. The <em>idObject</em> parameter is the horizontal distance the console has scrolled. The <em>idChild</em> parameter is the vertical distance the console has scrolled.</p></td>
</tr>
<tr class="odd">
<td><span id="EVENT_CONSOLE_UPDATE_SIMPLE"></span><span id="event_console_update_simple"></span>
<strong>EVENT_CONSOLE_UPDATE_SIMPLE</strong>
0x4003</td>
<td><p>A single character has changed. The <em>idObject</em> parameter is a <a href="coord-str.md" data-raw-source="[&lt;strong&gt;COORD&lt;/strong&gt;](coord-str.md)"><strong>COORD</strong></a> structure that specifies the character that has changed. The <em>idChild</em> parameter specifies the character in the low word and the <a href="console-screen-buffers.md#_win32_font_attributes" data-raw-source="[character attributes](console-screen-buffers.md#_win32_font_attributes)">character attributes</a> in the high word.</p></td>
</tr>
<tr class="even">
</tr>
<tr class="odd">
</tr>
<tr class="even">
</tr>
<tr class="odd">
</tr>
<tr class="even">
</tr>
</tbody>
</table>

Requirements
------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Minimum supported client</p></td>
<td><p>Windows 2000 Professional [desktop apps only]</p></td>
</tr>
<tr class="even">
<td><p>Minimum supported server</p></td>
<td><p>Windows 2000 Server [desktop apps only]</p></td>
</tr>
<tr class="odd">
<td><p>Header</p></td>
<td>Winuser.h</td>
</tr>
</tbody>
</table>

 

 




