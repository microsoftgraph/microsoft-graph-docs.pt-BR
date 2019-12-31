---
title: Listar participantes
description: Recupere uma lista de objetos participantes na chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 94f7ebd36cbbabd6ab9bc41e32124c72da8d16c8
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913594"
---
# <a name="list-participants"></a><span data-ttu-id="c638c-103">Listar participantes</span><span class="sxs-lookup"><span data-stu-id="c638c-103">List participants</span></span>

<span data-ttu-id="c638c-104">Recupere uma lista de objetos participantes na chamada.</span><span class="sxs-lookup"><span data-stu-id="c638c-104">Retrieve a list of participant objects in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="c638c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c638c-105">Permissions</span></span>

| <span data-ttu-id="c638c-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c638c-106">Permission type</span></span> | <span data-ttu-id="c638c-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c638c-107">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="c638c-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c638c-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="c638c-109">Não suportado</span><span class="sxs-lookup"><span data-stu-id="c638c-109">Not Supported</span></span>        |
| <span data-ttu-id="c638c-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c638c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c638c-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="c638c-111">Not Supported</span></span>        |
| <span data-ttu-id="c638c-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c638c-112">Application</span></span>     | <span data-ttu-id="c638c-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c638c-113">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="c638c-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c638c-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /communications/calls/{id}/participants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c638c-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c638c-115">Optional query parameters</span></span>

<span data-ttu-id="c638c-116">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c638c-116">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c638c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c638c-117">Request headers</span></span>

| <span data-ttu-id="c638c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c638c-118">Name</span></span>          | <span data-ttu-id="c638c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c638c-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c638c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c638c-120">Authorization</span></span> | <span data-ttu-id="c638c-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c638c-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c638c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c638c-123">Request body</span></span>

<span data-ttu-id="c638c-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c638c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c638c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="c638c-125">Response</span></span>

<span data-ttu-id="c638c-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [participantes](../resources/participant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c638c-126">If successful, this method returns a `200 OK` response code and collection of [participant](../resources/participant.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c638c-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c638c-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="c638c-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c638c-128">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c638c-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="c638c-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-participants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c638c-130">C#</span><span class="sxs-lookup"><span data-stu-id="c638c-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-participants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c638c-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c638c-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-participants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c638c-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c638c-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-participants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c638c-133">Java</span><span class="sxs-lookup"><span data-stu-id="c638c-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-participants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="c638c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c638c-134">Response</span></span>

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
         "metadata":null
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
                  "id":"ef43e42b-4c05-4594-9756-1edb3ccbc989"
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
         "metadata":null
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
