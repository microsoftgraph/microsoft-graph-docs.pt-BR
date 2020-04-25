---
title: Obter printJob
description: Recupere as propriedades e os relacionamentos de um trabalho de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 2833251d9d9ad7e65caafcebbc494f31c1ed8f7b
ms.sourcegitcommit: d2536f56e3a424219660bc0495ec8632932b4fb8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/25/2020
ms.locfileid: "43812489"
---
# <a name="get-printjob"></a><span data-ttu-id="16a97-103">Obter printJob</span><span class="sxs-lookup"><span data-stu-id="16a97-103">Get printJob</span></span>

<span data-ttu-id="16a97-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16a97-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16a97-105">Recupere as propriedades e os relacionamentos de um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="16a97-105">Retrieve the properties and relationships of a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="16a97-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="16a97-106">Permissions</span></span>
<span data-ttu-id="16a97-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16a97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="16a97-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="16a97-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="16a97-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16a97-110">Permission type</span></span> | <span data-ttu-id="16a97-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="16a97-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="16a97-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16a97-112">Delegated (work or school account)</span></span>| <span data-ttu-id="16a97-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="16a97-113">Users.Read.All</span></span> |
|<span data-ttu-id="16a97-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16a97-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16a97-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16a97-115">Not Supported.</span></span>|
|<span data-ttu-id="16a97-116">Application</span><span class="sxs-lookup"><span data-stu-id="16a97-116">Application</span></span>|<span data-ttu-id="16a97-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16a97-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16a97-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16a97-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="16a97-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="16a97-119">Optional query parameters</span></span>
<span data-ttu-id="16a97-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="16a97-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="16a97-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="16a97-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="16a97-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16a97-122">Request headers</span></span>
| <span data-ttu-id="16a97-123">Nome</span><span class="sxs-lookup"><span data-stu-id="16a97-123">Name</span></span>      |<span data-ttu-id="16a97-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="16a97-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="16a97-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="16a97-125">Authorization</span></span> | <span data-ttu-id="16a97-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16a97-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16a97-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16a97-128">Request body</span></span>
<span data-ttu-id="16a97-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="16a97-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="16a97-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="16a97-130">Response</span></span>
<span data-ttu-id="16a97-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [printJob](../resources/printjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16a97-131">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="16a97-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16a97-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="16a97-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16a97-133">Request</span></span>
<span data-ttu-id="16a97-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="16a97-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="16a97-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="16a97-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}
```
# <a name="c"></a>[<span data-ttu-id="16a97-136">C#</span><span class="sxs-lookup"><span data-stu-id="16a97-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16a97-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16a97-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16a97-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16a97-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="16a97-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="16a97-139">Response</span></span>
<span data-ttu-id="16a97-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="16a97-140">The following is an example of the response.</span></span>
><span data-ttu-id="16a97-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16a97-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
