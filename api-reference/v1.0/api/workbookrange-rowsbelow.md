---
title: 'workbookRange: rowsBelow'
description: Obtém um determinado número de linhas abaixo de um determinado intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 714743d68d31439afaa8aa648dfdf0f305f758ae
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575495"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="535f5-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="535f5-103">workbookRange: rowsBelow</span></span>

<span data-ttu-id="535f5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="535f5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="535f5-105">Obtém um determinado número de linhas abaixo de um determinado intervalo.</span><span class="sxs-lookup"><span data-stu-id="535f5-105">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="535f5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="535f5-106">Permissions</span></span>
<span data-ttu-id="535f5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="535f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="535f5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="535f5-109">Permission type</span></span>      | <span data-ttu-id="535f5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="535f5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="535f5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="535f5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="535f5-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="535f5-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="535f5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="535f5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="535f5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="535f5-114">Not supported.</span></span>    |
|<span data-ttu-id="535f5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="535f5-115">Application</span></span> | <span data-ttu-id="535f5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="535f5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="535f5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="535f5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id}/range/rowsBelow(count=n)
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="535f5-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="535f5-118">Function parameters</span></span>

| <span data-ttu-id="535f5-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="535f5-119">Parameter</span></span>    | <span data-ttu-id="535f5-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="535f5-120">Type</span></span>   |<span data-ttu-id="535f5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="535f5-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="535f5-122">Count</span><span class="sxs-lookup"><span data-stu-id="535f5-122">count</span></span>|<span data-ttu-id="535f5-123">Int32</span><span class="sxs-lookup"><span data-stu-id="535f5-123">Int32</span></span>| <span data-ttu-id="535f5-p102">Opcional. O número de linhas a serem incluídas no intervalo resultante. Em geral, use um número positivo para criar um intervalo fora do intervalo atual. Você também pode usar um número negativo para criar um intervalo dentro do intervalo atual. O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="535f5-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="535f5-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="535f5-129">Request headers</span></span>
| <span data-ttu-id="535f5-130">Nome</span><span class="sxs-lookup"><span data-stu-id="535f5-130">Name</span></span>       | <span data-ttu-id="535f5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="535f5-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="535f5-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="535f5-132">Authorization</span></span>  | <span data-ttu-id="535f5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="535f5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="535f5-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="535f5-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="535f5-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="535f5-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="535f5-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="535f5-138">Request body</span></span>
<span data-ttu-id="535f5-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="535f5-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="535f5-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="535f5-140">Response</span></span>
<span data-ttu-id="535f5-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="535f5-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="535f5-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="535f5-142">Example</span></span>
<span data-ttu-id="535f5-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="535f5-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="535f5-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="535f5-144">Request</span></span>
<span data-ttu-id="535f5-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="535f5-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="535f5-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="535f5-146">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow",
  "idempotent": true
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```
# <a name="c"></a>[<span data-ttu-id="535f5-147">C#</span><span class="sxs-lookup"><span data-stu-id="535f5-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-rowsbelow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="535f5-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="535f5-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-rowsbelow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="535f5-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="535f5-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-rowsbelow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="535f5-150">Java</span><span class="sxs-lookup"><span data-stu-id="535f5-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-rowsbelow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="535f5-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="535f5-151">Response</span></span>
<span data-ttu-id="535f5-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="535f5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```

<span data-ttu-id="535f5-155">Se chamada sem `count` o parâmetro, essa função é padrão para uma linha.</span><span class="sxs-lookup"><span data-stu-id="535f5-155">If called without the `count` parameter, this function defaults to one row.</span></span>

##### <a name="request"></a><span data-ttu-id="535f5-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="535f5-156">Request</span></span>
<span data-ttu-id="535f5-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="535f5-157">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="535f5-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="535f5-158">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow_nocount",
  "idempotent": true
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow
```
# <a name="c"></a>[<span data-ttu-id="535f5-159">C#</span><span class="sxs-lookup"><span data-stu-id="535f5-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-rowsbelow-nocount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="535f5-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="535f5-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-rowsbelow-nocount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="535f5-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="535f5-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-rowsbelow-nocount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="535f5-162">Java</span><span class="sxs-lookup"><span data-stu-id="535f5-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-rowsbelow-nocount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="535f5-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="535f5-163">Response</span></span>
<span data-ttu-id="535f5-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="535f5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

