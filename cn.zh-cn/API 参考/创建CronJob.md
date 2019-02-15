# 创建CronJob<a name="cci_02_3104"></a>

## 功能介绍<a name="section5825523"></a>

This API is used to create a CronJob resource object.

## URI<a name="section52429714"></a>

POST /apis/batch/v1beta1/namespaces/\{namespace\}/cronjobs

**表 1**  参数解释

<a name="table65625523"></a>
<table><thead align="left"><tr id="row19842874"><th class="cellrowborder" valign="top" width="22.220000000000002%" id="mcps1.2.4.1.1"><p id="p65652297517"><a name="p65652297517"></a><a name="p65652297517"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="17.169999999999998%" id="mcps1.2.4.1.2"><p id="p165661629135114"><a name="p165661629135114"></a><a name="p165661629135114"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="60.61%" id="mcps1.2.4.1.3"><p id="p14567629115114"><a name="p14567629115114"></a><a name="p14567629115114"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row54819108"><td class="cellrowborder" valign="top" width="22.220000000000002%" headers="mcps1.2.4.1.1 "><p id="p11162788"><a name="p11162788"></a><a name="p11162788"></a>namespace</p>
</td>
<td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.4.1.2 "><p id="p31770653"><a name="p31770653"></a><a name="p31770653"></a>Yes</p>
</td>
<td class="cellrowborder" valign="top" width="60.61%" headers="mcps1.2.4.1.3 "><p id="p23286070"><a name="p23286070"></a><a name="p23286070"></a>Object name and auth scope, such as for teams and projects.</p>
</td>
</tr>
<tr id="row8248038"><td class="cellrowborder" valign="top" width="22.220000000000002%" headers="mcps1.2.4.1.1 "><p id="p64111314"><a name="p64111314"></a><a name="p64111314"></a>pretty</p>
</td>
<td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.4.1.2 "><p id="p25633971"><a name="p25633971"></a><a name="p25633971"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="60.61%" headers="mcps1.2.4.1.3 "><p id="p63085809"><a name="p63085809"></a><a name="p63085809"></a>If 'true', then the output is pretty printed.</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section2105383"></a>

**请求参数：**

**表 2**  请求参数

<a name="table8040885"></a>
<table><thead align="left"><tr id="row23603642"><th class="cellrowborder" valign="top" width="22.447755224477554%" id="mcps1.2.5.1.1"><p id="p32846815"><a name="p32846815"></a><a name="p32846815"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="14.288571142885711%" id="mcps1.2.5.1.2"><p id="p43346336"><a name="p43346336"></a><a name="p43346336"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20.407959204079592%" id="mcps1.2.5.1.3"><p id="p21392359"><a name="p21392359"></a><a name="p21392359"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="p55059481"><a name="p55059481"></a><a name="p55059481"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row30632992"><td class="cellrowborder" valign="top" width="22.447755224477554%" headers="mcps1.2.5.1.1 "><p id="p65353316"><a name="p65353316"></a><a name="p65353316"></a>apiVersion</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.5.1.2 "><p id="p59127244"><a name="p59127244"></a><a name="p59127244"></a>Yes</p>
</td>
<td class="cellrowborder" valign="top" width="20.407959204079592%" headers="mcps1.2.5.1.3 "><p id="p24577473"><a name="p24577473"></a><a name="p24577473"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p44618282"><a name="p44618282"></a><a name="p44618282"></a><span>APIVersion defines the versioned schema of this representation of an object. Servers should convert recognized schemas to the latest internal value, and may reject unrecognized values.</span></p>
</td>
</tr>
<tr id="row66020222"><td class="cellrowborder" valign="top" width="22.447755224477554%" headers="mcps1.2.5.1.1 "><p id="p46037745"><a name="p46037745"></a><a name="p46037745"></a>kind</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.5.1.2 "><p id="p38069836"><a name="p38069836"></a><a name="p38069836"></a>Yes</p>
</td>
<td class="cellrowborder" valign="top" width="20.407959204079592%" headers="mcps1.2.5.1.3 "><p id="p63757880"><a name="p63757880"></a><a name="p63757880"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p64114652"><a name="p64114652"></a><a name="p64114652"></a>Kind is a string value representing the REST resource this object represents. Servers may infer this from the endpoint the client submits requests to. Cannot be updated. In CamelCase.</p>
</td>
</tr>
<tr id="row40160963"><td class="cellrowborder" valign="top" width="22.447755224477554%" headers="mcps1.2.5.1.1 "><p id="p31812591"><a name="p31812591"></a><a name="p31812591"></a>metadata</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.5.1.2 "><p id="p26683112"><a name="p26683112"></a><a name="p26683112"></a>Yes</p>
</td>
<td class="cellrowborder" valign="top" width="20.407959204079592%" headers="mcps1.2.5.1.3 "><p id="p13848469"><a name="p13848469"></a><a name="p13848469"></a><a href="公共参数.md#zh-cn_topic_0079614925_table47756489">表10</a></p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p29204826"><a name="p29204826"></a><a name="p29204826"></a>Standard list metadata.</p>
</td>
</tr>
<tr id="row61516845"><td class="cellrowborder" valign="top" width="22.447755224477554%" headers="mcps1.2.5.1.1 "><p id="p16808552"><a name="p16808552"></a><a name="p16808552"></a>spec</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.5.1.2 "><p id="p19315447"><a name="p19315447"></a><a name="p19315447"></a>Yes</p>
</td>
<td class="cellrowborder" valign="top" width="20.407959204079592%" headers="mcps1.2.5.1.3 "><p id="p21047363"><a name="p21047363"></a><a name="p21047363"></a><a href="#table51402650">表3</a></p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p42706636"><a name="p42706636"></a><a name="p42706636"></a>Specification of the desired behavior of a cron job, including the schedule.</p>
</td>
</tr>
<tr id="row48815407"><td class="cellrowborder" valign="top" width="22.447755224477554%" headers="mcps1.2.5.1.1 "><p id="p61733920"><a name="p61733920"></a><a name="p61733920"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.5.1.2 "><p id="p34391662"><a name="p34391662"></a><a name="p34391662"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="20.407959204079592%" headers="mcps1.2.5.1.3 "><p id="p34261248"><a name="p34261248"></a><a name="p34261248"></a><a href="#table28665255">表4</a></p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p11952954"><a name="p11952954"></a><a name="p11952954"></a><span>Current status of a cron job.</span></p>
</td>
</tr>
</tbody>
</table>

