---
title: Atualizar planilha
description: Atualize as propriedades do objeto de planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a1b77656aef9bc4e0daeb90705d8394205fd4d4e
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575023"
---
# <a name="update-worksheet"></a><span data-ttu-id="17786-103">Atualizar planilha</span><span class="sxs-lookup"><span data-stu-id="17786-103">Update worksheet</span></span>

<span data-ttu-id="17786-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17786-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="17786-105">Atualize as propriedades do objeto de planilha.</span><span class="sxs-lookup"><span data-stu-id="17786-105">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="17786-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="17786-106">Permissions</span></span>
<span data-ttu-id="17786-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17786-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17786-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17786-109">Permission type</span></span>      | <span data-ttu-id="17786-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="17786-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17786-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17786-111">Delegated (work or school account)</span></span> | <span data-ttu-id="17786-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17786-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="17786-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17786-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17786-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17786-114">Not supported.</span></span>    |
|<span data-ttu-id="17786-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17786-115">Application</span></span> | <span data-ttu-id="17786-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17786-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="17786-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17786-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="17786-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="17786-118">Optional request headers</span></span>
| <span data-ttu-id="17786-119">Nome</span><span class="sxs-lookup"><span data-stu-id="17786-119">Name</span></span>       | <span data-ttu-id="17786-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="17786-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="17786-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="17786-121">Authorization</span></span>  | <span data-ttu-id="17786-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17786-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="17786-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="17786-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="17786-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="17786-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="17786-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17786-127">Request body</span></span>
<span data-ttu-id="17786-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="17786-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="17786-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17786-131">Property</span></span>     | <span data-ttu-id="17786-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="17786-132">Type</span></span>   |<span data-ttu-id="17786-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="17786-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17786-134">nome</span><span class="sxs-lookup"><span data-stu-id="17786-134">name</span></span>|<span data-ttu-id="17786-135">string</span><span class="sxs-lookup"><span data-stu-id="17786-135">string</span></span>|<span data-ttu-id="17786-136">O nome de exibição da planilha.</span><span class="sxs-lookup"><span data-stu-id="17786-136">The display name of the worksheet.</span></span>|
|<span data-ttu-id="17786-137">position</span><span class="sxs-lookup"><span data-stu-id="17786-137">position</span></span>|<span data-ttu-id="17786-138">int</span><span class="sxs-lookup"><span data-stu-id="17786-138">int</span></span>|<span data-ttu-id="17786-139">A posição baseada em zero da planilha na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="17786-139">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="17786-140">visibilidade</span><span class="sxs-lookup"><span data-stu-id="17786-140">visibility</span></span>|<span data-ttu-id="17786-141">string</span><span class="sxs-lookup"><span data-stu-id="17786-141">string</span></span>|<span data-ttu-id="17786-142">A visibilidade da planilha.</span><span class="sxs-lookup"><span data-stu-id="17786-142">The Visibility of the worksheet.</span></span> <span data-ttu-id="17786-143">Os valores possíveis são: `Visible`, `Hidden`, `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="17786-143">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="17786-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="17786-144">Response</span></span>

<span data-ttu-id="17786-145">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [WorkbookWorksheet](../resources/worksheet.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17786-145">If successful, this method returns a `200 OK` response code and updated [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="17786-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17786-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17786-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17786-147">Request</span></span>
<span data-ttu-id="17786-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17786-148">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="17786-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="17786-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="17786-150">C#</span><span class="sxs-lookup"><span data-stu-id="17786-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17786-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17786-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17786-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17786-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="17786-153">Java</span><span class="sxs-lookup"><span data-stu-id="17786-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-worksheet-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="17786-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="17786-154">Response</span></span>
<span data-ttu-id="17786-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17786-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

