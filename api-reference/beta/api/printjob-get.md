---
title: Obter printJob
description: Recupere as propriedades e os relacionamentos de um trabalho de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: d1996ab8a7b1a5e8058654b54bba72907ba2fadf
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2020
ms.locfileid: "42947542"
---
# <a name="get-printjob"></a><span data-ttu-id="9a7d3-103">Obter printJob</span><span class="sxs-lookup"><span data-stu-id="9a7d3-103">Get printJob</span></span>

<span data-ttu-id="9a7d3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a7d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a7d3-105">Recupere as propriedades e os relacionamentos de um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="9a7d3-105">Retrieve the properties and relationships of a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a7d3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a7d3-106">Permissions</span></span>
<span data-ttu-id="9a7d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a7d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="9a7d3-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="9a7d3-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="9a7d3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a7d3-110">Permission type</span></span> | <span data-ttu-id="9a7d3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a7d3-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="9a7d3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a7d3-112">Delegated (work or school account)</span></span>| <span data-ttu-id="9a7d3-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="9a7d3-113">Users.Read.All</span></span> |
|<span data-ttu-id="9a7d3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a7d3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a7d3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a7d3-115">Not Supported.</span></span>|
|<span data-ttu-id="9a7d3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a7d3-116">Application</span></span>|<span data-ttu-id="9a7d3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a7d3-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a7d3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a7d3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9a7d3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a7d3-119">Request headers</span></span>
| <span data-ttu-id="9a7d3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9a7d3-120">Name</span></span>      |<span data-ttu-id="9a7d3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a7d3-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9a7d3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a7d3-122">Authorization</span></span> | <span data-ttu-id="9a7d3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a7d3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a7d3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a7d3-125">Request body</span></span>
<span data-ttu-id="9a7d3-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9a7d3-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9a7d3-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a7d3-127">Response</span></span>
<span data-ttu-id="9a7d3-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [printJob](../resources/printjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a7d3-128">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9a7d3-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a7d3-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a7d3-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a7d3-130">Request</span></span>
<span data-ttu-id="9a7d3-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a7d3-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9a7d3-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a7d3-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}
```
# <a name="c"></a>[<span data-ttu-id="9a7d3-133">C#</span><span class="sxs-lookup"><span data-stu-id="9a7d3-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a7d3-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a7d3-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a7d3-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a7d3-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9a7d3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a7d3-136">Response</span></span>
<span data-ttu-id="9a7d3-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9a7d3-137">The following is an example of the response.</span></span>
><span data-ttu-id="9a7d3-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a7d3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 408

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs/$entity",
  "id": "5182",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "createdBy": {},
  "status": {
    "processingState": "completed",
    "processingStateDescription": "The print job has completed successfully and no further processing will take place."
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
