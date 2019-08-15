---
title: Atualizar planilha
description: Atualize as propriedades do objeto de planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f217763abb8044c78b411c8ae8256e7a7ea681bf
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420942"
---
# <a name="update-worksheet"></a><span data-ttu-id="98330-103">Atualizar planilha</span><span class="sxs-lookup"><span data-stu-id="98330-103">Update worksheet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98330-104">Atualize as propriedades do objeto de planilha.</span><span class="sxs-lookup"><span data-stu-id="98330-104">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="98330-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="98330-105">Permissions</span></span>
<span data-ttu-id="98330-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98330-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98330-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98330-108">Permission type</span></span>      | <span data-ttu-id="98330-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="98330-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98330-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98330-110">Delegated (work or school account)</span></span> | <span data-ttu-id="98330-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98330-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="98330-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98330-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98330-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98330-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="98330-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98330-114">Application</span></span> | <span data-ttu-id="98330-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98330-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="98330-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98330-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="98330-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="98330-117">Optional request headers</span></span>
| <span data-ttu-id="98330-118">Name</span><span class="sxs-lookup"><span data-stu-id="98330-118">Name</span></span>       | <span data-ttu-id="98330-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="98330-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="98330-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="98330-120">Authorization</span></span>  | <span data-ttu-id="98330-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98330-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="98330-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="98330-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="98330-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="98330-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="98330-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98330-126">Request body</span></span>
<span data-ttu-id="98330-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="98330-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="98330-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98330-130">Property</span></span>     | <span data-ttu-id="98330-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="98330-131">Type</span></span>   |<span data-ttu-id="98330-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="98330-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98330-133">name</span><span class="sxs-lookup"><span data-stu-id="98330-133">name</span></span>|<span data-ttu-id="98330-134">string</span><span class="sxs-lookup"><span data-stu-id="98330-134">string</span></span>|<span data-ttu-id="98330-135">O nome de exibição da planilha.</span><span class="sxs-lookup"><span data-stu-id="98330-135">The display name of the worksheet.</span></span>|
|<span data-ttu-id="98330-136">position</span><span class="sxs-lookup"><span data-stu-id="98330-136">position</span></span>|<span data-ttu-id="98330-137">int</span><span class="sxs-lookup"><span data-stu-id="98330-137">int</span></span>|<span data-ttu-id="98330-138">A posição baseada em zero da planilha na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="98330-138">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="98330-139">visibilidade</span><span class="sxs-lookup"><span data-stu-id="98330-139">visibility</span></span>|<span data-ttu-id="98330-140">string</span><span class="sxs-lookup"><span data-stu-id="98330-140">string</span></span>|<span data-ttu-id="98330-p105">A visibilidade da planilha. Os valores possíveis são: `Visible`, `Hidden` e `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="98330-p105">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="98330-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="98330-143">Response</span></span>

<span data-ttu-id="98330-144">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookWorksheet](../resources/workbookworksheet.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98330-144">If successful, this method returns a `200 OK` response code and updated [workbookWorksheet](../resources/workbookworksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="98330-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98330-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="98330-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98330-146">Request</span></span>
<span data-ttu-id="98330-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98330-147">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="98330-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="98330-148">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="98330-149">C#</span><span class="sxs-lookup"><span data-stu-id="98330-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="98330-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98330-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="98330-151">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="98330-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="98330-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="98330-152">Response</span></span>
<span data-ttu-id="98330-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98330-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
