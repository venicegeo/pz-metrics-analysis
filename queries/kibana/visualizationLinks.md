
### accessJob_AttemptSuccess_ByTime
```
{$KIBANA_HOST}/app/kibana#/visualize/create?embed=true&type=histogram&indexPattern=pzlogger5&_g=(refreshInterval:(display:Off,pause:!f,value:0),time:(from:now-7d,to:now))&_a=(filters:!(),linked:!f,query:(query_string:(analyze_wildcard:!t,query:'*')),uiState:(spy:(mode:(fill:!f,name:!n)),vis:(colors:('AccessJob%20Attempts':%23F2C96D,'AccessJob%20Success':%23629E51,'auditData.action%3D!'accessData!'%20%26%26%20!'Geoserver%20Deployment%20success!'':%23508642,'auditData.action%3D!'relayedJobCreation!'%20%26%26%20!'AccessJob!'':%23F2C96D))),vis:(aggs:!((id:'1',params:(),schema:metric,type:count),(id:'2',params:(customInterval:'2h',extended_bounds:(),field:timeStamp,interval:h,min_doc_count:1),schema:segment,type:date_histogram),(id:'3',params:(filters:!((input:(query:(query_string:(analyze_wildcard:!t,query:'auditData.action%3D!'relayedJobCreation!'%20%26%26%20!'AccessJob!''))),label:'AccessJob%20Attempts'),(input:(query:(query_string:(analyze_wildcard:!t,query:'auditData.action%3D!'accessData!'%20%26%26%20!'Geoserver%20Deployment%20success!''))),label:'AccessJob%20Success'))),schema:group,type:filters)),listeners:(),params:(addLegend:!t,addTimeMarker:!f,addTooltip:!t,defaultYExtents:!f,mode:grouped,scale:linear,setYExtents:!f,shareYAxis:!t,spyPerPage:10,times:!(),yAxis:()),title:'ACCESS%20per%20hour%20attempt%2Fsuccess',type:histogram))
```


### executeServiceJob_AttemptSuccess_ByTime
```
{$KIBANA_HOST}/app/kibana#/visualize/create?embed=true&type=histogram&indexPattern=pzlogger5&_g=(refreshInterval:(display:Off,pause:!f,value:0),time:(from:now-7d,to:now))&_a=(filters:!(),linked:!f,query:(query_string:(analyze_wildcard:!t,query:'*')),uiState:(spy:(mode:(fill:!f,name:!n)),vis:(colors:('ExecuteServiceJob%20Attempts':%236ED0E0,'ExecuteServiceJob%20Success':%23EF843C))),vis:(aggs:!((id:'1',params:(),schema:metric,type:count),(id:'2',params:(customInterval:'2h',extended_bounds:(),field:timeStamp,interval:h,min_doc_count:1),schema:segment,type:date_histogram),(id:'3',params:(filters:!((input:(query:(query_string:(analyze_wildcard:!t,query:'auditData.action%3D!'executeService!''))),label:'ExecuteServiceJob%20Attempts'),(input:(query:(query_string:(analyze_wildcard:!t,query:'auditData.action%3D!'executeServiceWorkflowEventCreated!''))),label:'ExecuteServiceJob%20Success'))),schema:group,type:filters)),listeners:(),params:(addLegend:!t,addTimeMarker:!f,addTooltip:!t,defaultYExtents:!f,mode:grouped,scale:linear,setYExtents:!f,shareYAxis:!t,spyPerPage:10,times:!(),yAxis:()),title:'EXECUTESERVICE%20per%20hour%20attempts%20success',type:histogram))
```


### ingestJob_AttemptSuccess_ByTime
```
{$KIBANA_HOST}/app/kibana#/visualize/create?embed=true&type=histogram&indexPattern=pzlogger5&_g=(refreshInterval:(display:Off,pause:!f,value:0),time:(from:now-7d,to:now))&_a=(filters:!(),linked:!f,query:(query_string:(analyze_wildcard:!t,query:'*')),uiState:(spy:(mode:(fill:!f,name:request)),vis:(colors:('AccessJob%20Attempts':%23F2C96D,'AccessJob%20Success':%23629E51,'auditData.action%3D!'accessData!'%20%26%26%20!'Geoserver%20Deployment%20successul!'':%23508642,'auditData.action%3D!'relayedJobCreation!'%20%26%26%20!'AccessJob!'':%23F2C96D))),vis:(aggs:!((id:'1',params:(),schema:metric,type:count),(id:'2',params:(customInterval:'2h',extended_bounds:(),field:timeStamp,interval:h,min_doc_count:1),schema:segment,type:date_histogram),(id:'3',params:(filters:!((input:(query:(query_string:(analyze_wildcard:!t,query:'auditData.action%3D!'relayedJobCreation!'%20%26%26%20IngestJob'))),label:'IngestJob%20Attempts'),(input:(query:(query_string:(analyze_wildcard:!t,query:'auditData.action%3D!'loadedData!'%20%26%26%20!'Successful%20Load%20of%20Data'))),label:'IngestJob%20Success'))),schema:group,type:filters)),listeners:(),params:(addLegend:!t,addTimeMarker:!f,addTooltip:!t,defaultYExtents:!f,mode:grouped,scale:linear,setYExtents:!f,shareYAxis:!t,spyPerPage:10,times:!(),yAxis:()),title:'INGEST%20per%20hour%20attempt%2Fsuccess',type:histogram))
```


