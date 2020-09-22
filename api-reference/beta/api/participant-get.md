---
title: Obter participante
description: Recupere as propriedades e os relacionamentos de um objeto **participante** .
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: dd384696792e804ffcd39fd52a9693131133f7be
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004568"
---
# <a name="get-participant"></a><span data-ttu-id="1b704-103">Obter participante</span><span class="sxs-lookup"><span data-stu-id="1b704-103">Get participant</span></span>

<span data-ttu-id="1b704-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1b704-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b704-105">Recupere as propriedades e os relacionamentos de um objeto **participante** .</span><span class="sxs-lookup"><span data-stu-id="1b704-105">Retrieve the properties and relationships of a **participant** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b704-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b704-106">Permissions</span></span>

| <span data-ttu-id="1b704-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b704-107">Permission type</span></span> | <span data-ttu-id="1b704-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b704-108">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="1b704-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b704-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="1b704-110">Não suportado</span><span class="sxs-lookup"><span data-stu-id="1b704-110">Not Supported</span></span>        |
| <span data-ttu-id="1b704-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b704-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b704-112">Não suportado</span><span class="sxs-lookup"><span data-stu-id="1b704-112">Not Supported</span></span>        |
| <span data-ttu-id="1b704-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b704-113">Application</span></span>     | <span data-ttu-id="1b704-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1b704-114">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="1b704-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b704-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/participants/{id}
GET /communications/calls/{id}/participants/{id}
```
> <span data-ttu-id="1b704-116">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="1b704-116">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="1b704-117">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="1b704-117">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="1b704-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1b704-118">Optional query parameters</span></span>
<span data-ttu-id="1b704-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1b704-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b704-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b704-120">Request headers</span></span>
| <span data-ttu-id="1b704-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1b704-121">Name</span></span>          | <span data-ttu-id="1b704-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b704-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1b704-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b704-123">Authorization</span></span> | <span data-ttu-id="1b704-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b704-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b704-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b704-126">Request body</span></span>
<span data-ttu-id="1b704-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1b704-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b704-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b704-128">Response</span></span>
<span data-ttu-id="1b704-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [participante](../resources/participant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b704-129">If successful, this method returns a `200 OK` response code and a [participant](../resources/participant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b704-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b704-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1b704-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b704-131">Request</span></span>
<span data-ttu-id="1b704-132">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b704-132">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1b704-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b704-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-participant"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants/7e1b4346-85a6-4bdd-abe3-d11c5d420efe
```
# <a name="c"></a>[<span data-ttu-id="1b704-134">C#</span><span class="sxs-lookup"><span data-stu-id="1b704-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-participant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b704-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b704-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-participant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b704-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b704-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-participant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1b704-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b704-137">Response</span></span>

> <span data-ttu-id="1b704-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b704-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.participant"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "@odata.type":"#microsoft.graph.participant",
   "info":{
      "@odata.type":"#microsoft.graph.participantInfo",
      "identity":{
         "@odata.type":"#microsoft.graph.identitySet",
         "application":{
            "@odata.type":"#microsoft.graph.identity",
            "displayName":"Display Name",
            "id":"278405a3-f568-4b3e-b684-009193463064",
            "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
            },
         "user":null,
         "device":null,
         "phone":null
      },
      "id":null
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
   "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#communications/calls('7531d31f-d10d-44de-802f-c569dbca451c')/participants/$entity",
   "metadata":null,
   "recordingInfo":null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get participant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


