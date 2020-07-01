---
title: Obter callRecord
description: Recupere as propriedades e os relacionamentos do objeto callrecord.
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 68f27a6188096d75687cd5d3e7f0234fd5c75b9d
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006885"
---
# <a name="get-callrecord"></a><span data-ttu-id="9d28e-103">Obter callRecord</span><span class="sxs-lookup"><span data-stu-id="9d28e-103">Get callRecord</span></span>

<span data-ttu-id="9d28e-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="9d28e-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d28e-105">Recupere as propriedades e os relacionamentos de um objeto [callRecord](../resources/callrecords-callrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="9d28e-105">Retrieve the properties and relationships of a [callRecord](../resources/callrecords-callrecord.md) object.</span></span>

<span data-ttu-id="9d28e-106">Há duas maneiras de obter o **ID** de um **callRecord**:</span><span class="sxs-lookup"><span data-stu-id="9d28e-106">There are two ways to get the **id** of a **callRecord**:</span></span>

* <span data-ttu-id="9d28e-107">Assine as [notificações de alteração](/graph/api/resources/webhooks?view=graph-rest-beta) para o `/communications/callRecords` ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="9d28e-107">Subscribe to [change notifications](/graph/api/resources/webhooks?view=graph-rest-beta) to the `/communications/callRecords` endpoint.</span></span>
* <span data-ttu-id="9d28e-108">Use a propriedade **callChainId** de uma [chamada](../resources/call.md).</span><span class="sxs-lookup"><span data-stu-id="9d28e-108">Use the **callChainId** property of a [call](../resources/call.md).</span></span> <span data-ttu-id="9d28e-109">O registro de chamadas estará disponível somente após a conclusão da chamada associada.</span><span class="sxs-lookup"><span data-stu-id="9d28e-109">The call record is available only after the associated call is completed.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d28e-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="9d28e-110">Permissions</span></span>

<span data-ttu-id="9d28e-111">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="9d28e-111">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="9d28e-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d28e-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9d28e-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d28e-113">Permission type</span></span>                        | <span data-ttu-id="9d28e-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9d28e-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9d28e-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d28e-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="9d28e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d28e-116">Not supported.</span></span> |
| <span data-ttu-id="9d28e-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d28e-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d28e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d28e-118">Not supported.</span></span> |
| <span data-ttu-id="9d28e-119">Application</span><span class="sxs-lookup"><span data-stu-id="9d28e-119">Application</span></span>                            | <span data-ttu-id="9d28e-120">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d28e-120">CallRecords.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d28e-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d28e-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /communications/callRecords/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9d28e-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9d28e-122">Optional query parameters</span></span>

<span data-ttu-id="9d28e-123">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9d28e-123">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="9d28e-124">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9d28e-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d28e-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d28e-125">Request headers</span></span>

| <span data-ttu-id="9d28e-126">Nome</span><span class="sxs-lookup"><span data-stu-id="9d28e-126">Name</span></span>      |<span data-ttu-id="9d28e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d28e-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9d28e-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d28e-128">Authorization</span></span> | <span data-ttu-id="9d28e-129">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="9d28e-129">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d28e-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d28e-130">Request body</span></span>

<span data-ttu-id="9d28e-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9d28e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d28e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d28e-132">Response</span></span>

