---
title: 'Range: merge'
description: Mescla as células do intervalo em uma região da planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 88cf48d357dd1efb700c2a4f768cb0c54deb0edf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510603"
---
# <a name="range-merge"></a><span data-ttu-id="6b3d2-103">Range: merge</span><span class="sxs-lookup"><span data-stu-id="6b3d2-103">Range: merge</span></span>

<span data-ttu-id="6b3d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b3d2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b3d2-105">Mescla as células do intervalo em uma região da planilha.</span><span class="sxs-lookup"><span data-stu-id="6b3d2-105">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="6b3d2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6b3d2-106">Permissions</span></span>
<span data-ttu-id="6b3d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b3d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b3d2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b3d2-109">Permission type</span></span>      | <span data-ttu-id="6b3d2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b3d2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b3d2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b3d2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6b3d2-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b3d2-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6b3d2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b3d2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b3d2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b3d2-114">Not supported.</span></span>    |
|<span data-ttu-id="6b3d2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b3d2-115">Application</span></span> | <span data-ttu-id="6b3d2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b3d2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b3d2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b3d2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/merge
POST /workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="6b3d2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b3d2-118">Request headers</span></span>
| <span data-ttu-id="6b3d2-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6b3d2-119">Name</span></span>       | <span data-ttu-id="6b3d2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b3d2-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6b3d2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b3d2-121">Authorization</span></span>  | <span data-ttu-id="6b3d2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b3d2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6b3d2-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6b3d2-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="6b3d2-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="6b3d2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b3d2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b3d2-127">Request body</span></span>
<span data-ttu-id="6b3d2-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b3d2-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6b3d2-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6b3d2-129">Parameter</span></span>    | <span data-ttu-id="6b3d2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b3d2-130">Type</span></span>   |<span data-ttu-id="6b3d2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b3d2-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b3d2-132">across</span><span class="sxs-lookup"><span data-stu-id="6b3d2-132">across</span></span>|<span data-ttu-id="6b3d2-133">booliano</span><span class="sxs-lookup"><span data-stu-id="6b3d2-133">boolean</span></span>|<span data-ttu-id="6b3d2-p104">Opcional. Defina true para mesclar células em todas as linhas do intervalo especificado como células mescladas separadamente. O valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="6b3d2-p104">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="6b3d2-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b3d2-137">Response</span></span>

<span data-ttu-id="6b3d2-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b3d2-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b3d2-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b3d2-140">Example</span></span>
<span data-ttu-id="6b3d2-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="6b3d2-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6b3d2-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b3d2-142">Request</span></span>
<span data-ttu-id="6b3d2-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b3d2-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6b3d2-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b3d2-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6b3d2-145">C#</span><span class="sxs-lookup"><span data-stu-id="6b3d2-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-merge-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b3d2-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b3d2-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-merge-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b3d2-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b3d2-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-merge-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b3d2-148">Java</span><span class="sxs-lookup"><span data-stu-id="6b3d2-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-merge-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6b3d2-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b3d2-149">Response</span></span>
<span data-ttu-id="6b3d2-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b3d2-150">Here is an example of the response.</span></span> 
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
