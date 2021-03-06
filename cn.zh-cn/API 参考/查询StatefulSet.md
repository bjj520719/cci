# 查询StatefulSet<a name="cci_02_3031"></a>

## 功能介绍<a name="section15132207"></a>

查询StatefulSet的详细信息。

## URI<a name="section1972143"></a>

GET /apis/apps/v1/namespaces/\{namespace\}/statefulsets/\{name\}

**表 1**  Path参数

<a name="table1696332124519"></a>
<table><thead align="left"><tr id="row11961332194516"><th class="cellrowborder" valign="top" width="24%" id="mcps1.2.3.1.1"><p id="p396032144518"><a name="p396032144518"></a><a name="p396032144518"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="76%" id="mcps1.2.3.1.2"><p id="p18962325454"><a name="p18962325454"></a><a name="p18962325454"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row9960327457"><td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.3.1.1 "><p id="p1496113214456"><a name="p1496113214456"></a><a name="p1496113214456"></a>namespace</p>
</td>
<td class="cellrowborder" valign="top" width="76%" headers="mcps1.2.3.1.2 "><p id="p141902036155717"><a name="p141902036155717"></a><a name="p141902036155717"></a>Object name and auth scope, such as for teams and projects.</p>
</td>
</tr>
<tr id="row13794857171116"><td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.3.1.1 "><p id="p5984165818113"><a name="p5984165818113"></a><a name="p5984165818113"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="76%" headers="mcps1.2.3.1.2 "><p id="p4984175851116"><a name="p4984175851116"></a><a name="p4984175851116"></a>Name of the StatefulSet.</p>
</td>
</tr>
</tbody>
</table>

**表 2**  Query参数

<a name="d0e38675"></a>
<table><thead align="left"><tr id="row60367007"><th class="cellrowborder" valign="top" width="20.407959204079592%" id="mcps1.2.4.1.1"><p id="p65652297517"><a name="p65652297517"></a><a name="p65652297517"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16.328367163283673%" id="mcps1.2.4.1.2"><p id="p165661629135114"><a name="p165661629135114"></a><a name="p165661629135114"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="63.26367363263674%" id="mcps1.2.4.1.3"><p id="p14567629115114"><a name="p14567629115114"></a><a name="p14567629115114"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row24030130"><td class="cellrowborder" valign="top" width="20.407959204079592%" headers="mcps1.2.4.1.1 "><p id="p283486"><a name="p283486"></a><a name="p283486"></a>pretty</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.4.1.2 "><p id="p22962431"><a name="p22962431"></a><a name="p22962431"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="63.26367363263674%" headers="mcps1.2.4.1.3 "><p id="p48017661"><a name="p48017661"></a><a name="p48017661"></a>If 'true', then the output is pretty printed.</p>
</td>
</tr>
<tr id="row29505770"><td class="cellrowborder" valign="top" width="20.407959204079592%" headers="mcps1.2.4.1.1 "><p id="p41157182"><a name="p41157182"></a><a name="p41157182"></a>exact</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.4.1.2 "><p id="p45397409"><a name="p45397409"></a><a name="p45397409"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="63.26367363263674%" headers="mcps1.2.4.1.3 "><p id="p53311550"><a name="p53311550"></a><a name="p53311550"></a>Should the export be exact. Exact export maintains cluster-specific fields like 'Namespace'.</p>
</td>
</tr>
<tr id="row10041905"><td class="cellrowborder" valign="top" width="20.407959204079592%" headers="mcps1.2.4.1.1 "><p id="p8087957"><a name="p8087957"></a><a name="p8087957"></a>export</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.4.1.2 "><p id="p51144774"><a name="p51144774"></a><a name="p51144774"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="63.26367363263674%" headers="mcps1.2.4.1.3 "><p id="p49085995"><a name="p49085995"></a><a name="p49085995"></a>Should this value be exported. Export strips fields that a user cannot specify.</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section17749294"></a>

N/A

## 响应消息<a name="section25525926"></a>

**响应参数：**

响应参数的详细描述请参见[表86](数据结构.md#d0e37568)。

**响应示例：**

```
{
    "kind": "StatefulSet",
    "apiVersion": "apps/v1",
    "metadata": {
        "name": "statefulset-test",
        "namespace": "namespace-test",
        "selfLink": "/apis/apps/v1/namespaces/namespace-test/statefulsets/statefulset-test",
        "uid": "f4a35f35-b011-11e8-b6ef-f898ef6c78b4",
        "resourceVersion": "5209881",
        "generation": 1,
        "creationTimestamp": "2018-09-04T07:13:00Z",
        "labels": {
            "app": "statefulset-test"
        },
        "enable": true
    },
    "spec": {
        "replicas": 3,
        "selector": {
            "matchLabels": {
                "app": "statefulset-test"
            }
        },
        "template": {
            "metadata": {
                "creationTimestamp": null,
                "labels": {
                    "app": "statefulset-test"
                },
                "annotations": {
                    "cri.cci.io/container-type": "secure-container"
                },
                "enable": true
            },
            "spec": {
                "containers": [
                    {
                        "name": "container-0",
                        "image": "redis",
                        "resources": {
                            "limits": {
                                "cpu": "500m",
                                "memory": "1Gi"
                            },
                            "requests": {
                                "cpu": "500m",
                                "memory": "1Gi"
                            }
                        },
                        "terminationMessagePath": "/dev/termination-log",
                        "terminationMessagePolicy": "File",
                        "imagePullPolicy": "IfNotPresent"
                    }
                ],
                "restartPolicy": "Always",
                "terminationGracePeriodSeconds": 30,
                "dnsPolicy": "ClusterFirst",
                "securityContext": {},
                "imagePullSecrets": [
                    {
                        "name": "imagepull-secret"
                    }
                ],
                "schedulerName": "default-scheduler"
            }
        },
        "serviceName": "",
        "podManagementPolicy": "OrderedReady",
        "updateStrategy": {
            "type": "OnDelete"
        },
        "revisionHistoryLimit": 10
    },
    "status": {
        "observedGeneration": 1,
        "replicas": 3,
        "readyReplicas": 2,
        "currentReplicas": 3,
        "currentRevision": "statefulset-test-f986b645b",
        "updateRevision": "statefulset-test-f986b645b",
        "collisionCount": 0
    }
}
```

## 状态码<a name="section28406742"></a>

[表3](#d0e38773)描述API的状态码。

**表 3**  状态码

<a name="d0e38773"></a>
<table><thead align="left"><tr id="row48797355"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p60271674"><a name="p60271674"></a><a name="p60271674"></a>Status Code</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p50167450"><a name="p50167450"></a><a name="p50167450"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row37031667"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p46775020"><a name="p46775020"></a><a name="p46775020"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p30680237"><a name="p30680237"></a><a name="p30680237"></a>This operation succeeds, and a StatefulSet resource object is returned.</p>
</td>
</tr>
</tbody>
</table>