### jobs_Attempt_ByTypeAndUser
```
{$KIBANA_HOST}/app/kibana#/visualize/create?embed=true&type=histogram&indexPattern=pzlogger5&_g=(refreshInterval:(display:Off,pause:!f,value:0),time:(from:now-7d,mode:quick,to:now))&_a=(filters:!(('$state':(store:appState),meta:(alias:!n,disabled:!f,index:pzlogger5,key:auditData.action,negate:!f,value:relayedJobCreation),query:(match:(auditData.action:(query:relayedJobCreation,type:phrase)))),('$state':(store:appState),meta:(alias:!n,disabled:!f,index:pzlogger5,key:auditData.actor,negate:!f,value:npetest008.gxaws.dev),query:(match:(auditData.actor:(query:npetest008.gxaws.dev,type:phrase))))),linked:!f,query:(query_string:(analyze_wildcard:!t,query:'*')),uiState:(spy:(mode:(fill:!f,name:!n))),vis:(aggs:!((id:'1',params:(),schema:metric,type:count),(id:'2',params:(filters:!((input:(query:(query_string:(analyze_wildcard:!t,query:AccessJob))),label:''),(input:(query:(query_string:(analyze_wildcard:!t,query:ExecuteServiceJob)))),(input:(query:(query_string:(analyze_wildcard:!t,query:IngestJob)))))),schema:segment,type:filters)),listeners:(),params:(addLegend:!t,addTimeMarker:!f,addTooltip:!t,defaultYExtents:!f,mode:stacked,scale:linear,setYExtents:!f,shareYAxis:!t,spyPerPage:10,times:!(),yAxis:()),title:'New%20Visualization',type:histogram))
```


### total_Jobs_OverTime
```
{$KIBANA_HOST}/app/kibana#/visualize/create?embed=true&type=metric&indexPattern=pzlogger5&_g=(refreshInterval:(display:Off,pause:!f,value:0),time:(from:now-7d,to:now))&_a=(filters:!(),linked:!f,query:(query_string:(analyze_wildcard:!t,query:auditData.action%3D%22relayedJobCreation%22)),uiState:(),vis:(aggs:!((id:'1',params:(),schema:metric,type:count)),listeners:(),params:(fontSize:84),title:totaljobspertime,type:metric))
```


### userLoggedIn_ByTime
```
{$KIBANA_HOST}/app/kibana#/visualize/create?embed=true&type=line&indexPattern=pzlogger5&_g=(refreshInterval:(display:Off,pause:!f,value:0),time:(from:now-7d,to:now))&_a=(filters:!(),linked:!f,query:(query_string:(analyze_wildcard:!t,query:'*')),uiState:(spy:(mode:(fill:!f,name:request)),vis:(colors:('auditData.action%3D!'userLoggedIn!'':%237EB26D))),vis:(aggs:!((id:'1',params:(),schema:metric,type:count),(id:'2',params:(customInterval:'2h',extended_bounds:(),field:timeStamp,interval:h,min_doc_count:1),schema:segment,type:date_histogram),(id:'3',params:(filters:!((input:(query:(query_string:(analyze_wildcard:!t,query:'auditData.action%3D!'userLoggedIn!''))),label:'User%20Logged%20In'))),schema:group,type:filters)),listeners:(),params:(addLegend:!t,addTimeMarker:!f,addTooltip:!t,defaultYExtents:!f,drawLinesBetweenPoints:!t,interpolate:linear,radiusRatio:9,scale:linear,setYExtents:!f,shareYAxis:!t,showCircles:!t,smoothLines:!f,times:!(),yAxis:()),title:USERLOGGEDIN,type:line))
```


### workflow_ObjectCreation_ByTime
```
{$KIBANA_HOST}/app/kibana#/visualize/create?embed=true&type=line&indexPattern=pzlogger5&_g=(refreshInterval:(display:Off,pause:!f,value:0),time:(from:now-7d,to:now))&_a=(filters:!(),linked:!f,query:(query_string:(analyze_wildcard:!t,query:'*')),uiState:(vis:(colors:(Alert:%23BF1B00,Event:%237EB26D,EventType:%23584477,Trigger:%2365C5DB))),vis:(aggs:!((id:'1',params:(),schema:metric,type:count),(id:'2',params:(customInterval:'2h',extended_bounds:(),field:timeStamp,interval:h,min_doc_count:1),schema:segment,type:date_histogram),(id:'3',params:(filters:!((input:(query:(query_string:(analyze_wildcard:!t,query:'auditData.action%3D!'createdAlert!'%20%26%26%20!'successfully%20created%20alert!''))),label:Alert),(input:(query:(query_string:(analyze_wildcard:!t,query:'auditData.action%3D!'createdTrigger!'%20%26%26%20!'successfully%20created%20trigger!''))),label:Trigger),(input:(query:(query_string:(analyze_wildcard:!t,query:'auditData.action%3D!'createdEvent!'%20%26%26%20!'successfully%20created%20event!''))),label:Event),(input:(query:(query_string:(analyze_wildcard:!t,query:'auditData.action%3D!'createdEventType%20%26%26%20!'successfully%20created%20eventType!''))),label:EventType))),schema:group,type:filters)),listeners:(),params:(addLegend:!t,addTimeMarker:!f,addTooltip:!t,defaultYExtents:!f,drawLinesBetweenPoints:!t,interpolate:linear,radiusRatio:9,scale:linear,setYExtents:!f,shareYAxis:!t,showCircles:!t,smoothLines:!f,times:!(),yAxis:()),title:workflowObjectCreation,type:line))
```

