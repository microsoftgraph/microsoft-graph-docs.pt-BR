---
title: 'NamedItem: Range'
description: Retorna o objeto Range associado ao nome. Gera uma exceção quando o tipo de item nomeado não é um intervalo.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 8dcedaca340f87eae9ecd9dac0a242046bb6dbbf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971059"
---
# <a name="nameditem-range"></a><span data-ttu-id="7d728-104">NamedItem: Range</span><span class="sxs-lookup"><span data-stu-id="7d728-104">NamedItem: Range</span></span>

<span data-ttu-id="7d728-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d728-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7d728-p102">Retorna o objeto Range associado ao nome. Gera uma exceção quando o tipo de item nomeado não é um intervalo.</span><span class="sxs-lookup"><span data-stu-id="7d728-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>
## <a name="permissions"></a><span data-ttu-id="7d728-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="7d728-108">Permissions</span></span>
<span data-ttu-id="7d728-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d728-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d728-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d728-111">Permission type</span></span>      | <span data-ttu-id="7d728-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7d728-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d728-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d728-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7d728-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d728-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7d728-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d728-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d728-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d728-116">Not supported.</span></span>    |
|<span data-ttu-id="7d728-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d728-117">Application</span></span> | <span data-ttu-id="7d728-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d728-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d728-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d728-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range

```
## <a name="request-headers"></a><span data-ttu-id="7d728-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d728-120">Request headers</span></span>
| <span data-ttu-id="7d728-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7d728-121">Name</span></span>       | <span data-ttu-id="7d728-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d728-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7d728-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d728-123">Authorization</span></span>  | <span data-ttu-id="7d728-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d728-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7d728-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7d728-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="7d728-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="7d728-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d728-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d728-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7d728-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d728-130">Response</span></span>

<span data-ttu-id="7d728-131">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d728-131">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d728-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d728-132">Example</span></span>
<span data-ttu-id="7d728-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7d728-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7d728-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d728-134">Request</span></span>
<span data-ttu-id="7d728-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d728-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7d728-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d728-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "idempotent": true,
  "name": "nameditem_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range
```
# <a name="c"></a>[<span data-ttu-id="7d728-137">C#</span><span class="sxs-lookup"><span data-stu-id="7d728-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditem-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d728-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d728-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditem-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d728-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d728-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditem-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7d728-140">Java</span><span class="sxs-lookup"><span data-stu-id="7d728-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/nameditem-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7d728-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d728-141">Response</span></span>
<span data-ttu-id="7d728-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d728-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

