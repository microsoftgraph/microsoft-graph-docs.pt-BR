---
title: Listar participantes
description: Recupere uma lista de objetos participantes na chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: c9e9fb8e1ea8a78629aa7c1fdf5639864a4f5162
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912850"
---
# <a name="list-participants"></a><span data-ttu-id="38ce1-103">Listar participantes</span><span class="sxs-lookup"><span data-stu-id="38ce1-103">List participants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38ce1-104">Recupere uma lista de objetos participantes na chamada.</span><span class="sxs-lookup"><span data-stu-id="38ce1-104">Retrieve a list of participant objects in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="38ce1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="38ce1-105">Permissions</span></span>

| <span data-ttu-id="38ce1-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38ce1-106">Permission type</span></span> | <span data-ttu-id="38ce1-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38ce1-107">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="38ce1-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38ce1-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="38ce1-109">Não suportado</span><span class="sxs-lookup"><span data-stu-id="38ce1-109">Not Supported</span></span>        |
| <span data-ttu-id="38ce1-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38ce1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38ce1-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="38ce1-111">Not Supported</span></span>        |
| <span data-ttu-id="38ce1-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38ce1-112">Application</span></span>     | <span data-ttu-id="38ce1-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="38ce1-113">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="38ce1-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38ce1-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /app/calls/{id}/participants
GET /communications/calls/{id}/participants
```
> <span data-ttu-id="38ce1-115">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="38ce1-115">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="38ce1-116">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="38ce1-116">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="38ce1-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="38ce1-117">Optional query parameters</span></span>

<span data-ttu-id="38ce1-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="38ce1-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38ce1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38ce1-119">Request headers</span></span>

| <span data-ttu-id="38ce1-120">Nome</span><span class="sxs-lookup"><span data-stu-id="38ce1-120">Name</span></span>          | <span data-ttu-id="38ce1-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="38ce1-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="38ce1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="38ce1-122">Authorization</span></span> | <span data-ttu-id="38ce1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38ce1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38ce1-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38ce1-125">Request body</span></span>

<span data-ttu-id="38ce1-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="38ce1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38ce1-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="38ce1-127">Response</span></span>

<span data-ttu-id="38ce1-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [participantes](../resources/participant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38ce1-128">If successful, this method returns a `200 OK` response code and collection of [participant](../resources/participant.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38ce1-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38ce1-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="38ce1-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38ce1-130">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="38ce1-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="38ce1-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-participants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="38ce1-132">C#</span><span class="sxs-lookup"><span data-stu-id="38ce1-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-participants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="38ce1-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38ce1-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-participants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="38ce1-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38ce1-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-participants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="38ce1-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="38ce1-135">Response</span></span>

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
