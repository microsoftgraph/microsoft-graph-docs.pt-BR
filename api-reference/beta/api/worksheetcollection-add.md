---
title: 'WorksheetCollection: add'
description: .activate() nele.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 8507fa67a0f3c6d28d25d3c8d5c5f22bc9610751
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049524"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="508ac-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="508ac-103">WorksheetCollection: add</span></span>

<span data-ttu-id="508ac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="508ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="508ac-p101">Adiciona uma nova planilha à pasta de trabalho. A planilha será adicionada ao final das planilhas existentes. Se você quiser ativar a planilha recém-adicionada, chame “.activate()” nela.</span><span class="sxs-lookup"><span data-stu-id="508ac-p101">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="508ac-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="508ac-108">Permissions</span></span>
<span data-ttu-id="508ac-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="508ac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="508ac-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="508ac-111">Permission type</span></span>      | <span data-ttu-id="508ac-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="508ac-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="508ac-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="508ac-113">Delegated (work or school account)</span></span> | <span data-ttu-id="508ac-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="508ac-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="508ac-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="508ac-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="508ac-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="508ac-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="508ac-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="508ac-117">Application</span></span> | <span data-ttu-id="508ac-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="508ac-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="508ac-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="508ac-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/
POST /me/drive/root:/{item-path}:/workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="508ac-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="508ac-120">Request headers</span></span>
| <span data-ttu-id="508ac-121">Nome</span><span class="sxs-lookup"><span data-stu-id="508ac-121">Name</span></span>       | <span data-ttu-id="508ac-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="508ac-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="508ac-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="508ac-123">Authorization</span></span>  | <span data-ttu-id="508ac-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="508ac-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="508ac-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="508ac-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="508ac-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="508ac-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="508ac-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="508ac-129">Request body</span></span>
<span data-ttu-id="508ac-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="508ac-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="508ac-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="508ac-131">Parameter</span></span>    | <span data-ttu-id="508ac-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="508ac-132">Type</span></span>   |<span data-ttu-id="508ac-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="508ac-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="508ac-134">nome</span><span class="sxs-lookup"><span data-stu-id="508ac-134">name</span></span>|<span data-ttu-id="508ac-135">string</span><span class="sxs-lookup"><span data-stu-id="508ac-135">string</span></span>|<span data-ttu-id="508ac-p105">Opcional. O nome da planilha a ser adicionada. Se especificado, o nome deve ser exclusivo. Se não especificado, o Excel determina o nome da nova planilha.</span><span class="sxs-lookup"><span data-stu-id="508ac-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="508ac-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="508ac-140">Response</span></span>

<span data-ttu-id="508ac-141">Se tiver êxito, este método retornará `200 OK` o código de resposta e o objeto [workbookWorksheet](../resources/workbookworksheet.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="508ac-141">If successful, this method returns `200 OK` response code and [workbookWorksheet](../resources/workbookworksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="508ac-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="508ac-142">Example</span></span>
<span data-ttu-id="508ac-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="508ac-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="508ac-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="508ac-144">Request</span></span>
<span data-ttu-id="508ac-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="508ac-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="508ac-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="508ac-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheetcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/add
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
# <a name="c"></a>[<span data-ttu-id="508ac-147">C#</span><span class="sxs-lookup"><span data-stu-id="508ac-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheetcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="508ac-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="508ac-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheetcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="508ac-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="508ac-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheetcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="508ac-150">Java</span><span class="sxs-lookup"><span data-stu-id="508ac-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheetcollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="508ac-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="508ac-151">Response</span></span>
<span data-ttu-id="508ac-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="508ac-152">Here is an example of the response.</span></span> <span data-ttu-id="508ac-153">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="508ac-153">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "WorksheetCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


