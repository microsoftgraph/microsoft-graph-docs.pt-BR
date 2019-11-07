---
title: Obter workbookApplication
description: Recupere as propriedades e os relacionamentos do objeto workbookApplication.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 399cb1452bc3c1c009d4c08668b2409f6eec2f04
ms.sourcegitcommit: 2f3e7325b5bc1f0cdc12a8acdf34d31cea3b8bdb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/07/2019
ms.locfileid: "38023174"
---
# <a name="get-workbookapplication"></a><span data-ttu-id="7498a-103">Obter workbookApplication</span><span class="sxs-lookup"><span data-stu-id="7498a-103">Get workbookApplication</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7498a-104">Recupere as propriedades e os relacionamentos de um objeto [workbookApplication](../resources/workbookapplication.md) .</span><span class="sxs-lookup"><span data-stu-id="7498a-104">Retrieve the properties and relationships of a [workbookApplication](../resources/workbookapplication.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7498a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7498a-105">Permissions</span></span>
<span data-ttu-id="7498a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7498a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7498a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7498a-108">Permission type</span></span>      | <span data-ttu-id="7498a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7498a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7498a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7498a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7498a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7498a-111">Files.ReadWrite</span></span>     |
|<span data-ttu-id="7498a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7498a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7498a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7498a-113">Not supported.</span></span>    |
|<span data-ttu-id="7498a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7498a-114">Application</span></span> | <span data-ttu-id="7498a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7498a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7498a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7498a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/application
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7498a-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7498a-117">Optional query parameters</span></span>
<span data-ttu-id="7498a-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7498a-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7498a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7498a-119">Request headers</span></span>
| <span data-ttu-id="7498a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7498a-120">Name</span></span>      |<span data-ttu-id="7498a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7498a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7498a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7498a-122">Authorization</span></span>  | <span data-ttu-id="7498a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7498a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7498a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7498a-125">Request body</span></span>
<span data-ttu-id="7498a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7498a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7498a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="7498a-127">Response</span></span>

<span data-ttu-id="7498a-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [workbookApplication](../resources/workbookapplication.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7498a-128">If successful, this method returns a `200 OK` response code and a [workbookApplication](../resources/workbookapplication.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7498a-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7498a-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="7498a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7498a-130">Request</span></span>
<span data-ttu-id="7498a-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7498a-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7498a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7498a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookApplication"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7498a-133">C#</span><span class="sxs-lookup"><span data-stu-id="7498a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7498a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7498a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7498a-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7498a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="7498a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7498a-136">Response</span></span>
<span data-ttu-id="7498a-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7498a-137">Here is an example of the response.</span></span> 

><span data-ttu-id="7498a-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7498a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookApplication"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 48

{
  "calculationMode": "calculationMode-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get workbookApplication",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
