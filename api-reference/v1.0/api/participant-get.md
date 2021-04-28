---
title: Obter participante
description: Recupere as propriedades e as relações de um **objeto** participante.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d1d09c3bf78d604905a634245e45216fa94312c7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054508"
---
# <a name="get-participant"></a><span data-ttu-id="26cd8-103">Obter participante</span><span class="sxs-lookup"><span data-stu-id="26cd8-103">Get participant</span></span>

<span data-ttu-id="26cd8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26cd8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="26cd8-105">Recupere as propriedades e as relações de um **objeto** participante.</span><span class="sxs-lookup"><span data-stu-id="26cd8-105">Retrieve the properties and relationships of a **participant** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="26cd8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="26cd8-106">Permissions</span></span>

| <span data-ttu-id="26cd8-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26cd8-107">Permission type</span></span> | <span data-ttu-id="26cd8-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26cd8-108">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="26cd8-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26cd8-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="26cd8-110">Não suportado</span><span class="sxs-lookup"><span data-stu-id="26cd8-110">Not Supported</span></span>        |
| <span data-ttu-id="26cd8-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26cd8-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26cd8-112">Não suportado</span><span class="sxs-lookup"><span data-stu-id="26cd8-112">Not Supported</span></span>        |
| <span data-ttu-id="26cd8-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26cd8-113">Application</span></span>     | <span data-ttu-id="26cd8-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="26cd8-114">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="26cd8-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26cd8-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /communications/calls/{id}/participants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="26cd8-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="26cd8-116">Optional query parameters</span></span>
<span data-ttu-id="26cd8-117">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="26cd8-117">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="26cd8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26cd8-118">Request headers</span></span>
| <span data-ttu-id="26cd8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="26cd8-119">Name</span></span>          | <span data-ttu-id="26cd8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="26cd8-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="26cd8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="26cd8-121">Authorization</span></span> | <span data-ttu-id="26cd8-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26cd8-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26cd8-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26cd8-124">Request body</span></span>
<span data-ttu-id="26cd8-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="26cd8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26cd8-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="26cd8-126">Response</span></span>
<span data-ttu-id="26cd8-127">Se tiver êxito, este método retornará um código `200 OK` de resposta e um [objeto](../resources/participant.md) participante no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26cd8-127">If successful, this method returns a `200 OK` response code and a [participant](../resources/participant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26cd8-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26cd8-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="26cd8-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26cd8-129">Request</span></span>
<span data-ttu-id="26cd8-130">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="26cd8-130">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="26cd8-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="26cd8-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-participant"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants/7e1b4346-85a6-4bdd-abe3-d11c5d420efe
```
# <a name="c"></a>[<span data-ttu-id="26cd8-132">C#</span><span class="sxs-lookup"><span data-stu-id="26cd8-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-participant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26cd8-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26cd8-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-participant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26cd8-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26cd8-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-participant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26cd8-135">Java</span><span class="sxs-lookup"><span data-stu-id="26cd8-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-participant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="26cd8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="26cd8-136">Response</span></span>

> <span data-ttu-id="26cd8-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="26cd8-137">**Note:** The response object shown here might be shortened for readability.</span></span>

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
            "id":"278405a3-f568-4b3e-b684-009193463064"
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
   "metadata":null
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