**表 3**  CronJobSpec字段数据结构说明

<a name="table51402650"></a>
<table><thead align="left"><tr id="row2975313"><th class="cellrowborder" valign="top" width="23%" id="mcps1.2.5.1.1"><p id="p39673810"><a name="p39673810"></a><a name="p39673810"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.2"><p id="p59462043"><a name="p59462043"></a><a name="p59462043"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.3"><p id="p51696213"><a name="p51696213"></a><a name="p51696213"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42%" id="mcps1.2.5.1.4"><p id="p26643752"><a name="p26643752"></a><a name="p26643752"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row10660283"><td class="cellrowborder" valign="top" width="23%" headers="mcps1.2.5.1.1 "><p id="p58176566"><a name="p58176566"></a><a name="p58176566"></a>concurrencyPolicy</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p270813244402"><a name="p270813244402"></a><a name="p270813244402"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.3 "><p id="p48343558"><a name="p48343558"></a><a name="p48343558"></a><span>String</span></p>
</td>
<td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.5.1.4 "><p id="p8335102813362"><a name="p8335102813362"></a><a name="p8335102813362"></a><span>Specifies how to treat concurrent executions of a Job. Valid values are: - "Allow" (default): allows CronJobs to run concurrently; - "Forbid": forbids concurrent runs, skipping next run if previous run hasn’t finished yet; - "Replace": cancels currently running job and replaces it with a new one</span>.</p>
</td>
</tr>
<tr id="row10300809"><td class="cellrowborder" valign="top" width="23%" headers="mcps1.2.5.1.1 "><p id="p197193233615"><a name="p197193233615"></a><a name="p197193233615"></a>failedJobsHistoryLimit</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p270652414011"><a name="p270652414011"></a><a name="p270652414011"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.3 "><p id="p1355353"><a name="p1355353"></a><a name="p1355353"></a>Integer(int32)</p>
</td>
<td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.5.1.4 "><p id="p0334192817366"><a name="p0334192817366"></a><a name="p0334192817366"></a>The number of failed finished jobs to retain. This is a pointer to distinguish between explicit zero and not specified. Defaults to 1.</p>
</td>
</tr>
<tr id="row34103458"><td class="cellrowborder" valign="top" width="23%" headers="mcps1.2.5.1.1 "><p id="p16961232143615"><a name="p16961232143615"></a><a name="p16961232143615"></a>jobTemplate</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p14704102404010"><a name="p14704102404010"></a><a name="p14704102404010"></a>Yes</p>
</td>
<td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.3 "><p id="p19240909"><a name="p19240909"></a><a name="p19240909"></a><a href="#table928061144217">表6</a></p>
</td>
<td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.5.1.4 "><p id="p933322823614"><a name="p933322823614"></a><a name="p933322823614"></a><span>Specifies the job that will be created when executing a CronJob.</span></p>
</td>
</tr>
<tr id="row7831802"><td class="cellrowborder" valign="top" width="23%" headers="mcps1.2.5.1.1 "><p id="p1694193283616"><a name="p1694193283616"></a><a name="p1694193283616"></a>schedule</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p4703142494015"><a name="p4703142494015"></a><a name="p4703142494015"></a>Yes</p>
</td>
<td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.3 "><p id="p49457273"><a name="p49457273"></a><a name="p49457273"></a><span>String</span></p>
</td>
<td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.5.1.4 "><p id="p8331928143612"><a name="p8331928143612"></a><a name="p8331928143612"></a>The schedule in Cron format.</p>
</td>
</tr>
<tr id="row17813596"><td class="cellrowborder" valign="top" width="23%" headers="mcps1.2.5.1.1 "><p id="p193143210361"><a name="p193143210361"></a><a name="p193143210361"></a>startingDeadlineSeconds</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p77021224134014"><a name="p77021224134014"></a><a name="p77021224134014"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.3 "><p id="p1758932144016"><a name="p1758932144016"></a><a name="p1758932144016"></a>Integer(int64)</p>
</td>
<td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.5.1.4 "><p id="p1330102803616"><a name="p1330102803616"></a><a name="p1330102803616"></a><span>Optional deadline in seconds for starting the job if it misses scheduled time for any reason. Missed jobs executions will be counted as failed ones.</span></p>
</td>
</tr>
<tr id="row24881422"><td class="cellrowborder" valign="top" width="23%" headers="mcps1.2.5.1.1 "><p id="p79383211361"><a name="p79383211361"></a><a name="p79383211361"></a>successfulJobsHistoryLimit</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p19699162454018"><a name="p19699162454018"></a><a name="p19699162454018"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.3 "><p id="p19571328409"><a name="p19571328409"></a><a name="p19571328409"></a>Integer(int32)</p>
</td>
<td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.5.1.4 "><p id="p63296288365"><a name="p63296288365"></a><a name="p63296288365"></a>The number of successful finished jobs to retain. This is a pointer to distinguish between explicit zero and not specified. Defaults to 3.</p>
</td>
</tr>
<tr id="row47082918374"><td class="cellrowborder" valign="top" width="23%" headers="mcps1.2.5.1.1 "><p id="p670929193712"><a name="p670929193712"></a><a name="p670929193712"></a>suspend</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p15709590371"><a name="p15709590371"></a><a name="p15709590371"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.3 "><p id="p1770917913713"><a name="p1770917913713"></a><a name="p1770917913713"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.5.1.4 "><p id="p187091194376"><a name="p187091194376"></a><a name="p187091194376"></a><span>This flag tells the controller to suspend subsequent executions, it does not apply to already started executions. Defaults to false.</span></p>
</td>
</tr>
</tbody>
</table>

