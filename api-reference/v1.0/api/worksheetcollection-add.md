---
title: 'WorksheetCollection: add'
description: . Activate () nele.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 78bba9db604501406a3dc0f9028dadaa36a60f5a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278257"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="7eb09-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="7eb09-103">WorksheetCollection: add</span></span>

<span data-ttu-id="7eb09-p101">Adiciona uma nova planilha à pasta de trabalho. A planilha será adicionada ao final das planilhas existentes. Se você quiser ativar a planilha recém-adicionada, chame “.activate()” nela.</span><span class="sxs-lookup"><span data-stu-id="7eb09-p101">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="7eb09-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7eb09-107">Permissions</span></span>
<span data-ttu-id="7eb09-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7eb09-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7eb09-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7eb09-110">Permission type</span></span>      | <span data-ttu-id="7eb09-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7eb09-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7eb09-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7eb09-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7eb09-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7eb09-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7eb09-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7eb09-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7eb09-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7eb09-115">Not supported.</span></span>    |
|<span data-ttu-id="7eb09-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7eb09-116">Application</span></span> | <span data-ttu-id="7eb09-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7eb09-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7eb09-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7eb09-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="7eb09-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7eb09-119">Request headers</span></span>
| <span data-ttu-id="7eb09-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7eb09-120">Name</span></span>       | <span data-ttu-id="7eb09-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7eb09-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7eb09-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7eb09-122">Authorization</span></span>  | <span data-ttu-id="7eb09-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7eb09-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7eb09-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7eb09-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="7eb09-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="7eb09-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7eb09-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7eb09-128">Request body</span></span>
<span data-ttu-id="7eb09-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7eb09-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7eb09-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7eb09-130">Parameter</span></span>    | <span data-ttu-id="7eb09-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7eb09-131">Type</span></span>   |<span data-ttu-id="7eb09-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7eb09-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7eb09-133">name</span><span class="sxs-lookup"><span data-stu-id="7eb09-133">name</span></span>|<span data-ttu-id="7eb09-134">string</span><span class="sxs-lookup"><span data-stu-id="7eb09-134">string</span></span>|<span data-ttu-id="7eb09-p105">Opcional. O nome da planilha a ser adicionada. Se especificado, o nome deve ser exclusivo. Se não especificado, o Excel determina o nome da nova planilha.</span><span class="sxs-lookup"><span data-stu-id="7eb09-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="7eb09-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7eb09-139">Response</span></span>

<span data-ttu-id="7eb09-140">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [WorkbookWorksheet](../resources/worksheet.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7eb09-140">If successful, this method returns `200 OK` response code and [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7eb09-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7eb09-141">Example</span></span>
<span data-ttu-id="7eb09-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7eb09-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7eb09-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7eb09-143">Request</span></span>
<span data-ttu-id="7eb09-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7eb09-144">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="7eb09-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="7eb09-145">Response</span></span>
<span data-ttu-id="7eb09-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7eb09-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7eb09-149">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="7eb09-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7eb09-150">C#</span><span class="sxs-lookup"><span data-stu-id="7eb09-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/worksheetcollection_add-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7eb09-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="7eb09-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/worksheetcollection_add-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7eb09-152">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7eb09-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/worksheetcollection_add-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/worksheetcollection-add.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/worksheetcollection-add.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/worksheetcollection-add.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
