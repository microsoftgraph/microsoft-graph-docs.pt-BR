---
title: 'NamedItem: Range'
description: Retorna o objeto Range associado ao nome. Gera uma exceção quando o tipo de item nomeado não é um intervalo.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ruoyingl
ms.openlocfilehash: 362fc951603ffbd3dc6f6ec2283ec92fef4b1443
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052114"
---
# <a name="nameditem-range"></a><span data-ttu-id="2359c-104">NamedItem: Range</span><span class="sxs-lookup"><span data-stu-id="2359c-104">NamedItem: Range</span></span>

<span data-ttu-id="2359c-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2359c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2359c-p102">Retorna o objeto Range associado ao nome. Gera uma exceção quando o tipo de item nomeado não é um intervalo.</span><span class="sxs-lookup"><span data-stu-id="2359c-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>
## <a name="permissions"></a><span data-ttu-id="2359c-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="2359c-108">Permissions</span></span>
<span data-ttu-id="2359c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2359c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2359c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2359c-111">Permission type</span></span>      | <span data-ttu-id="2359c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2359c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2359c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2359c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2359c-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2359c-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2359c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2359c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2359c-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2359c-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2359c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2359c-117">Application</span></span> | <span data-ttu-id="2359c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2359c-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2359c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2359c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/Range
GET /me/drive/root:/{item-path}:/workbook/names/{name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="2359c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2359c-120">Request headers</span></span>
| <span data-ttu-id="2359c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2359c-121">Name</span></span>       | <span data-ttu-id="2359c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2359c-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2359c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2359c-123">Authorization</span></span>  | <span data-ttu-id="2359c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2359c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2359c-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2359c-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="2359c-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="2359c-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2359c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2359c-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="2359c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2359c-130">Response</span></span>

<span data-ttu-id="2359c-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2359c-131">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2359c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2359c-132">Example</span></span>
<span data-ttu-id="2359c-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2359c-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2359c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2359c-134">Request</span></span>
<span data-ttu-id="2359c-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2359c-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2359c-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2359c-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "nameditem_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/Range
```
# <a name="c"></a>[<span data-ttu-id="2359c-137">C#</span><span class="sxs-lookup"><span data-stu-id="2359c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditem-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2359c-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2359c-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditem-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2359c-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2359c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditem-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2359c-140">Java</span><span class="sxs-lookup"><span data-stu-id="2359c-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/nameditem-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2359c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2359c-141">Response</span></span>
<span data-ttu-id="2359c-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2359c-142">Here is an example of the response.</span></span> <span data-ttu-id="2359c-143">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2359c-143">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "NamedItem: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


