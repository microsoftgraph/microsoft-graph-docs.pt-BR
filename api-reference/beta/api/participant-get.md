---
title: Obter participante
description: Recupere as propriedades e os relacionamentos de um objeto **participante** .
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 73ad70fa54104f973b59ae6f2f8c3b4196fe18e1
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006505"
---
# <a name="get-participant"></a><span data-ttu-id="22e72-103">Obter participante</span><span class="sxs-lookup"><span data-stu-id="22e72-103">Get participant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22e72-104">Recupere as propriedades e os relacionamentos de um objeto **participante** .</span><span class="sxs-lookup"><span data-stu-id="22e72-104">Retrieve the properties and relationships of a **participant** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="22e72-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="22e72-105">Permissions</span></span>

| <span data-ttu-id="22e72-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22e72-106">Permission type</span></span> | <span data-ttu-id="22e72-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="22e72-107">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="22e72-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22e72-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="22e72-109">Não suportado</span><span class="sxs-lookup"><span data-stu-id="22e72-109">Not Supported</span></span>        |
| <span data-ttu-id="22e72-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22e72-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22e72-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="22e72-111">Not Supported</span></span>        |
| <span data-ttu-id="22e72-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22e72-112">Application</span></span>     | <span data-ttu-id="22e72-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="22e72-113">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="22e72-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22e72-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/participants/{id}
GET /communications/calls/{id}/participants/{id}
```
> <span data-ttu-id="22e72-115">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="22e72-115">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="22e72-116">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="22e72-116">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="22e72-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="22e72-117">Optional query parameters</span></span>
<span data-ttu-id="22e72-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="22e72-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22e72-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22e72-119">Request headers</span></span>
| <span data-ttu-id="22e72-120">Nome</span><span class="sxs-lookup"><span data-stu-id="22e72-120">Name</span></span>          | <span data-ttu-id="22e72-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="22e72-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="22e72-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="22e72-122">Authorization</span></span> | <span data-ttu-id="22e72-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22e72-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22e72-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22e72-125">Request body</span></span>
<span data-ttu-id="22e72-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22e72-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22e72-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="22e72-127">Response</span></span>
<span data-ttu-id="22e72-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [participante](../resources/participant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22e72-128">If successful, this method returns a `200 OK` response code and a [participant](../resources/participant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22e72-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22e72-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="22e72-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22e72-130">Request</span></span>
<span data-ttu-id="22e72-131">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="22e72-131">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="22e72-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="22e72-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-participant"
}-->
```http
GET https://graph.microsoft.com/v1.0/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants/7e1b4346-85a6-4bdd-abe3-d11c5d420efe
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="22e72-133">C#</span><span class="sxs-lookup"><span data-stu-id="22e72-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-participant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22e72-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22e72-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-participant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="22e72-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22e72-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-participant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="22e72-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="22e72-136">Response</span></span>

> <span data-ttu-id="22e72-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22e72-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
