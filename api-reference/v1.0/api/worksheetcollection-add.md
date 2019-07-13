---
title: 'WorksheetCollection: add'
description: . Activate () nele.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3bd363a48c3e99133246b1ab46c0d7fcb4d8aa1b
ms.sourcegitcommit: ca55fc5f5711966eaa41da31cd1ae99820e9e586
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2019
ms.locfileid: "35645258"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="7fde3-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="7fde3-103">WorksheetCollection: add</span></span>

<span data-ttu-id="7fde3-104">Adiciona uma nova planilha à pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="7fde3-104">Adds a new worksheet to the workbook.</span></span> <span data-ttu-id="7fde3-105">A planilha será adicionada ao final das planilhas existentes.</span><span class="sxs-lookup"><span data-stu-id="7fde3-105">The worksheet will be added at the end of existing worksheets.</span></span> <span data-ttu-id="7fde3-106">Se você deseja ativar a planilha recém-adicionada, chame. Activate () nele.</span><span class="sxs-lookup"><span data-stu-id="7fde3-106">If you wish to activate the newly added worksheet, call .activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="7fde3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7fde3-107">Permissions</span></span>
<span data-ttu-id="7fde3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fde3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fde3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7fde3-110">Permission type</span></span>      | <span data-ttu-id="7fde3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7fde3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7fde3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7fde3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7fde3-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7fde3-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7fde3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7fde3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fde3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fde3-115">Not supported.</span></span>    |
|<span data-ttu-id="7fde3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fde3-116">Application</span></span> | <span data-ttu-id="7fde3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fde3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fde3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7fde3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="7fde3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7fde3-119">Request headers</span></span>
| <span data-ttu-id="7fde3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7fde3-120">Name</span></span>       | <span data-ttu-id="7fde3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7fde3-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7fde3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7fde3-122">Authorization</span></span>  | <span data-ttu-id="7fde3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7fde3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7fde3-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7fde3-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="7fde3-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="7fde3-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fde3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7fde3-128">Request body</span></span>
<span data-ttu-id="7fde3-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7fde3-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7fde3-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7fde3-130">Parameter</span></span>    | <span data-ttu-id="7fde3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7fde3-131">Type</span></span>   |<span data-ttu-id="7fde3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7fde3-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7fde3-133">name</span><span class="sxs-lookup"><span data-stu-id="7fde3-133">name</span></span>|<span data-ttu-id="7fde3-134">string</span><span class="sxs-lookup"><span data-stu-id="7fde3-134">string</span></span>|<span data-ttu-id="7fde3-p105">Opcional. O nome da planilha a ser adicionada. Se especificado, o nome deve ser exclusivo. Se não especificado, o Excel determina o nome da nova planilha.</span><span class="sxs-lookup"><span data-stu-id="7fde3-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="7fde3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fde3-139">Response</span></span>

<span data-ttu-id="7fde3-140">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [WorkbookWorksheet](../resources/worksheet.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7fde3-140">If successful, this method returns `200 OK` response code and [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fde3-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7fde3-141">Example</span></span>
<span data-ttu-id="7fde3-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7fde3-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7fde3-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fde3-143">Request</span></span>
<span data-ttu-id="7fde3-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7fde3-144">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7fde3-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="7fde3-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheetcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/add
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7fde3-146">C#</span><span class="sxs-lookup"><span data-stu-id="7fde3-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheetcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7fde3-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="7fde3-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheetcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7fde3-148">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7fde3-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheetcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7fde3-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fde3-149">Response</span></span>
<span data-ttu-id="7fde3-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7fde3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "WorksheetCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
