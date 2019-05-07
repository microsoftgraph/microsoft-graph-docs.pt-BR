---
title: 'WorksheetProtection: protect'
description: Protege uma planilha. Gera uma exceção se a planilha estiver protegida.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2584cce4bae3f7289ea25900c00a8c5585016ac9
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33601217"
---
# <a name="worksheetprotection-protect"></a><span data-ttu-id="1848d-104">WorksheetProtection: protect</span><span class="sxs-lookup"><span data-stu-id="1848d-104">WorksheetProtection: protect</span></span>

<span data-ttu-id="1848d-105">Protege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="1848d-105">Protect a worksheet.</span></span> <span data-ttu-id="1848d-106">Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="1848d-106">It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="1848d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1848d-107">Permissions</span></span>
<span data-ttu-id="1848d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1848d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1848d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1848d-110">Permission type</span></span>      | <span data-ttu-id="1848d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1848d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1848d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1848d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1848d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1848d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1848d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1848d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1848d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1848d-115">Not supported.</span></span>    |
|<span data-ttu-id="1848d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1848d-116">Application</span></span> | <span data-ttu-id="1848d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1848d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1848d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1848d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="1848d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1848d-119">Request headers</span></span>
| <span data-ttu-id="1848d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1848d-120">Name</span></span>       | <span data-ttu-id="1848d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1848d-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1848d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1848d-122">Authorization</span></span>  | <span data-ttu-id="1848d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1848d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1848d-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1848d-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="1848d-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="1848d-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1848d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1848d-128">Request body</span></span>
<span data-ttu-id="1848d-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1848d-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1848d-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1848d-130">Parameter</span></span>    | <span data-ttu-id="1848d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1848d-131">Type</span></span>   |<span data-ttu-id="1848d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1848d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1848d-133">options</span><span class="sxs-lookup"><span data-stu-id="1848d-133">options</span></span>|<span data-ttu-id="1848d-134">WorkbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="1848d-134">WorkbookWorksheetProtectionOptions</span></span>|<span data-ttu-id="1848d-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1848d-135">Optional.</span></span> <span data-ttu-id="1848d-136">Opções de proteção da planilha.</span><span class="sxs-lookup"><span data-stu-id="1848d-136">sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="1848d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1848d-137">Response</span></span>

<span data-ttu-id="1848d-p107">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1848d-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1848d-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1848d-140">Example</span></span>
<span data-ttu-id="1848d-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="1848d-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1848d-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1848d-142">Request</span></span>
<span data-ttu-id="1848d-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1848d-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_protect"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/protect
Content-type: application/json
Content-length: 383

{
  "options": {
    "allowFormatCells": true,
    "allowFormatColumns": true,
    "allowFormatRows": true,
    "allowInsertColumns": true,
    "allowInsertRows": true,
    "allowInsertHyperlinks": true,
    "allowDeleteColumns": true,
    "allowDeleteRows": true,
    "allowSort": true,
    "allowAutoFilter": true,
    "allowPivotTables": true
  }
}
```

##### <a name="response"></a><span data-ttu-id="1848d-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="1848d-144">Response</span></span>
<span data-ttu-id="1848d-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1848d-145">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1848d-146">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="1848d-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1848d-147">Basic</span><span class="sxs-lookup"><span data-stu-id="1848d-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/worksheetprotection_protect-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1848d-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1848d-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/worksheetprotection_protect-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/worksheetprotection-protect.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/worksheetprotection-protect.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
