---
title: 'WorksheetCollection: add'
description: . Activate () nele.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: deef2c869445db92a145518fc5c2297da722daad
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987212"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="23ee5-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="23ee5-103">WorksheetCollection: add</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23ee5-p101">Adiciona uma nova planilha à pasta de trabalho. A planilha será adicionada ao final das planilhas existentes. Se você quiser ativar a planilha recém-adicionada, chame “.activate()” nela.</span><span class="sxs-lookup"><span data-stu-id="23ee5-p101">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="23ee5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="23ee5-107">Permissions</span></span>
<span data-ttu-id="23ee5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23ee5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23ee5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23ee5-110">Permission type</span></span>      | <span data-ttu-id="23ee5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23ee5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23ee5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23ee5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="23ee5-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23ee5-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="23ee5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23ee5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23ee5-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23ee5-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="23ee5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23ee5-116">Application</span></span> | <span data-ttu-id="23ee5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23ee5-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="23ee5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23ee5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="23ee5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23ee5-119">Request headers</span></span>
| <span data-ttu-id="23ee5-120">Nome</span><span class="sxs-lookup"><span data-stu-id="23ee5-120">Name</span></span>       | <span data-ttu-id="23ee5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="23ee5-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="23ee5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="23ee5-122">Authorization</span></span>  | <span data-ttu-id="23ee5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23ee5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="23ee5-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="23ee5-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="23ee5-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="23ee5-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="23ee5-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23ee5-128">Request body</span></span>
<span data-ttu-id="23ee5-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="23ee5-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="23ee5-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="23ee5-130">Parameter</span></span>    | <span data-ttu-id="23ee5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="23ee5-131">Type</span></span>   |<span data-ttu-id="23ee5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="23ee5-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23ee5-133">name</span><span class="sxs-lookup"><span data-stu-id="23ee5-133">name</span></span>|<span data-ttu-id="23ee5-134">string</span><span class="sxs-lookup"><span data-stu-id="23ee5-134">string</span></span>|<span data-ttu-id="23ee5-p105">Opcional. O nome da planilha a ser adicionada. Se especificado, o nome deve ser exclusivo. Se não especificado, o Excel determina o nome da nova planilha.</span><span class="sxs-lookup"><span data-stu-id="23ee5-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="23ee5-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="23ee5-139">Response</span></span>

<span data-ttu-id="23ee5-140">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [workbookWorksheet](../resources/workbookworksheet.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23ee5-140">If successful, this method returns `200 OK` response code and [workbookWorksheet](../resources/workbookworksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23ee5-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23ee5-141">Example</span></span>
<span data-ttu-id="23ee5-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="23ee5-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="23ee5-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23ee5-143">Request</span></span>
<span data-ttu-id="23ee5-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="23ee5-144">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="23ee5-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="23ee5-145">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="23ee5-146">C#</span><span class="sxs-lookup"><span data-stu-id="23ee5-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheetcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="23ee5-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="23ee5-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheetcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="23ee5-148">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="23ee5-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheetcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="23ee5-149">Java</span><span class="sxs-lookup"><span data-stu-id="23ee5-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheetcollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="23ee5-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="23ee5-150">Response</span></span>
<span data-ttu-id="23ee5-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="23ee5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
