---
title: 'Range: UsedRange'
description: Retorna o intervalo usado do objeto range determinado.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 77ea975e615a527fa173870a45740a9d041b5715
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510568"
---
# <a name="range-usedrange"></a><span data-ttu-id="e34c6-103">Range: UsedRange</span><span class="sxs-lookup"><span data-stu-id="e34c6-103">Range: UsedRange</span></span>

<span data-ttu-id="e34c6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e34c6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e34c6-105">Retorna o intervalo usado do objeto range determinado.</span><span class="sxs-lookup"><span data-stu-id="e34c6-105">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e34c6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e34c6-106">Permissions</span></span>
<span data-ttu-id="e34c6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e34c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e34c6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e34c6-109">Permission type</span></span>      | <span data-ttu-id="e34c6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e34c6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e34c6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e34c6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e34c6-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e34c6-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e34c6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e34c6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e34c6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e34c6-114">Not supported.</span></span>    |
|<span data-ttu-id="e34c6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e34c6-115">Application</span></span> | <span data-ttu-id="e34c6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e34c6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e34c6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e34c6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/usedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/usedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/usedRange

```
## <a name="request-headers"></a><span data-ttu-id="e34c6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e34c6-118">Request headers</span></span>
| <span data-ttu-id="e34c6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e34c6-119">Name</span></span>       | <span data-ttu-id="e34c6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e34c6-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e34c6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e34c6-121">Authorization</span></span>  | <span data-ttu-id="e34c6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e34c6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e34c6-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e34c6-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="e34c6-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e34c6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="e34c6-127">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="e34c6-127">Path parameters</span></span>
| <span data-ttu-id="e34c6-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e34c6-128">Parameter</span></span>    | <span data-ttu-id="e34c6-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e34c6-129">Type</span></span>   |<span data-ttu-id="e34c6-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e34c6-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e34c6-131">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="e34c6-131">valuesOnly</span></span>|<span data-ttu-id="e34c6-132">booliano</span><span class="sxs-lookup"><span data-stu-id="e34c6-132">boolean</span></span>|<span data-ttu-id="e34c6-p104">Opcional. Considera apenas as células com valores como células usadas.</span><span class="sxs-lookup"><span data-stu-id="e34c6-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="e34c6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e34c6-135">Response</span></span>

<span data-ttu-id="e34c6-136">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e34c6-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e34c6-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e34c6-137">Example</span></span>
<span data-ttu-id="e34c6-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e34c6-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e34c6-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e34c6-139">Request</span></span>
<span data-ttu-id="e34c6-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e34c6-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e34c6-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="e34c6-141">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange
```
# <a name="c"></a>[<span data-ttu-id="e34c6-142">C#</span><span class="sxs-lookup"><span data-stu-id="e34c6-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e34c6-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e34c6-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e34c6-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e34c6-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e34c6-145">Java</span><span class="sxs-lookup"><span data-stu-id="e34c6-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-usedrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e34c6-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="e34c6-146">Response</span></span>
<span data-ttu-id="e34c6-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e34c6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="e34c6-150">Veja um exemplo que especifica o parâmetro `valuesOnly` opcional.</span><span class="sxs-lookup"><span data-stu-id="e34c6-150">Here is an example specifying the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="e34c6-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e34c6-151">Request</span></span>
<span data-ttu-id="e34c6-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e34c6-152">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e34c6-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="e34c6-153">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange_valuesonly"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange(valuesOnly=true)
```
# <a name="c"></a>[<span data-ttu-id="e34c6-154">C#</span><span class="sxs-lookup"><span data-stu-id="e34c6-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-usedrange-valuesonly-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e34c6-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e34c6-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-usedrange-valuesonly-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e34c6-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e34c6-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-usedrange-valuesonly-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e34c6-157">Java</span><span class="sxs-lookup"><span data-stu-id="e34c6-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-usedrange-valuesonly-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e34c6-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="e34c6-158">Response</span></span>

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
  "cellCount": 90,
  "columnCount": 90,
  "columnIndex": 90,
  "valueTypes": "valueTypes-value"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