**表 4**  status字段数据结构说明

<a name="table28665255"></a>
<table><thead align="left"><tr id="row8005580"><th class="cellrowborder" valign="top" width="22.68%" id="mcps1.2.5.1.1"><p id="p44472221"><a name="p44472221"></a><a name="p44472221"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="14.430000000000001%" id="mcps1.2.5.1.2"><p id="p45480180"><a name="p45480180"></a><a name="p45480180"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="19.59%" id="mcps1.2.5.1.3"><p id="p60015926"><a name="p60015926"></a><a name="p60015926"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="43.3%" id="mcps1.2.5.1.4"><p id="p29451853"><a name="p29451853"></a><a name="p29451853"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row36789921"><td class="cellrowborder" valign="top" width="22.68%" headers="mcps1.2.5.1.1 "><p id="p27193625"><a name="p27193625"></a><a name="p27193625"></a>active</p>
</td>
<td class="cellrowborder" valign="top" width="14.430000000000001%" headers="mcps1.2.5.1.2 "><p id="p15879111544318"><a name="p15879111544318"></a><a name="p15879111544318"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.2.5.1.3 "><p id="p2878161564312"><a name="p2878161564312"></a><a name="p2878161564312"></a><a href="#table292410545345">表5</a></p>
</td>
<td class="cellrowborder" valign="top" width="43.3%" headers="mcps1.2.5.1.4 "><p id="p28761915184314"><a name="p28761915184314"></a><a name="p28761915184314"></a><span>A list of pointers to currently running jobs.</span></p>
</td>
</tr>
<tr id="row29065558"><td class="cellrowborder" valign="top" width="22.68%" headers="mcps1.2.5.1.1 "><p id="p5499969"><a name="p5499969"></a><a name="p5499969"></a>lastScheduleTime</p>
</td>
<td class="cellrowborder" valign="top" width="14.430000000000001%" headers="mcps1.2.5.1.2 "><p id="p181051554144319"><a name="p181051554144319"></a><a name="p181051554144319"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.2.5.1.3 "><p id="p47840241"><a name="p47840241"></a><a name="p47840241"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.3%" headers="mcps1.2.5.1.4 "><p id="p49854342"><a name="p49854342"></a><a name="p49854342"></a>Information when was the last time the job was successfully scheduled.</p>
</td>
</tr>
</tbody>
</table>

