---
title: Atualizar tablecolumn
description: Atualize as propriedades do objeto tablecolumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: dc69cc73bcc39dd2014ffa2d6074c8f601dd5d8d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050273"
---
# <a name="update-tablecolumn"></a><span data-ttu-id="b32cf-103">Atualizar tablecolumn</span><span class="sxs-lookup"><span data-stu-id="b32cf-103">Update tablecolumn</span></span>

<span data-ttu-id="b32cf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b32cf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b32cf-105">Atualize as propriedades do objeto tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="b32cf-105">Update the properties of tablecolumn object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b32cf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b32cf-106">Permissions</span></span>
<span data-ttu-id="b32cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b32cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b32cf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b32cf-109">Permission type</span></span>      | <span data-ttu-id="b32cf-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b32cf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b32cf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b32cf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b32cf-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b32cf-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b32cf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b32cf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b32cf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b32cf-114">Not supported.</span></span>    |
|<span data-ttu-id="b32cf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b32cf-115">Application</span></span> | <span data-ttu-id="b32cf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b32cf-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b32cf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b32cf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="b32cf-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="b32cf-118">Optional request headers</span></span>
| <span data-ttu-id="b32cf-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b32cf-119">Name</span></span>       | <span data-ttu-id="b32cf-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b32cf-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b32cf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b32cf-121">Authorization</span></span>  | <span data-ttu-id="b32cf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b32cf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b32cf-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b32cf-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="b32cf-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="b32cf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b32cf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b32cf-127">Request body</span></span>
<span data-ttu-id="b32cf-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b32cf-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b32cf-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b32cf-131">Property</span></span>     | <span data-ttu-id="b32cf-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="b32cf-132">Type</span></span>   |<span data-ttu-id="b32cf-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="b32cf-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b32cf-134">values</span><span class="sxs-lookup"><span data-stu-id="b32cf-134">values</span></span>|<span data-ttu-id="b32cf-135">Json</span><span class="sxs-lookup"><span data-stu-id="b32cf-135">Json</span></span>|<span data-ttu-id="b32cf-p105">Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="b32cf-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="b32cf-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b32cf-139">Response</span></span>

<span data-ttu-id="b32cf-140">Se tiver êxito, este método retornará um código de resposta e `200 OK` um [objeto WorkbookTableColumn](../resources/workbooktablecolumn.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b32cf-140">If successful, this method returns a `200 OK` response code and updated [WorkbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b32cf-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b32cf-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b32cf-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b32cf-142">Request</span></span>
<span data-ttu-id="b32cf-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b32cf-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b32cf-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="b32cf-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tablecolumn"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
Content-type: application/json
Content-length: 81

{
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
# <a name="c"></a>[<span data-ttu-id="b32cf-145">C#</span><span class="sxs-lookup"><span data-stu-id="b32cf-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tablecolumn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b32cf-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b32cf-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tablecolumn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b32cf-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b32cf-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tablecolumn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b32cf-148">Java</span><span class="sxs-lookup"><span data-stu-id="b32cf-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tablecolumn-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---
> [!NOTE]
> <span data-ttu-id="b32cf-149">Se você quiser atualizar vários campos de uma coluna, faça **dos valores uma** matriz de cadeia de caracteres na solicitação.</span><span class="sxs-lookup"><span data-stu-id="b32cf-149">If you want to update multiple fields of a column, make **values** a string array in the request.</span></span> <span data-ttu-id="b32cf-150">Por exemplo: `"values": [["a"], [1], [2], [3]]`.</span><span class="sxs-lookup"><span data-stu-id="b32cf-150">For example: `"values": [["a"], [1], [2], [3]]`.</span></span>

##### <a name="response"></a><span data-ttu-id="b32cf-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="b32cf-151">Response</span></span>
<span data-ttu-id="b32cf-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b32cf-152">Here is an example of the response.</span></span> <span data-ttu-id="b32cf-153">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b32cf-153">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": "99",
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tablecolumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

