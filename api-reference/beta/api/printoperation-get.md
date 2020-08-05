---
title: Obter operação
description: Recupere uma operação.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: dd03367e71a9c5273e294ac022d4ac9d8a5e2760
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565623"
---
# <a name="get-printoperation"></a><span data-ttu-id="45794-103">Obter operação</span><span class="sxs-lookup"><span data-stu-id="45794-103">Get printOperation</span></span>

<span data-ttu-id="45794-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45794-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45794-105">Recupere as propriedades e os relacionamentos de um objeto Print [Operation](../resources/printoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="45794-105">Retrieve the properties and relationships of a [printOperation](../resources/printoperation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="45794-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="45794-106">Permissions</span></span>
<span data-ttu-id="45794-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45794-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45794-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45794-109">Permission type</span></span> | <span data-ttu-id="45794-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="45794-110">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="45794-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45794-111">Delegated (work or school account)</span></span>| <span data-ttu-id="45794-112">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="45794-112">User.Read.All</span></span> |
|<span data-ttu-id="45794-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45794-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45794-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45794-114">Not Supported.</span></span>|
|<span data-ttu-id="45794-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45794-115">Application</span></span>|<span data-ttu-id="45794-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45794-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45794-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45794-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/operations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="45794-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45794-118">Request headers</span></span>
| <span data-ttu-id="45794-119">Nome</span><span class="sxs-lookup"><span data-stu-id="45794-119">Name</span></span>      |<span data-ttu-id="45794-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="45794-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="45794-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="45794-121">Authorization</span></span> | <span data-ttu-id="45794-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45794-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="45794-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45794-124">Request body</span></span>
<span data-ttu-id="45794-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="45794-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="45794-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="45794-126">Response</span></span>
<span data-ttu-id="45794-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [reoperation](../resources/printOperation.md) (ou uma derivada de **reoperation**) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45794-127">If successful, this method returns a `200 OK` response code and a [printOperation](../resources/printOperation.md) object (or a derivative of **printOperation**) in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="45794-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45794-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="45794-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45794-129">Request</span></span>
<span data-ttu-id="45794-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="45794-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="45794-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="45794-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printoperation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/operations/{id}
```
# <a name="c"></a>[<span data-ttu-id="45794-132">C#</span><span class="sxs-lookup"><span data-stu-id="45794-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45794-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45794-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45794-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45794-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="45794-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="45794-135">Response</span></span>
<span data-ttu-id="45794-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="45794-136">The following is an example of the response.</span></span>
><span data-ttu-id="45794-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45794-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1199

{
    "@odata.context": "https://graph.microsoft-ppe.com/beta/$metadata#print/operations/$entity",
    "@odata.type": "#microsoft.graph.printerCreateOperation",
    "id": "81f4cca3-b3b7-47ea-9f88-7ddbf7208ef4",
    "createdDateTime": "2020-06-15T22:27:03.031849Z",
    "certificate": "{ceritificate}",
    "status": {
        "state": "succeeded",
        "description": "The operation has completed successfully."
    },
    "printer": {
        "registeredDateTime": "2020-06-15T22:27:12.0920077Z",
        "acceptingJobs": null,
        "isShared": false,
        "id": "e56f9cdd-acec-486f-a05e-b622ff0bcc7d",
        "name": "Test Printer",
        "manufacturer": "Test Printer Manufacturer",
        "model": "Test Printer Model",
        "isAcceptingJobs": null,
        "capabilities": null,
        "status": {
            "processingState": "unknown",
            "processingStateReasons": [],
            "processingStateDescription": ""
        },
        "location": {
            "latitude": null,
            "longitude": null
        },
        "defaults": {
            "copiesPerJob": 1,
            "finishings": []
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