**表 5**  ObjectReference\_v1\_core

<a name="table292410545345"></a>
<table><thead align="left"><tr id="row393905412349"><th class="cellrowborder" valign="top" width="22.68%" id="mcps1.2.5.1.1"><p id="p1194317544343"><a name="p1194317544343"></a><a name="p1194317544343"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="14.430000000000001%" id="mcps1.2.5.1.2"><p id="p6945145418346"><a name="p6945145418346"></a><a name="p6945145418346"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="19.59%" id="mcps1.2.5.1.3"><p id="p119482548345"><a name="p119482548345"></a><a name="p119482548345"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="43.3%" id="mcps1.2.5.1.4"><p id="p5951854103415"><a name="p5951854103415"></a><a name="p5951854103415"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row139531254163415"><td class="cellrowborder" valign="top" width="22.68%" headers="mcps1.2.5.1.1 "><p id="p9309104362"><a name="p9309104362"></a><a name="p9309104362"></a>apiVersion</p>
</td>
<td class="cellrowborder" valign="top" width="14.430000000000001%" headers="mcps1.2.5.1.2 "><p id="p8351135933611"><a name="p8351135933611"></a><a name="p8351135933611"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.2.5.1.3 "><p id="p13971166133711"><a name="p13971166133711"></a><a name="p13971166133711"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="43.3%" headers="mcps1.2.5.1.4 "><p id="p148611520163713"><a name="p148611520163713"></a><a name="p148611520163713"></a>API version of the referent.</p>
</td>
</tr>
<tr id="row1967105412340"><td class="cellrowborder" valign="top" width="22.68%" headers="mcps1.2.5.1.1 "><p id="p73041603367"><a name="p73041603367"></a><a name="p73041603367"></a>fieldPath</p>
</td>
<td class="cellrowborder" valign="top" width="14.430000000000001%" headers="mcps1.2.5.1.2 "><p id="p3357205973618"><a name="p3357205973618"></a><a name="p3357205973618"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.2.5.1.3 "><p id="p1397918610378"><a name="p1397918610378"></a><a name="p1397918610378"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="43.3%" headers="mcps1.2.5.1.4 "><p id="p829713282379"><a name="p829713282379"></a><a name="p829713282379"></a>If referring to a piece of an object instead of an entire object, this string should contain a valid JSON/Go field access statement, such as desiredState.manifest.containers[2]. For example, if the object reference is to a container within a pod, this would take on a value like: "spec.containers{name}" (where "name" refers to the name of the container that triggered the event) or if no container name is specified "spec.containers[2]" (container with index 2 in this pod). This syntax is chosen only to have some well-defined way of referencing a part of an object.</p>
</td>
</tr>
<tr id="row1335012117364"><td class="cellrowborder" valign="top" width="22.68%" headers="mcps1.2.5.1.1 "><p id="p73511321153615"><a name="p73511321153615"></a><a name="p73511321153615"></a>kind</p>
</td>
<td class="cellrowborder" valign="top" width="14.430000000000001%" headers="mcps1.2.5.1.2 "><p id="p7364195943619"><a name="p7364195943619"></a><a name="p7364195943619"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.2.5.1.3 "><p id="p79861669378"><a name="p79861669378"></a><a name="p79861669378"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="43.3%" headers="mcps1.2.5.1.4 "><p id="p176891427372"><a name="p176891427372"></a><a name="p176891427372"></a>Kind of the referent. More info: https://git.k8s.io/community/contributors/devel/api-conventions.md#types-kinds</p>
</td>
</tr>
<tr id="row586802119360"><td class="cellrowborder" valign="top" width="22.68%" headers="mcps1.2.5.1.1 "><p id="p386892183612"><a name="p386892183612"></a><a name="p386892183612"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="14.430000000000001%" headers="mcps1.2.5.1.2 "><p id="p4373145973611"><a name="p4373145973611"></a><a name="p4373145973611"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.2.5.1.3 "><p id="p1399819623718"><a name="p1399819623718"></a><a name="p1399819623718"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="43.3%" headers="mcps1.2.5.1.4 "><p id="p12343750133712"><a name="p12343750133712"></a><a name="p12343750133712"></a>Name of the referent. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names</p>
</td>
</tr>
<tr id="row133561622193618"><td class="cellrowborder" valign="top" width="22.68%" headers="mcps1.2.5.1.1 "><p id="p3356112215367"><a name="p3356112215367"></a><a name="p3356112215367"></a>namespace</p>
</td>
<td class="cellrowborder" valign="top" width="14.430000000000001%" headers="mcps1.2.5.1.2 "><p id="p123795597367"><a name="p123795597367"></a><a name="p123795597367"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.2.5.1.3 "><p id="p1681274371"><a name="p1681274371"></a><a name="p1681274371"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="43.3%" headers="mcps1.2.5.1.4 "><p id="p12142256143711"><a name="p12142256143711"></a><a name="p12142256143711"></a>Namespace of the referent. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/namespaces/</p>
</td>
</tr>
<tr id="row15874192293617"><td class="cellrowborder" valign="top" width="22.68%" headers="mcps1.2.5.1.1 "><p id="p2087462253615"><a name="p2087462253615"></a><a name="p2087462253615"></a>resourceVersion</p>
</td>
<td class="cellrowborder" valign="top" width="14.430000000000001%" headers="mcps1.2.5.1.2 "><p id="p5384115973613"><a name="p5384115973613"></a><a name="p5384115973613"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.2.5.1.3 "><p id="p715157153711"><a name="p715157153711"></a><a name="p715157153711"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="43.3%" headers="mcps1.2.5.1.4 "><p id="p155505513815"><a name="p155505513815"></a><a name="p155505513815"></a>Specific resourceVersion to which this reference is made, if any. More info: https://git.k8s.io/community/contributors/devel/api-conventions.md#concurrency-control-and-consistency</p>
</td>
</tr>
<tr id="row4731450143610"><td class="cellrowborder" valign="top" width="22.68%" headers="mcps1.2.5.1.1 "><p id="p11731650193611"><a name="p11731650193611"></a><a name="p11731650193611"></a>uid</p>
</td>
<td class="cellrowborder" valign="top" width="14.430000000000001%" headers="mcps1.2.5.1.2 "><p id="p5390459133619"><a name="p5390459133619"></a><a name="p5390459133619"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.2.5.1.3 "><p id="p92313717371"><a name="p92313717371"></a><a name="p92313717371"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="43.3%" headers="mcps1.2.5.1.4 "><p id="p11731504366"><a name="p11731504366"></a><a name="p11731504366"></a>UID of the referent. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#uids</p>
</td>
</tr>
</tbody>
</table>

