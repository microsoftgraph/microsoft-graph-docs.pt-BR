---
title: Atualizar tablecolumn
description: Atualize as propriedades do objeto tablecolumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b22d8d76b9ece640cc873024c28dd1c0380ea9cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48012905"
---
# <a name="update-tablecolumn"></a><span data-ttu-id="a39f3-103">Atualizar tablecolumn</span><span class="sxs-lookup"><span data-stu-id="a39f3-103">Update tablecolumn</span></span>

<span data-ttu-id="a39f3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a39f3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a39f3-105">Atualize as propriedades do objeto tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="a39f3-105">Update the properties of tablecolumn object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a39f3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a39f3-106">Permissions</span></span>
<span data-ttu-id="a39f3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a39f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a39f3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a39f3-109">Permission type</span></span>      | <span data-ttu-id="a39f3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a39f3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a39f3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a39f3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a39f3-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a39f3-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a39f3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a39f3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a39f3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a39f3-114">Not supported.</span></span>    |
|<span data-ttu-id="a39f3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a39f3-115">Application</span></span> | <span data-ttu-id="a39f3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a39f3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a39f3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a39f3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/columns/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="a39f3-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="a39f3-118">Optional request headers</span></span>
| <span data-ttu-id="a39f3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a39f3-119">Name</span></span>       | <span data-ttu-id="a39f3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a39f3-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a39f3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a39f3-121">Authorization</span></span>  | <span data-ttu-id="a39f3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a39f3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a39f3-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a39f3-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="a39f3-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="a39f3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a39f3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a39f3-127">Request body</span></span>
<span data-ttu-id="a39f3-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="a39f3-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a39f3-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a39f3-131">Property</span></span>     | <span data-ttu-id="a39f3-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="a39f3-132">Type</span></span>   |<span data-ttu-id="a39f3-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="a39f3-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a39f3-134">values</span><span class="sxs-lookup"><span data-stu-id="a39f3-134">values</span></span>|<span data-ttu-id="a39f3-135">Json</span><span class="sxs-lookup"><span data-stu-id="a39f3-135">Json</span></span>|<span data-ttu-id="a39f3-p105">Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="a39f3-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="a39f3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a39f3-139">Response</span></span>

<span data-ttu-id="a39f3-140">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [WorkbookTableColumn](../resources/workbooktablecolumn.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a39f3-140">If successful, this method returns a `200 OK` response code and updated [WorkbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a39f3-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a39f3-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a39f3-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a39f3-142">Request</span></span>
<span data-ttu-id="a39f3-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a39f3-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a39f3-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="a39f3-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a39f3-145">C#</span><span class="sxs-lookup"><span data-stu-id="a39f3-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tablecolumn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a39f3-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a39f3-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tablecolumn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a39f3-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a39f3-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tablecolumn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a39f3-148">Java</span><span class="sxs-lookup"><span data-stu-id="a39f3-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tablecolumn-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---
> [!NOTE]
> <span data-ttu-id="a39f3-149">Se você quiser atualizar vários campos de uma coluna, torne **os valores** uma matriz de cadeia de caracteres na solicitação.</span><span class="sxs-lookup"><span data-stu-id="a39f3-149">If you want to update multiple fields of a column, make **values** a string array in the request.</span></span> <span data-ttu-id="a39f3-150">Por exemplo: `"values": [["a"], [1], [2], [3]]`.</span><span class="sxs-lookup"><span data-stu-id="a39f3-150">For example: `"values": [["a"], [1], [2], [3]]`.</span></span>

##### <a name="response"></a><span data-ttu-id="a39f3-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="a39f3-151">Response</span></span>
<span data-ttu-id="a39f3-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a39f3-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": 99,
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

