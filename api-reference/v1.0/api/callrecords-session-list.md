---
title: Listar sessões do callRecord
description: Recupere a lista de objetos de sessão para um callRecord.
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 084731b05439b4e22cb16064f5703bab362a84ad
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491934"
---
# <a name="list-callrecord-sessions"></a><span data-ttu-id="4455e-103">Listar sessões do callRecord</span><span class="sxs-lookup"><span data-stu-id="4455e-103">List callRecord sessions</span></span>

<span data-ttu-id="4455e-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="4455e-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="4455e-105">Recupere a lista de [sessões](../resources/callrecords-session.md) associadas a um objeto [callRecord](../resources/callrecords-callrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="4455e-105">Retrieve the list of [sessions](../resources/callrecords-session.md) associated with a [callRecord](../resources/callrecords-callrecord.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4455e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4455e-106">Permissions</span></span>

<span data-ttu-id="4455e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4455e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4455e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4455e-109">Permission type</span></span>                        | <span data-ttu-id="4455e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4455e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4455e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4455e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4455e-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4455e-112">Not supported.</span></span> |
| <span data-ttu-id="4455e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4455e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4455e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4455e-114">Not supported.</span></span> |
| <span data-ttu-id="4455e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4455e-115">Application</span></span>                            | <span data-ttu-id="4455e-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="4455e-116">CallRecords.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4455e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4455e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /communications/callRecords/{id}/sessions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4455e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4455e-118">Optional query parameters</span></span>

<span data-ttu-id="4455e-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4455e-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4455e-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4455e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4455e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4455e-121">Request headers</span></span>

| <span data-ttu-id="4455e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4455e-122">Name</span></span>      |<span data-ttu-id="4455e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4455e-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4455e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4455e-124">Authorization</span></span> | <span data-ttu-id="4455e-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="4455e-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4455e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4455e-126">Request body</span></span>

<span data-ttu-id="4455e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4455e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4455e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4455e-128">Response</span></span>

<span data-ttu-id="4455e-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e os objetos de [sessão](../resources/callrecords-session.md) solicitados no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4455e-129">If successful, this method returns a `200 OK` response code and the requested [session](../resources/callrecords-session.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4455e-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4455e-130">Examples</span></span>

### <a name="example-1-get-session-list"></a><span data-ttu-id="4455e-131">Exemplo 1: obter lista de sessão</span><span class="sxs-lookup"><span data-stu-id="4455e-131">Example 1: Get session list</span></span>

#### <a name="request"></a><span data-ttu-id="4455e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4455e-132">Request</span></span>

<span data-ttu-id="4455e-133">Veja a seguir um exemplo da solicitação para obter a lista de [sessões](../resources/callrecords-session.md) de um [callRecord](../resources/callrecords-callrecord.md).</span><span class="sxs-lookup"><span data-stu-id="4455e-133">The following is an example of the request to get the list of [sessions](../resources/callrecords-session.md) for a [callRecord](../resources/callrecords-callrecord.md).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_callrecord_sessions"
}-->

```http
GET https://graph.microsoft.com/v1.0/communications/callRecords/{id}/sessions
```

#### <a name="response"></a><span data-ttu-id="4455e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4455e-134">Response</span></span>

<span data-ttu-id="4455e-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4455e-135">The following is an example of the response.</span></span>

> <span data-ttu-id="4455e-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4455e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.session",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions",
    "value": [
        {
            "id": "e523d2ed-2966-4b6b-925b-754a88034cc5",
            "modalities": [
                "audio"
            ],
            "startDateTime": "2020-02-25T18:52:21.2169889Z",
            "endDateTime": "2020-02-25T18:52:46.7640013Z",
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
            }
        }
    ],
    "@odata.nextlink": "https://graph.microsoft.com/v1.0/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions?$skiptoken=abc"
}
```

### <a name="example-2-get-session-list-with-segments"></a><span data-ttu-id="4455e-138">Exemplo 2: obter a lista de sessão com segmentos</span><span class="sxs-lookup"><span data-stu-id="4455e-138">Example 2: Get session list with segments</span></span>

#### <a name="request"></a><span data-ttu-id="4455e-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4455e-139">Request</span></span>

<span data-ttu-id="4455e-140">Veja a seguir um exemplo da solicitação para obter a lista de [sessões](../resources/callrecords-session.md) para um [callRecord](../resources/callrecords-callrecord.md) com [segmentos](../resources/callrecords-segment.md) incluídos.</span><span class="sxs-lookup"><span data-stu-id="4455e-140">The following is an example of the request to get the list of [sessions](../resources/callrecords-session.md) for a [callRecord](../resources/callrecords-callrecord.md) with [segments](../resources/callrecords-segment.md) included.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_callrecord_sessions_expanded"
}-->

```http
GET https://graph.microsoft.com/v1.0/communications/callRecords/{id}/sessions?$expand=segments
```

#### <a name="response"></a><span data-ttu-id="4455e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="4455e-141">Response</span></span>

<span data-ttu-id="4455e-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4455e-142">The following is an example of the response.</span></span>

> <span data-ttu-id="4455e-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4455e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.session",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions",
    "value": [
        {
            "id": "e523d2ed-2966-4b6b-925b-754a88034cc5",
            "modalities": [
                "audio"
            ],
            "startDateTime": "2020-02-25T18:52:21.2169889Z",
            "endDateTime": "2020-02-25T18:52:46.7640013Z",
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
            "segments@odata.context": "https://graph.microsoft.com/v1.0/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions('e523d2ed-2966-4b6b-925b-754a88034cc5')/segments",
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
    "@odata.nextlink": "https://graph.microsoft.com/v1.0/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions?$expand=segments&$skiptoken=abc"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List sessions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