**表 6**  jobTemplate字段数据结构说明

<a name="table928061144217"></a>
<table><thead align="left"><tr id="row329581184215"><th class="cellrowborder" valign="top" width="22.447755224477554%" id="mcps1.2.5.1.1"><p id="p143000124216"><a name="p143000124216"></a><a name="p143000124216"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.2"><p id="p15304101134219"><a name="p15304101134219"></a><a name="p15304101134219"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="19.388061193880613%" id="mcps1.2.5.1.3"><p id="p10308181104215"><a name="p10308181104215"></a><a name="p10308181104215"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="p16311181134212"><a name="p16311181134212"></a><a name="p16311181134212"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1131319119429"><td class="cellrowborder" valign="top" width="22.447755224477554%" headers="mcps1.2.5.1.1 "><p id="p4320141164216"><a name="p4320141164216"></a><a name="p4320141164216"></a>metadata</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p672712490460"><a name="p672712490460"></a><a name="p672712490460"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="19.388061193880613%" headers="mcps1.2.5.1.3 "><p id="p164941501417"><a name="p164941501417"></a><a name="p164941501417"></a><a href="公共参数.md#zh-cn_topic_0079614925_table47756489">表10</a></p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p833416174219"><a name="p833416174219"></a><a name="p833416174219"></a><span>Standard object’s metadata of the jobs created from this template.</span></p>
</td>
</tr>
<tr id="row153356134215"><td class="cellrowborder" valign="top" width="22.447755224477554%" headers="mcps1.2.5.1.1 "><p id="p933919116429"><a name="p933919116429"></a><a name="p933919116429"></a>spec</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p572394914610"><a name="p572394914610"></a><a name="p572394914610"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="19.388061193880613%" headers="mcps1.2.5.1.3 "><p id="p203474194211"><a name="p203474194211"></a><a name="p203474194211"></a><a href="公共参数.md#table51402650">表100</a></p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p1335141134213"><a name="p1335141134213"></a><a name="p1335141134213"></a>Specification of the desired behavior of the job.</p>
</td>
</tr>
</tbody>
</table>