<span data-ttu-id="9d28e-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [Microsoft. Graph. CallRecords. callRecord](../resources/callrecords-callrecord.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d28e-133">If successful, this method returns a `200 OK` response code and the requested [microsoft.graph.callRecords.callRecord](../resources/callrecords-callrecord.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9d28e-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9d28e-134">Examples</span></span>

### <a name="example-1-get-basic-details"></a><span data-ttu-id="9d28e-135">Exemplo 1: obter detalhes básicos</span><span class="sxs-lookup"><span data-stu-id="9d28e-135">Example 1: Get basic details</span></span>

#### <a name="request"></a><span data-ttu-id="9d28e-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d28e-136">Request</span></span>

<span data-ttu-id="9d28e-137">Veja a seguir um exemplo da solicitação para obter os detalhes básicos de um [callRecord](../resources/callrecords-callrecord.md).</span><span class="sxs-lookup"><span data-stu-id="9d28e-137">The following is an example of the request to get the basic details from a [callRecord](../resources/callrecords-callrecord.md).</span></span>


# <a name="http"></a>[<span data-ttu-id="9d28e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d28e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_callrecord"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/callRecords/{id}
```
# <a name="c"></a>[<span data-ttu-id="9d28e-139">C#</span><span class="sxs-lookup"><span data-stu-id="9d28e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-callrecord-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d28e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d28e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-callrecord-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d28e-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d28e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-callrecord-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9d28e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d28e-142">Response</span></span>

<span data-ttu-id="9d28e-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9d28e-143">The following is an example of the response.</span></span>

> <span data-ttu-id="9d28e-144">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="9d28e-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9d28e-145">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="9d28e-145">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.callRecord"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#communications/callRecords/$entity",
    "version": 1,
    "type": "peerToPeer",
    "modalities": [
        "audio"
    ],
    "lastModifiedDateTime": "2020-02-25T19:00:24.582757Z",
    "startDateTime": "2020-02-25T18:52:21.2169889Z",
    "endDateTime": "2020-02-25T18:52:46.7640013Z",
    "id": "e523d2ed-2966-4b6b-925b-754a88034cc5",
    "organizer": {
        "user": {
            "id": "821809f5-0000-0000-0000-3b5136c0e777",
            "displayName": "Abbie Wilkins",
            "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
        }
    },
    "participants": [
        {
            "user": {
                "id": "821809f5-0000-0000-0000-3b5136c0e777",
                "displayName": "Abbie Wilkins",
                "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
            }
        },
        {
            "user": {
                "id": "f69e2c00-0000-0000-0000-185e5f5f5d8a",
                "displayName": "Owen Franklin",
                "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
            }
        }
    ]
}
```

### <a name="example-2-get-full-details"></a><span data-ttu-id="9d28e-146">Exemplo 2: obter detalhes completos</span><span class="sxs-lookup"><span data-stu-id="9d28e-146">Example 2: Get full details</span></span>

#### <a name="request"></a><span data-ttu-id="9d28e-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d28e-147">Request</span></span>

<span data-ttu-id="9d28e-148">Veja a seguir um exemplo da solicitação para obter os detalhes completos de um [callRecord](../resources/callrecords-callrecord.md), incluindo componentes de sessão e de segmento.</span><span class="sxs-lookup"><span data-stu-id="9d28e-148">The following is an example of the request to get the full details from a [callRecord](../resources/callrecords-callrecord.md), including session and segment components.</span></span>


# <a name="http"></a>[<span data-ttu-id="9d28e-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d28e-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_callrecord_expanded"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/callRecords/{id}?$expand=sessions($expand=segments)
```
# <a name="c"></a>[<span data-ttu-id="9d28e-150">C#</span><span class="sxs-lookup"><span data-stu-id="9d28e-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-callrecord-expanded-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d28e-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d28e-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-callrecord-expanded-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d28e-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d28e-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-callrecord-expanded-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9d28e-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d28e-153">Response</span></span>

<span data-ttu-id="9d28e-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9d28e-154">The following is an example of the response.</span></span> <span data-ttu-id="9d28e-155">Se a lista de sessões estiver truncada, `sessions@odata.nextlink` será fornecido um valor para recuperar a próxima página de sessões.</span><span class="sxs-lookup"><span data-stu-id="9d28e-155">If the sessions list is truncated, a `sessions@odata.nextlink` value will be provided to retrieve the next page of sessions.</span></span>

> <span data-ttu-id="9d28e-156">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="9d28e-156">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9d28e-157">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="9d28e-157">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.callRecord"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#communications/callRecords(sessions(segments()))/$entity",
    "version": 1,
    "type": "peerToPeer",
    "modalities": [
        "audio"
    ],
    "lastModifiedDateTime": "2020-02-25T19:00:24.582757Z",
    "startDateTime": "2020-02-25T18:52:21.2169889Z",
    "endDateTime": "2020-02-25T18:52:46.7640013Z",
    "id": "e523d2ed-2966-4b6b-925b-754a88034cc5",
    "organizer": {
        "user": {
            "id": "821809f5-0000-0000-0000-3b5136c0e777",
            "displayName": "Abbie Wilkins",
            "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
        }
    },
    "participants": [
        {
            "user": {
                "id": "821809f5-0000-0000-0000-3b5136c0e777",
                "displayName": "Abbie Wilkins",
                "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
            }
        },
        {
            "user": {
                "id": "f69e2c00-0000-0000-0000-185e5f5f5d8a",
                "displayName": "Owen Franklin",
                "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
            }
        }
    ],
    "sessions@odata.context": "https://graph.microsoft.com/beta/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions(segments())",
    "sessions": [
        {
            "modalities": [
                "audio"
            ],
            "startDateTime": "2020-02-25T18:52:21.2169889Z",
            "endDateTime": "2020-02-25T18:52:46.7640013Z",
            "id": "e523d2ed-2966-4b6b-925b-754a88034cc5",
            "caller": {
                "@odata.type": "#microsoft.graph.callRecords.participantEndpoint",
                "userAgent": {
                    "@odata.type": "#microsoft.graph.callRecords.clientUserAgent",
                    "headerValue": "RTCC/7.0.0.0 UCWA/7.0.0.0 AndroidLync/6.25.0.27 (SM-G930U Android 8.0.0)",
                    "platform": "android",
                    "productFamily": "skypeForBusiness"
                },
                "identity": {
                    "@odata.type": "#microsoft.graph.identitySet",
                    "user": {
                        "id": "821809f5-0000-0000-0000-3b5136c0e777",
                        "displayName": "Abbie Wilkins",
                        "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
                    }
                }
            },
            "callee": {
                "@odata.type": "#microsoft.graph.callRecords.participantEndpoint",
                "userAgent": {
                    "@odata.type": "#microsoft.graph.callRecords.clientUserAgent",
                    "headerValue": "UCCAPI/16.0.12527.20122 OC/16.0.12527.20194 (Skype for Business)",
                    "platform": "windows",
                    "productFamily": "skypeForBusiness"
                },
                "identity": {
                    "user": {
                        "id": "f69e2c00-0000-0000-0000-185e5f5f5d8a",
                        "displayName": "Owen Franklin",
                        "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
                    }
                },
                "feedback": {
                    "rating": "poor",
                    "tokens": {
                        "NoSound": false,
                        "OtherNoSound": false,
                        "Echo": false,
                        "Noisy": true,
                        "LowVolume": false,
                        "Stopped": false,
                        "DistortedSound": false,
                        "Interruptions": false
                    }
                }
            },
            "segments@odata.context": "https://graph.microsoft.com/beta/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions('e523d2ed-2966-4b6b-925b-754a88034cc5')/segments",
            "segments": [
                {
                    "startDateTime": "2020-02-25T18:52:21.2169889Z",
                    "endDateTime": "2020-02-25T18:52:46.7640013Z",
                    "id": "e523d2ed-2966-4b6b-925b-754a88034cc5",
                    "caller": {
                        "@odata.type": "#microsoft.graph.callRecords.participantEndpoint",
                        "userAgent": {
                            "@odata.type": "#microsoft.graph.callRecords.clientUserAgent",
                            "headerValue": "RTCC/7.0.0.0 UCWA/7.0.0.0 AndroidLync/6.25.0.27 (SM-G930U Android 8.0.0)",
                            "platform": "android",
                            "productFamily": "skypeForBusiness"
                        },
                        "identity": {
                            "user": {
                                "id": "821809f5-0000-0000-0000-3b5136c0e777",
                                "displayName": "Abbie Wilkins",
                                "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
                            }
                        }
                    },
                    "callee": {
                        "@odata.type": "#microsoft.graph.callRecords.participantEndpoint",
                        "userAgent": {
                            "@odata.type": "#microsoft.graph.callRecords.clientUserAgent",
                            "headerValue": "UCCAPI/16.0.12527.20122 OC/16.0.12527.20194 (Skype for Business)",
                            "platform": "windows",
                            "productFamily": "skypeForBusiness"
                        },
                        "identity": {
                            "user": {
                                "id": "f69e2c00-0000-0000-0000-185e5f5f5d8a",
                                "displayName": "Owen Franklin",
                                "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
                            }
                        }
                    },
                    "media": [
                        {
                            "label": "main-audio",
                            "callerNetwork": {
                                "ipAddress": "10.150.0.2",
                                "subnet": "10.150.0.0",
                                "linkSpeed": 54000000,
                                "connectionType": "wifi",
                                "port": 27288,
                                "reflexiveIPAddress": "127.0.0.2",
                                "relayIPAddress": "52.114.188.32",
                                "relayPort": 53889,
                                "macAddress": "00-00-00-00-00-00",
                                "dnsSuffix": null,
                                "sentQualityEventRatio": 0,
                                "receivedQualityEventRatio": 0.27,
                                "delayEventRatio": 0,
                                "bandwidthLowEventRatio": 0
                            },
                            "calleeNetwork": {
                                "ipAddress": "10.139.0.12",
                                "subnet": "10.139.80.0",
                                "linkSpeed": 4294967295,
                                "connectionType": "wired",
                                "port": 50011,
                                "reflexiveIPAddress": "127.0.0.2",
                                "relayIPAddress": "52.114.188.102",
                                "relayPort": 52810,
                                "macAddress": "00-00-00-00-00-00-00-00",
                                "dnsSuffix": null,
                                "sentQualityEventRatio": 0.31,
                                "receivedQualityEventRatio": 0,
                                "delayEventRatio": 0,
                                "bandwidthLowEventRatio": 0
                            },
                            "callerDevice": {
                                "captureDeviceName": "Default input device",
                                "renderDeviceName": "Default output device",
                                "receivedSignalLevel": -10,
                                "receivedNoiseLevel": -68,
                                "initialSignalLevelRootMeanSquare": 60.25816,
                                "renderZeroVolumeEventRatio": 1,
                                "renderMuteEventRatio": 1,
                                "micGlitchRate": 23,
                                "speakerGlitchRate": 3830
                            },
                            "calleeDevice": {
                                "captureDeviceName": "Microphone (Microsoft Virtual Audio Device (Simple) (WDM))",
                                "captureDeviceDriver": "Microsoft: 5.0.8638.1100",
                                "renderDeviceName": "Speakers (Microsoft Virtual Audio Device (Simple) (WDM))",
                                "renderDeviceDriver": "Microsoft: 5.0.8638.1100",
                                "receivedSignalLevel": -14,
                                "receivedNoiseLevel": -86,
                                "initialSignalLevelRootMeanSquare": 146.7885,
                                "micGlitchRate": 143,
                                "speakerGlitchRate": 182
                            },
                            "streams": [
                                {
                                    "streamId": "1504545584",
                                    "streamDirection": "callerToCallee",
                                    "averageAudioDegradation": null,
                                    "averageJitter": "PT0.016S",
                                    "maxJitter": "PT0.021S",
                                    "averagePacketLossRate": 0,
                                    "maxPacketLossRate": 0,
                                    "averageRatioOfConcealedSamples": null,
                                    "maxRatioOfConcealedSamples": null,
                                    "averageRoundTripTime": "PT0.061S",
                                    "maxRoundTripTime": "PT0.079S",
                                    "packetUtilization": 67,
                                    "averageBandwidthEstimate": 9965083,
                                    "wasMediaBypassed": false,
                                    "averageAudioNetworkJitter": "PT0.043S",
                                    "maxAudioNetworkJitter": "PT0.046S"
                                },
                                {
                                    "streamId": "1785122252",
                                    "streamDirection": "calleeToCaller",
                                    "averageAudioDegradation": 1.160898,
                                    "averageJitter": "PT0.007S",
                                    "maxJitter": "PT0.012S",
                                    "averagePacketLossRate": 0.01381693,
                                    "maxPacketLossRate": 0.03738318,
                                    "averageRatioOfConcealedSamples": 0.06233422,
                                    "maxRatioOfConcealedSamples": 0.07192807,
                                    "averageRoundTripTime": "PT0.064S",
                                    "maxRoundTripTime": "PT0.106S",
                                    "packetUtilization": 709,
                                    "averageBandwidthEstimate": 15644878,
                                    "wasMediaBypassed": false,
                                    "averageAudioNetworkJitter": "PT0.266S",
                                    "maxAudioNetworkJitter": "PT0.474S"
                                }
                            ]
                        }
                    ]
                }
            ]
        }
    ],
    "sessions@odata.nextlink": "https://graph.microsoft.com/beta/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions?$expand=segments&$skiptoken=abc"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get callRecord",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
