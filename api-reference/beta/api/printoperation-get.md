---
title: Obter operação
description: Recupere uma operação.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 85b0031d0bf4949a0309fbbe148c8f8119f0b032
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007135"
---
# <a name="get-printoperation"></a><span data-ttu-id="288ee-103">Obter operação</span><span class="sxs-lookup"><span data-stu-id="288ee-103">Get printOperation</span></span>

<span data-ttu-id="288ee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="288ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="288ee-105">Recupere as propriedades e os relacionamentos de um objeto Print [Operation](../resources/printoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="288ee-105">Retrieve the properties and relationships of a [printOperation](../resources/printoperation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="288ee-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="288ee-106">Permissions</span></span>
<span data-ttu-id="288ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="288ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="288ee-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="288ee-109">Permission type</span></span> | <span data-ttu-id="288ee-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="288ee-110">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="288ee-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="288ee-111">Delegated (work or school account)</span></span>| <span data-ttu-id="288ee-112">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="288ee-112">User.Read.All</span></span> |
|<span data-ttu-id="288ee-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="288ee-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="288ee-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="288ee-114">Not Supported.</span></span>|
|<span data-ttu-id="288ee-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="288ee-115">Application</span></span>|<span data-ttu-id="288ee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="288ee-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="288ee-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="288ee-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/operations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="288ee-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="288ee-118">Request headers</span></span>
| <span data-ttu-id="288ee-119">Nome</span><span class="sxs-lookup"><span data-stu-id="288ee-119">Name</span></span>      |<span data-ttu-id="288ee-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="288ee-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="288ee-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="288ee-121">Authorization</span></span> | <span data-ttu-id="288ee-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="288ee-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="288ee-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="288ee-124">Request body</span></span>
<span data-ttu-id="288ee-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="288ee-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="288ee-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="288ee-126">Response</span></span>
<span data-ttu-id="288ee-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [reoperation](../resources/printOperation.md) (ou uma derivada de **reoperation**) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="288ee-127">If successful, this method returns a `200 OK` response code and a [printOperation](../resources/printOperation.md) object (or a derivative of **printOperation**) in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="288ee-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="288ee-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="288ee-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="288ee-129">Request</span></span>
<span data-ttu-id="288ee-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="288ee-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_printoperation"
}-->
```http
GET https://graph.microsoft.com/beta/print/operations/{id}
```

### <a name="response"></a><span data-ttu-id="288ee-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="288ee-131">Response</span></span>
<span data-ttu-id="288ee-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="288ee-132">The following is an example of the response.</span></span>
><span data-ttu-id="288ee-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="288ee-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
