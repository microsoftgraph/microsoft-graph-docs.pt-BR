---
title: Atualizar tablecolumn
description: Atualize as propriedades do objeto tablecolumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: cea3f51c5da8a0702ecdb1abf4e6472aef5886c8
ms.sourcegitcommit: c74195b8725c3f28bb3bded43c855261590a0cec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/06/2019
ms.locfileid: "36775557"
---
# <a name="update-tablecolumn"></a><span data-ttu-id="b944c-103">Atualizar tablecolumn</span><span class="sxs-lookup"><span data-stu-id="b944c-103">Update tablecolumn</span></span>

<span data-ttu-id="b944c-104">Atualize as propriedades do objeto tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="b944c-104">Update the properties of tablecolumn object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b944c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b944c-105">Permissions</span></span>
<span data-ttu-id="b944c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b944c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b944c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b944c-108">Permission type</span></span>      | <span data-ttu-id="b944c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b944c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b944c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b944c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b944c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b944c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b944c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b944c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b944c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b944c-113">Not supported.</span></span>    |
|<span data-ttu-id="b944c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b944c-114">Application</span></span> | <span data-ttu-id="b944c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b944c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b944c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b944c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/columns/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="b944c-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="b944c-117">Optional request headers</span></span>
| <span data-ttu-id="b944c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b944c-118">Name</span></span>       | <span data-ttu-id="b944c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b944c-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b944c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b944c-120">Authorization</span></span>  | <span data-ttu-id="b944c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b944c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b944c-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b944c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b944c-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="b944c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b944c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b944c-126">Request body</span></span>
<span data-ttu-id="b944c-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b944c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b944c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b944c-130">Property</span></span>     | <span data-ttu-id="b944c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b944c-131">Type</span></span>   |<span data-ttu-id="b944c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b944c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b944c-133">values</span><span class="sxs-lookup"><span data-stu-id="b944c-133">values</span></span>|<span data-ttu-id="b944c-134">Json</span><span class="sxs-lookup"><span data-stu-id="b944c-134">Json</span></span>|<span data-ttu-id="b944c-p105">Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="b944c-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="b944c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b944c-138">Response</span></span>

<span data-ttu-id="b944c-139">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [WorkbookTableColumn](../resources/workbooktablecolumn.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b944c-139">If successful, this method returns a `200 OK` response code and updated [WorkbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b944c-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b944c-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b944c-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b944c-141">Request</span></span>
<span data-ttu-id="b944c-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b944c-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b944c-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="b944c-143">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b944c-144">C#</span><span class="sxs-lookup"><span data-stu-id="b944c-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tablecolumn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b944c-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b944c-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tablecolumn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b944c-146">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b944c-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tablecolumn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b944c-147">Java</span><span class="sxs-lookup"><span data-stu-id="b944c-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tablecolumn-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---
> [!NOTE]
> <span data-ttu-id="b944c-148">Se você quiser atualizar vários campos de uma coluna, torne **os valores** uma matriz de cadeia de caracteres na solicitação.</span><span class="sxs-lookup"><span data-stu-id="b944c-148">If you want to update multiple fields of a column, make **values** a string array in the request.</span></span> <span data-ttu-id="b944c-149">Por exemplo: `"values": [["a"], [1], [2], [3]]`.</span><span class="sxs-lookup"><span data-stu-id="b944c-149">For example: `"values": [["a"], [1], [2], [3]]`.</span></span>

##### <a name="response"></a><span data-ttu-id="b944c-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="b944c-150">Response</span></span>
<span data-ttu-id="b944c-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b944c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
