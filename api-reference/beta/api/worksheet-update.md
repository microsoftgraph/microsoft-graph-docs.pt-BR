---
title: Atualizar planilha
description: Atualize as propriedades do objeto de planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 38d8b9e86bb075729756e224e146c3fb932f1018
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050693"
---
# <a name="update-worksheet"></a><span data-ttu-id="111ad-103">Atualizar planilha</span><span class="sxs-lookup"><span data-stu-id="111ad-103">Update worksheet</span></span>

<span data-ttu-id="111ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="111ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="111ad-105">Atualize as propriedades do objeto de planilha.</span><span class="sxs-lookup"><span data-stu-id="111ad-105">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="111ad-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="111ad-106">Permissions</span></span>
<span data-ttu-id="111ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="111ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="111ad-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="111ad-109">Permission type</span></span>      | <span data-ttu-id="111ad-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="111ad-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="111ad-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="111ad-111">Delegated (work or school account)</span></span> | <span data-ttu-id="111ad-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="111ad-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="111ad-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="111ad-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="111ad-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="111ad-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="111ad-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="111ad-115">Application</span></span> | <span data-ttu-id="111ad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="111ad-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="111ad-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="111ad-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="111ad-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="111ad-118">Optional request headers</span></span>
| <span data-ttu-id="111ad-119">Nome</span><span class="sxs-lookup"><span data-stu-id="111ad-119">Name</span></span>       | <span data-ttu-id="111ad-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="111ad-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="111ad-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="111ad-121">Authorization</span></span>  | <span data-ttu-id="111ad-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="111ad-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="111ad-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="111ad-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="111ad-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="111ad-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="111ad-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="111ad-127">Request body</span></span>
<span data-ttu-id="111ad-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="111ad-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="111ad-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="111ad-131">Property</span></span>     | <span data-ttu-id="111ad-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="111ad-132">Type</span></span>   |<span data-ttu-id="111ad-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="111ad-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="111ad-134">nome</span><span class="sxs-lookup"><span data-stu-id="111ad-134">name</span></span>|<span data-ttu-id="111ad-135">string</span><span class="sxs-lookup"><span data-stu-id="111ad-135">string</span></span>|<span data-ttu-id="111ad-136">O nome de exibição da planilha.</span><span class="sxs-lookup"><span data-stu-id="111ad-136">The display name of the worksheet.</span></span>|
|<span data-ttu-id="111ad-137">position</span><span class="sxs-lookup"><span data-stu-id="111ad-137">position</span></span>|<span data-ttu-id="111ad-138">int</span><span class="sxs-lookup"><span data-stu-id="111ad-138">int</span></span>|<span data-ttu-id="111ad-139">A posição baseada em zero da planilha na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="111ad-139">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="111ad-140">visibilidade</span><span class="sxs-lookup"><span data-stu-id="111ad-140">visibility</span></span>|<span data-ttu-id="111ad-141">string</span><span class="sxs-lookup"><span data-stu-id="111ad-141">string</span></span>|<span data-ttu-id="111ad-p105">A visibilidade da planilha. Os valores possíveis são: `Visible`, `Hidden` e `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="111ad-p105">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="111ad-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="111ad-144">Response</span></span>

<span data-ttu-id="111ad-145">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [workbookWorksheet](../resources/workbookworksheet.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="111ad-145">If successful, this method returns a `200 OK` response code and updated [workbookWorksheet](../resources/workbookworksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="111ad-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="111ad-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="111ad-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="111ad-147">Request</span></span>
<span data-ttu-id="111ad-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="111ad-148">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="111ad-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="111ad-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_worksheet"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}
Content-type: application/json
Content-length: 100

{
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```
# <a name="c"></a>[<span data-ttu-id="111ad-150">C#</span><span class="sxs-lookup"><span data-stu-id="111ad-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="111ad-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="111ad-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="111ad-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="111ad-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="111ad-153">Java</span><span class="sxs-lookup"><span data-stu-id="111ad-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-worksheet-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="111ad-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="111ad-154">Response</span></span>
<span data-ttu-id="111ad-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="111ad-155">Here is an example of the response.</span></span> <span data-ttu-id="111ad-156">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="111ad-156">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