**请求示例：**

```
{
    "apiVersion": "batch/v1beta1",
    "kind": "CronJob",
    "metadata": {
        "name": "cronjob-test",
        "namespace": "default"
    },
    "spec": {
        "concurrencyPolicy": "Allow",
        "jobTemplate": {
            "spec": {
                "template": {
                    "metadata": {
                        "enable": true,
                        "labels": {
                            "sjname": "cronjob-test"
                        }
                    },
                    "spec": {
                        "containers": [
                            {
                                "image": "nginx:stable-perl",
                                "imagePullPolicy": "IfNotPresent",
                                "lifecycle": {},
                                "name": "container-0"
                            }
                        ],
                        "dnsPolicy": "ClusterFirst",
                        "imagePullSecrets": [
                            {
                                "name": "default-secret"
                            }
                        ],
                        "restartPolicy": "OnFailure"
                    }
                }
            }
        },
        "schedule": "*/59 * * * *"
    }
}
```

## 响应消息<a name="section18948451"></a>

**响应参数：**

响应参数的详细描述请参见[表2](#table8040885)。

**响应示例：**

```
{
    "apiVersion": "batch/v1beta1",
    "kind": "CronJob",
    "metadata": {
        "creationTimestamp": "2018-03-07T12:08:52Z",
        "enable": true,
        "name": "cronjob-test",
        "namespace": "default",
        "resourceVersion": "441019",
        "selfLink": "/apis/batch/v1beta1/namespaces/default/cronjobs/cronjob-test",
        "uid": "4d78b666-2200-11e8-96aa-fa163ecd089c"
    },
    "spec": {
        "concurrencyPolicy": "Allow",
        "failedJobsHistoryLimit": 1,
        "jobTemplate": {
            "metadata": {
                "creationTimestamp": null,
                "enable": true
            },
            "spec": {
                "template": {
                    "metadata": {
                        "creationTimestamp": null,
                        "enable": true,
                        "labels": {
                            "sjname": "cronjob-test"
                        }
                    },
                    "spec": {
                        "containers": [
                            {
                                "image": "nginx:stable-perl",
                                "imagePullPolicy": "IfNotPresent",
                                "lifecycle": {},
                                "name": "container-0",
                                "resources": {},
                                "terminationMessagePath": "/dev/termination-log",
                                "terminationMessagePolicy": "File"
                            }
                        ],
                        "dnsPolicy": "ClusterFirst",
                        "imagePullSecrets": [
                            {
                                "name": "default-secret"
                            }
                        ],
                        "restartPolicy": "OnFailure",
                        "schedulerName": "default-scheduler",
                        "securityContext": {},
                        "terminationGracePeriodSeconds": 30
                    }
                }
            }
        },
        "schedule": "*/59 * * * *",
        "successfulJobsHistoryLimit": 3,
        "suspend": false
    },
    "status": {}
}
```

## 状态码<a name="section36318335"></a>

**表 7**  状态码

<a name="table30003806"></a>
<table><thead align="left"><tr id="row20731931"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p1564889"><a name="p1564889"></a><a name="p1564889"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p59647195"><a name="p59647195"></a><a name="p59647195"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row66693514"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p33465549"><a name="p33465549"></a><a name="p33465549"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p26354957"><a name="p26354957"></a><a name="p26354957"></a>The request has been fulfilled, resulting in the creation of a new resource.</p>
</td>
</tr>
</tbody>
</table>

