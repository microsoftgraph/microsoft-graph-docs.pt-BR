---
title: Obter participante
description: Recupere as propriedades e os relacionamentos de um objeto **participante** .
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: ec9f7393db1101d529d92635159fc27ca7aeb8fe
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913433"
---
# <a name="get-participant"></a><span data-ttu-id="25a6a-103">Obter participante</span><span class="sxs-lookup"><span data-stu-id="25a6a-103">Get participant</span></span>

<span data-ttu-id="25a6a-104">Recupere as propriedades e os relacionamentos de um objeto **participante** .</span><span class="sxs-lookup"><span data-stu-id="25a6a-104">Retrieve the properties and relationships of a **participant** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="25a6a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="25a6a-105">Permissions</span></span>

| <span data-ttu-id="25a6a-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25a6a-106">Permission type</span></span> | <span data-ttu-id="25a6a-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="25a6a-107">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="25a6a-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25a6a-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="25a6a-109">Não suportado</span><span class="sxs-lookup"><span data-stu-id="25a6a-109">Not Supported</span></span>        |
| <span data-ttu-id="25a6a-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25a6a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25a6a-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="25a6a-111">Not Supported</span></span>        |
| <span data-ttu-id="25a6a-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25a6a-112">Application</span></span>     | <span data-ttu-id="25a6a-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="25a6a-113">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="25a6a-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25a6a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /communications/calls/{id}/participants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="25a6a-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="25a6a-115">Optional query parameters</span></span>
<span data-ttu-id="25a6a-116">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="25a6a-116">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="25a6a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25a6a-117">Request headers</span></span>
| <span data-ttu-id="25a6a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="25a6a-118">Name</span></span>          | <span data-ttu-id="25a6a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="25a6a-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="25a6a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="25a6a-120">Authorization</span></span> | <span data-ttu-id="25a6a-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25a6a-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25a6a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25a6a-123">Request body</span></span>
<span data-ttu-id="25a6a-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="25a6a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25a6a-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="25a6a-125">Response</span></span>
<span data-ttu-id="25a6a-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [participante](../resources/participant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25a6a-126">If successful, this method returns a `200 OK` response code and a [participant](../resources/participant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25a6a-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25a6a-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="25a6a-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25a6a-128">Request</span></span>
<span data-ttu-id="25a6a-129">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="25a6a-129">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="25a6a-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="25a6a-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-participant"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants/7e1b4346-85a6-4bdd-abe3-d11c5d420efe
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="25a6a-131">C#</span><span class="sxs-lookup"><span data-stu-id="25a6a-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-participant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="25a6a-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25a6a-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-participant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="25a6a-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25a6a-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-participant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="25a6a-134">Java</span><span class="sxs-lookup"><span data-stu-id="25a6a-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-participant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="25a6a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="25a6a-135">Response</span></span>

> <span data-ttu-id="25a6a-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="25a6a-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
