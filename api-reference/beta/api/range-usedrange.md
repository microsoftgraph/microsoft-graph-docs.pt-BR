---
title: 'Range: UsedRange'
description: Retorna o intervalo usado do objeto range determinado.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e22ca741dfd74554b4da3810eb41bffc8a487563
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578840"
---
# <a name="range-usedrange"></a><span data-ttu-id="2221e-103">Range: UsedRange</span><span class="sxs-lookup"><span data-stu-id="2221e-103">Range: UsedRange</span></span>

<span data-ttu-id="2221e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2221e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2221e-105">Retorna o intervalo usado do objeto range determinado.</span><span class="sxs-lookup"><span data-stu-id="2221e-105">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2221e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2221e-106">Permissions</span></span>
<span data-ttu-id="2221e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2221e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2221e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2221e-109">Permission type</span></span>      | <span data-ttu-id="2221e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2221e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2221e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2221e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2221e-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2221e-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2221e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2221e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2221e-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2221e-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2221e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2221e-115">Application</span></span> | <span data-ttu-id="2221e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2221e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2221e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2221e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/UsedRange
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/UsedRange
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/UsedRange
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/UsedRange
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/UsedRange
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/UsedRange

```
## <a name="request-headers"></a><span data-ttu-id="2221e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2221e-118">Request headers</span></span>
| <span data-ttu-id="2221e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2221e-119">Name</span></span>       | <span data-ttu-id="2221e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2221e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2221e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2221e-121">Authorization</span></span>  | <span data-ttu-id="2221e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2221e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2221e-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2221e-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="2221e-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="2221e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2221e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2221e-127">Request body</span></span>
<span data-ttu-id="2221e-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2221e-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2221e-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2221e-129">Parameter</span></span>    | <span data-ttu-id="2221e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2221e-130">Type</span></span>   |<span data-ttu-id="2221e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2221e-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2221e-132">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="2221e-132">valuesOnly</span></span>|<span data-ttu-id="2221e-133">booliano</span><span class="sxs-lookup"><span data-stu-id="2221e-133">boolean</span></span>|<span data-ttu-id="2221e-p104">Opcional. Considera apenas as células com valores como células usadas.</span><span class="sxs-lookup"><span data-stu-id="2221e-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="2221e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2221e-136">Response</span></span>

<span data-ttu-id="2221e-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2221e-137">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2221e-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2221e-138">Example</span></span>
<span data-ttu-id="2221e-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2221e-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2221e-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2221e-140">Request</span></span>
<span data-ttu-id="2221e-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2221e-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2221e-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="2221e-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_usedrange"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/UsedRange
Content-type: application/json
Content-length: 24

{
  "valuesOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="2221e-143">C#</span><span class="sxs-lookup"><span data-stu-id="2221e-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2221e-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2221e-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2221e-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2221e-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2221e-146">Java</span><span class="sxs-lookup"><span data-stu-id="2221e-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-usedrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2221e-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="2221e-147">Response</span></span>
<span data-ttu-id="2221e-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2221e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


