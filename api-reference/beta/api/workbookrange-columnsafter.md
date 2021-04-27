---
title: 'workbookRange: columnsAfter'
description: Obtém um determinado número de colunas à direita do intervalo especificado.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b1b42f977c2c5d85eaf6295e204d293cf6c1feea
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036055"
---
# <a name="workbookrange-columnsafter"></a><span data-ttu-id="db28c-103">workbookRange: columnsAfter</span><span class="sxs-lookup"><span data-stu-id="db28c-103">workbookRange: columnsAfter</span></span>

<span data-ttu-id="db28c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db28c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db28c-105">Obtém um determinado número de colunas à direita do intervalo especificado.</span><span class="sxs-lookup"><span data-stu-id="db28c-105">Gets a certain number of columns to the right of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="db28c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="db28c-106">Permissions</span></span>
<span data-ttu-id="db28c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db28c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db28c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db28c-109">Permission type</span></span>      | <span data-ttu-id="db28c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db28c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db28c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db28c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="db28c-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db28c-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="db28c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db28c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db28c-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db28c-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="db28c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db28c-115">Application</span></span> | <span data-ttu-id="db28c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db28c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="db28c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db28c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id}/range/columnsAfter(count=n)
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id}/range/columnsAfter(count=n)

```
## <a name="function-parameters"></a><span data-ttu-id="db28c-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="db28c-118">Function parameters</span></span>

| <span data-ttu-id="db28c-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="db28c-119">Parameter</span></span>    | <span data-ttu-id="db28c-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="db28c-120">Type</span></span>   |<span data-ttu-id="db28c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="db28c-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db28c-122">Count</span><span class="sxs-lookup"><span data-stu-id="db28c-122">count</span></span>|<span data-ttu-id="db28c-123">Int32</span><span class="sxs-lookup"><span data-stu-id="db28c-123">Int32</span></span>|<span data-ttu-id="db28c-p102">O número de colunas a serem incluídas no intervalo resultante. Em geral, use um número positivo para criar um intervalo fora do intervalo atual. Você também pode usar um número negativo para criar um intervalo dentro do intervalo atual. O valor padrão é 1</span><span class="sxs-lookup"><span data-stu-id="db28c-p102">The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1</span></span>|

## <a name="request-headers"></a><span data-ttu-id="db28c-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db28c-128">Request headers</span></span>
| <span data-ttu-id="db28c-129">Nome</span><span class="sxs-lookup"><span data-stu-id="db28c-129">Name</span></span>       | <span data-ttu-id="db28c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="db28c-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="db28c-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="db28c-131">Authorization</span></span>  | <span data-ttu-id="db28c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db28c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="db28c-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="db28c-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="db28c-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="db28c-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="db28c-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db28c-137">Request body</span></span>
<span data-ttu-id="db28c-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="db28c-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db28c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="db28c-139">Response</span></span>

<span data-ttu-id="db28c-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db28c-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db28c-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db28c-141">Example</span></span>
<span data-ttu-id="db28c-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="db28c-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="db28c-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db28c-143">Request</span></span>
<span data-ttu-id="db28c-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="db28c-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db28c-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="db28c-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrange_columnsafter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)
```
# <a name="c"></a>[<span data-ttu-id="db28c-146">C#</span><span class="sxs-lookup"><span data-stu-id="db28c-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-columnsafter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db28c-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db28c-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-columnsafter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db28c-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db28c-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-columnsafter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db28c-149">Java</span><span class="sxs-lookup"><span data-stu-id="db28c-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-columnsafter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="db28c-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="db28c-150">Response</span></span>
<span data-ttu-id="db28c-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db28c-151">Here is an example of the response.</span></span> <span data-ttu-id="db28c-152">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="db28c-152">Note: The response object shown here might be shortened for readability.</span></span>
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


