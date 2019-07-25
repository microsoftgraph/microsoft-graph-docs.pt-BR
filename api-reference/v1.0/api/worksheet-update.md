---
title: Atualizar planilha
description: Atualize as propriedades do objeto de planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 365ec4c2b3e13fa72c0925ff35c10bc1a85b6c45
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884224"
---
# <a name="update-worksheet"></a><span data-ttu-id="225d0-103">Atualizar planilha</span><span class="sxs-lookup"><span data-stu-id="225d0-103">Update worksheet</span></span>

<span data-ttu-id="225d0-104">Atualize as propriedades do objeto de planilha.</span><span class="sxs-lookup"><span data-stu-id="225d0-104">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="225d0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="225d0-105">Permissions</span></span>
<span data-ttu-id="225d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="225d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="225d0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="225d0-108">Permission type</span></span>      | <span data-ttu-id="225d0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="225d0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="225d0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="225d0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="225d0-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="225d0-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="225d0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="225d0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="225d0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="225d0-113">Not supported.</span></span>    |
|<span data-ttu-id="225d0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="225d0-114">Application</span></span> | <span data-ttu-id="225d0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="225d0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="225d0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="225d0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="225d0-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="225d0-117">Optional request headers</span></span>
| <span data-ttu-id="225d0-118">Name</span><span class="sxs-lookup"><span data-stu-id="225d0-118">Name</span></span>       | <span data-ttu-id="225d0-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="225d0-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="225d0-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="225d0-120">Authorization</span></span>  | <span data-ttu-id="225d0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="225d0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="225d0-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="225d0-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="225d0-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="225d0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="225d0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="225d0-126">Request body</span></span>
<span data-ttu-id="225d0-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="225d0-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="225d0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="225d0-130">Property</span></span>     | <span data-ttu-id="225d0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="225d0-131">Type</span></span>   |<span data-ttu-id="225d0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="225d0-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="225d0-133">name</span><span class="sxs-lookup"><span data-stu-id="225d0-133">name</span></span>|<span data-ttu-id="225d0-134">string</span><span class="sxs-lookup"><span data-stu-id="225d0-134">string</span></span>|<span data-ttu-id="225d0-135">O nome de exibição da planilha.</span><span class="sxs-lookup"><span data-stu-id="225d0-135">The display name of the worksheet.</span></span>|
|<span data-ttu-id="225d0-136">position</span><span class="sxs-lookup"><span data-stu-id="225d0-136">position</span></span>|<span data-ttu-id="225d0-137">int</span><span class="sxs-lookup"><span data-stu-id="225d0-137">int</span></span>|<span data-ttu-id="225d0-138">A posição baseada em zero da planilha na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="225d0-138">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="225d0-139">visibilidade</span><span class="sxs-lookup"><span data-stu-id="225d0-139">visibility</span></span>|<span data-ttu-id="225d0-140">string</span><span class="sxs-lookup"><span data-stu-id="225d0-140">string</span></span>|<span data-ttu-id="225d0-141">A visibilidade da planilha.</span><span class="sxs-lookup"><span data-stu-id="225d0-141">The Visibility of the worksheet.</span></span> <span data-ttu-id="225d0-142">Os valores possíveis são: `Visible`, `Hidden`, `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="225d0-142">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="225d0-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="225d0-143">Response</span></span>

<span data-ttu-id="225d0-144">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [WorkbookWorksheet](../resources/worksheet.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="225d0-144">If successful, this method returns a `200 OK` response code and updated [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="225d0-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="225d0-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="225d0-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="225d0-146">Request</span></span>
<span data-ttu-id="225d0-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="225d0-147">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="225d0-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="225d0-148">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="225d0-149">C#</span><span class="sxs-lookup"><span data-stu-id="225d0-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="225d0-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="225d0-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="225d0-151">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="225d0-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="225d0-152">Java</span><span class="sxs-lookup"><span data-stu-id="225d0-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-worksheet-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="225d0-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="225d0-153">Response</span></span>
<span data-ttu-id="225d0-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="225d0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
