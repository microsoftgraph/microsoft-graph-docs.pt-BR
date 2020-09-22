---
title: 'Range: merge'
description: Mescla as células do intervalo em uma região da planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 58a5f86abc58cc47fcdd899edb92cda6297a4762
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051617"
---
# <a name="range-merge"></a><span data-ttu-id="b6739-103">Range: merge</span><span class="sxs-lookup"><span data-stu-id="b6739-103">Range: merge</span></span>

<span data-ttu-id="b6739-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6739-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b6739-105">Mescla as células do intervalo em uma região da planilha.</span><span class="sxs-lookup"><span data-stu-id="b6739-105">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="b6739-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6739-106">Permissions</span></span>
<span data-ttu-id="b6739-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6739-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6739-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6739-109">Permission type</span></span>      | <span data-ttu-id="b6739-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6739-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6739-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6739-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b6739-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6739-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b6739-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6739-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6739-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6739-114">Not supported.</span></span>    |
|<span data-ttu-id="b6739-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6739-115">Application</span></span> | <span data-ttu-id="b6739-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6739-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6739-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6739-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/merge
POST /workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="b6739-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6739-118">Request headers</span></span>
| <span data-ttu-id="b6739-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b6739-119">Name</span></span>       | <span data-ttu-id="b6739-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6739-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b6739-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6739-121">Authorization</span></span>  | <span data-ttu-id="b6739-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6739-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b6739-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b6739-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="b6739-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="b6739-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6739-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6739-127">Request body</span></span>
<span data-ttu-id="b6739-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6739-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b6739-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b6739-129">Parameter</span></span>    | <span data-ttu-id="b6739-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6739-130">Type</span></span>   |<span data-ttu-id="b6739-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6739-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6739-132">across</span><span class="sxs-lookup"><span data-stu-id="b6739-132">across</span></span>|<span data-ttu-id="b6739-133">booliano</span><span class="sxs-lookup"><span data-stu-id="b6739-133">boolean</span></span>|<span data-ttu-id="b6739-p104">Opcional. Defina true para mesclar células em todas as linhas do intervalo especificado como células mescladas separadamente. O valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="b6739-p104">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="b6739-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6739-137">Response</span></span>

<span data-ttu-id="b6739-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6739-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6739-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6739-140">Example</span></span>
<span data-ttu-id="b6739-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b6739-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b6739-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6739-142">Request</span></span>
<span data-ttu-id="b6739-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6739-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b6739-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6739-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```
# <a name="c"></a>[<span data-ttu-id="b6739-145">C#</span><span class="sxs-lookup"><span data-stu-id="b6739-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-merge-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6739-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6739-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-merge-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6739-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6739-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-merge-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b6739-148">Java</span><span class="sxs-lookup"><span data-stu-id="b6739-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-merge-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b6739-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6739-149">Response</span></span>
<span data-ttu-id="b6739-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6739-150">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: merge",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

