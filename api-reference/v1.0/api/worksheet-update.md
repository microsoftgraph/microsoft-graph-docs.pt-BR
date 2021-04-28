---
title: Atualizar planilha
description: Atualize as propriedades do objeto de planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 83c1e896209c59f43520448b03b293becbd2c775
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055614"
---
# <a name="update-worksheet"></a><span data-ttu-id="1c58e-103">Atualizar planilha</span><span class="sxs-lookup"><span data-stu-id="1c58e-103">Update worksheet</span></span>

<span data-ttu-id="1c58e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c58e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1c58e-105">Atualize as propriedades do objeto de planilha.</span><span class="sxs-lookup"><span data-stu-id="1c58e-105">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1c58e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c58e-106">Permissions</span></span>
<span data-ttu-id="1c58e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c58e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c58e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c58e-109">Permission type</span></span>      | <span data-ttu-id="1c58e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c58e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c58e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c58e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1c58e-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c58e-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1c58e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c58e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c58e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c58e-114">Not supported.</span></span>    |
|<span data-ttu-id="1c58e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c58e-115">Application</span></span> | <span data-ttu-id="1c58e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c58e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c58e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c58e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="1c58e-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="1c58e-118">Optional request headers</span></span>
| <span data-ttu-id="1c58e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1c58e-119">Name</span></span>       | <span data-ttu-id="1c58e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c58e-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1c58e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c58e-121">Authorization</span></span>  | <span data-ttu-id="1c58e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c58e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1c58e-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1c58e-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="1c58e-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="1c58e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c58e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c58e-127">Request body</span></span>
<span data-ttu-id="1c58e-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="1c58e-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1c58e-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c58e-131">Property</span></span>     | <span data-ttu-id="1c58e-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c58e-132">Type</span></span>   |<span data-ttu-id="1c58e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c58e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c58e-134">nome</span><span class="sxs-lookup"><span data-stu-id="1c58e-134">name</span></span>|<span data-ttu-id="1c58e-135">string</span><span class="sxs-lookup"><span data-stu-id="1c58e-135">string</span></span>|<span data-ttu-id="1c58e-136">O nome de exibição da planilha.</span><span class="sxs-lookup"><span data-stu-id="1c58e-136">The display name of the worksheet.</span></span>|
|<span data-ttu-id="1c58e-137">position</span><span class="sxs-lookup"><span data-stu-id="1c58e-137">position</span></span>|<span data-ttu-id="1c58e-138">int</span><span class="sxs-lookup"><span data-stu-id="1c58e-138">int</span></span>|<span data-ttu-id="1c58e-139">A posição baseada em zero da planilha na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1c58e-139">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="1c58e-140">visibilidade</span><span class="sxs-lookup"><span data-stu-id="1c58e-140">visibility</span></span>|<span data-ttu-id="1c58e-141">string</span><span class="sxs-lookup"><span data-stu-id="1c58e-141">string</span></span>|<span data-ttu-id="1c58e-142">A visibilidade da planilha.</span><span class="sxs-lookup"><span data-stu-id="1c58e-142">The Visibility of the worksheet.</span></span> <span data-ttu-id="1c58e-143">Os valores possíveis são: `Visible`, `Hidden`, `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="1c58e-143">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="1c58e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c58e-144">Response</span></span>

<span data-ttu-id="1c58e-145">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [WorkbookWorksheet](../resources/worksheet.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c58e-145">If successful, this method returns a `200 OK` response code and updated [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1c58e-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c58e-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c58e-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c58e-147">Request</span></span>
<span data-ttu-id="1c58e-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c58e-148">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1c58e-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c58e-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_worksheet"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}
Content-type: application/json
Content-length: 100

{
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```
# <a name="c"></a>[<span data-ttu-id="1c58e-150">C#</span><span class="sxs-lookup"><span data-stu-id="1c58e-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c58e-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c58e-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c58e-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c58e-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c58e-153">Java</span><span class="sxs-lookup"><span data-stu-id="1c58e-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-worksheet-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1c58e-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c58e-154">Response</span></span>
<span data-ttu-id="1c58e-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c58e-155">Here is an example of the response.</span></span> <span data-ttu-id="1c58e-156">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1c58e-156">Note: The response object shown here might be shortened for readability.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

