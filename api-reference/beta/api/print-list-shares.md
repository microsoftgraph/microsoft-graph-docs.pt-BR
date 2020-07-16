---
title: Obter compartilhamentos
description: Recupere uma lista de compartilhamentos de impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: f67ba775906e9b21287d48fe1e1cc8bbfbacd89d
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080643"
---
# <a name="list-shares"></a><span data-ttu-id="02e94-103">Lista de compartilhamentos</span><span class="sxs-lookup"><span data-stu-id="02e94-103">List shares</span></span>

<span data-ttu-id="02e94-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02e94-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02e94-105">Recupere uma lista de **printerShares**.</span><span class="sxs-lookup"><span data-stu-id="02e94-105">Retrieve a list of **printerShares**.</span></span>

## <a name="permissions"></a><span data-ttu-id="02e94-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="02e94-106">Permissions</span></span>
<span data-ttu-id="02e94-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02e94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="02e94-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="02e94-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="02e94-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02e94-110">Permission type</span></span> | <span data-ttu-id="02e94-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02e94-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="02e94-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02e94-112">Delegated (work or school account)</span></span>| <span data-ttu-id="02e94-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="02e94-113">Users.Read.All</span></span> |
|<span data-ttu-id="02e94-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02e94-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02e94-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02e94-115">Not Supported.</span></span>|
|<span data-ttu-id="02e94-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02e94-116">Application</span></span>|<span data-ttu-id="02e94-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02e94-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02e94-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02e94-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares
```

## <a name="optional-query-parameters"></a><span data-ttu-id="02e94-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="02e94-119">Optional query parameters</span></span>
<span data-ttu-id="02e94-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="02e94-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="02e94-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="02e94-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="02e94-122">Para ver uma lista de recursos de cada compartilhamento de impressora, inclua o `$select=capabilities` parâmetro de consulta opcional.</span><span class="sxs-lookup"><span data-stu-id="02e94-122">To see a list of each printer share's capabilities, include the optional `$select=capabilities` query parameter.</span></span>

### <a name="exceptions"></a><span data-ttu-id="02e94-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="02e94-123">Exceptions</span></span>
<span data-ttu-id="02e94-124">Não há suporte para alguns operadores: `$count` , `$orderby` , `$search` .</span><span class="sxs-lookup"><span data-stu-id="02e94-124">Some operators are not supported: `$count`, `$orderby`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02e94-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02e94-125">Request headers</span></span>
| <span data-ttu-id="02e94-126">Nome</span><span class="sxs-lookup"><span data-stu-id="02e94-126">Name</span></span>      |<span data-ttu-id="02e94-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="02e94-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="02e94-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="02e94-128">Authorization</span></span> | <span data-ttu-id="02e94-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02e94-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02e94-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02e94-131">Request body</span></span>
<span data-ttu-id="02e94-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="02e94-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="02e94-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="02e94-133">Response</span></span>
<span data-ttu-id="02e94-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [printerShare](../resources/printershare.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02e94-134">If successful, this method returns a `200 OK` response code and a collection of [printerShare](../resources/printershare.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="02e94-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02e94-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02e94-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02e94-136">Request</span></span>
<span data-ttu-id="02e94-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="02e94-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="02e94-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="02e94-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_shares"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares
```
# <a name="c"></a>[<span data-ttu-id="02e94-139">C#</span><span class="sxs-lookup"><span data-stu-id="02e94-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shares-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02e94-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02e94-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shares-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02e94-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02e94-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shares-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="02e94-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="02e94-142">Response</span></span>
<span data-ttu-id="02e94-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="02e94-143">The following is an example of the response.</span></span>
><span data-ttu-id="02e94-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02e94-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares",
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
  "description": "List shares",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
