---
title: Listar participantes
description: Recupere uma lista de objetos participantes na chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 94017581dd76297fb3c55bce7ef82ea966144b63
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987369"
---
# <a name="list-participants"></a><span data-ttu-id="cabbf-103">Listar participantes</span><span class="sxs-lookup"><span data-stu-id="cabbf-103">List participants</span></span>

<span data-ttu-id="cabbf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cabbf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cabbf-105">Recupere uma lista de objetos participantes na chamada.</span><span class="sxs-lookup"><span data-stu-id="cabbf-105">Retrieve a list of participant objects in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="cabbf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cabbf-106">Permissions</span></span>

| <span data-ttu-id="cabbf-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cabbf-107">Permission type</span></span> | <span data-ttu-id="cabbf-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cabbf-108">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="cabbf-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cabbf-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="cabbf-110">Não suportado</span><span class="sxs-lookup"><span data-stu-id="cabbf-110">Not Supported</span></span>        |
| <span data-ttu-id="cabbf-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cabbf-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cabbf-112">Não suportado</span><span class="sxs-lookup"><span data-stu-id="cabbf-112">Not Supported</span></span>        |
| <span data-ttu-id="cabbf-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cabbf-113">Application</span></span>     | <span data-ttu-id="cabbf-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cabbf-114">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="cabbf-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cabbf-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /app/calls/{id}/participants
GET /communications/calls/{id}/participants
```
> <span data-ttu-id="cabbf-116">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="cabbf-116">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="cabbf-117">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="cabbf-117">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="cabbf-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cabbf-118">Optional query parameters</span></span>

<span data-ttu-id="cabbf-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cabbf-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cabbf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cabbf-120">Request headers</span></span>

| <span data-ttu-id="cabbf-121">Nome</span><span class="sxs-lookup"><span data-stu-id="cabbf-121">Name</span></span>          | <span data-ttu-id="cabbf-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="cabbf-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="cabbf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cabbf-123">Authorization</span></span> | <span data-ttu-id="cabbf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cabbf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cabbf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cabbf-126">Request body</span></span>

<span data-ttu-id="cabbf-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cabbf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cabbf-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="cabbf-128">Response</span></span>

<span data-ttu-id="cabbf-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [participantes](../resources/participant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cabbf-129">If successful, this method returns a `200 OK` response code and collection of [participant](../resources/participant.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cabbf-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cabbf-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="cabbf-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cabbf-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="cabbf-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="cabbf-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-participants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants
```
# <a name="c"></a>[<span data-ttu-id="cabbf-133">C#</span><span class="sxs-lookup"><span data-stu-id="cabbf-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-participants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cabbf-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cabbf-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-participants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cabbf-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cabbf-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-participants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="cabbf-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="cabbf-136">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.participant",
  "isCollection": true,
  "truncated": true
}-->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "value":[
      {
         "@odata.type":"#microsoft.graph.participant",
         "info":{
            "@odata.type":"#microsoft.graph.participantInfo",
            "identity":{
               "@odata.type":"#microsoft.graph.identitySet",
               "application":{
                  "@odata.type":"#microsoft.graph.identity",
                  "id":"f2fa86af-3c51-4bc2-8fc0-475452d9764f",
                  "displayName":null
               },
               "user":null,
               "device":null,
               "phone":null
            },
            "id":"eec3812a-fdc3-4fb4-825c-a06c9f35414e"
         },
         "mediaStreams":[
            {
               "@odata.type":"#microsoft.graph.mediaStream",
               "mediaType":"audio",
               "sourceId":"3",
               "direction":"sendReceive",
               "serverMuted":false,
               "label":null
            }
         ],
         "isMuted":false,
         "isInLobby":false,
         "id":"a7ebfb2d-871e-419c-87af-27290b22e8db",
         "metadata":null,
         "recordingInfo":null
      },
      {
         "@odata.type":"#microsoft.graph.participant",
         "info":{
            "@odata.type":"#microsoft.graph.participantInfo",
            "identity":{
               "@odata.type":"#microsoft.graph.identitySet",
               "application":{
                  "@odata.type":"#microsoft.graph.identity",
                  "displayName":"Test Participant",
                  "id":"ef43e42b-4c05-4594-9756-1edb3ccbc989",
                  "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
               },
               "user":null,
               "device":null,
               "phone":null
            },
            "id":"278405a3-f568-4b3e-b684-009193463064"
         },
         "mediaStreams":[
            {
               "@odata.type":"#microsoft.graph.mediaStream",
               "mediaType":"audio",
               "sourceId":"1",
               "direction":"sendReceive",
               "serverMuted":false,
               "label":null
            }
         ],
         "isMuted":false,
         "isInLobby":false,
         "id":"1e126418-44a0-4a94-a6f8-0efe1ad71acb",
         "metadata":null,
         "recordingInfo":null
      }
   ],
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#communications/calls('7531d31f-d10d-44de-802f-c569dbca451c')/participants"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List participants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


