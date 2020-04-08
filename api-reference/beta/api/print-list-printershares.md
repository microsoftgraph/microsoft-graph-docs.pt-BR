---
title: Obter printerShares
description: Recupere uma lista de compartilhamentos de impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 02fc83e45a19165a23600c9c03bc94e74ff9f493
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2020
ms.locfileid: "42948282"
---
# <a name="list-printershares"></a><span data-ttu-id="2fc88-103">Listar printerShares</span><span class="sxs-lookup"><span data-stu-id="2fc88-103">List printerShares</span></span>

<span data-ttu-id="2fc88-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fc88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fc88-105">Recupere uma lista de **printerShares**.</span><span class="sxs-lookup"><span data-stu-id="2fc88-105">Retrieve a list of **printerShares**.</span></span>

## <a name="permissions"></a><span data-ttu-id="2fc88-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2fc88-106">Permissions</span></span>
<span data-ttu-id="2fc88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fc88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2fc88-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="2fc88-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="2fc88-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2fc88-110">Permission type</span></span> | <span data-ttu-id="2fc88-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2fc88-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="2fc88-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2fc88-112">Delegated (work or school account)</span></span>| <span data-ttu-id="2fc88-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="2fc88-113">Users.Read.All</span></span> |
|<span data-ttu-id="2fc88-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2fc88-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2fc88-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fc88-115">Not Supported.</span></span>|
|<span data-ttu-id="2fc88-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2fc88-116">Application</span></span>|<span data-ttu-id="2fc88-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fc88-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2fc88-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2fc88-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printerShares
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2fc88-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2fc88-119">Optional query parameters</span></span>
<span data-ttu-id="2fc88-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2fc88-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2fc88-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2fc88-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="2fc88-122">Exceções</span><span class="sxs-lookup"><span data-stu-id="2fc88-122">Exceptions</span></span>

* <span data-ttu-id="2fc88-123">Não `$count` há suporte para o operador.</span><span class="sxs-lookup"><span data-stu-id="2fc88-123">The `$count` operator is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2fc88-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2fc88-124">Request headers</span></span>
| <span data-ttu-id="2fc88-125">Nome</span><span class="sxs-lookup"><span data-stu-id="2fc88-125">Name</span></span>      |<span data-ttu-id="2fc88-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fc88-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2fc88-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="2fc88-127">Authorization</span></span> | <span data-ttu-id="2fc88-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2fc88-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2fc88-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2fc88-130">Request body</span></span>
<span data-ttu-id="2fc88-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2fc88-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2fc88-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fc88-132">Response</span></span>
<span data-ttu-id="2fc88-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [printerShare](../resources/printershare.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fc88-133">If successful, this method returns a `200 OK` response code and a collection of [printerShare](../resources/printershare.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2fc88-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2fc88-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2fc88-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2fc88-135">Request</span></span>
<span data-ttu-id="2fc88-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2fc88-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2fc88-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="2fc88-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printershares"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printerShares
```
# <a name="c"></a>[<span data-ttu-id="2fc88-138">C#</span><span class="sxs-lookup"><span data-stu-id="2fc88-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printershares-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2fc88-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2fc88-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printershares-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2fc88-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2fc88-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printershares-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2fc88-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fc88-141">Response</span></span>
<span data-ttu-id="2fc88-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2fc88-142">The following is an example of the response.</span></span>
><span data-ttu-id="2fc88-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2fc88-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 269

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printerShares",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "name": "PrinterShareName",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List printerShares",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
