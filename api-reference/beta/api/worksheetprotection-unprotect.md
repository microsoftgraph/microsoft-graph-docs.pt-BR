---
title: 'workbookWorksheetProtection: desproteger'
description: Desprotege uma planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c1556a164a4da6bf46753605904556c50ea63d2e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269283"
---
# <a name="workbookworksheetprotection-unprotect"></a><span data-ttu-id="7c462-103">workbookWorksheetProtection: desproteger</span><span class="sxs-lookup"><span data-stu-id="7c462-103">workbookWorksheetProtection: unprotect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c462-104">Desprotege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="7c462-104">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="7c462-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7c462-105">Permissions</span></span>
<span data-ttu-id="7c462-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c462-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c462-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c462-108">Permission type</span></span>      | <span data-ttu-id="7c462-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7c462-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c462-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c462-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7c462-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c462-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7c462-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c462-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c462-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c462-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7c462-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c462-114">Application</span></span> | <span data-ttu-id="7c462-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c462-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c462-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c462-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="7c462-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c462-117">Request headers</span></span>
| <span data-ttu-id="7c462-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7c462-118">Name</span></span>       | <span data-ttu-id="7c462-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c462-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7c462-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c462-120">Authorization</span></span>  | <span data-ttu-id="7c462-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c462-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7c462-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7c462-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7c462-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="7c462-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c462-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c462-126">Request body</span></span>
<span data-ttu-id="7c462-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c462-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7c462-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7c462-128">Parameter</span></span>    | <span data-ttu-id="7c462-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c462-129">Type</span></span>   |<span data-ttu-id="7c462-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c462-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c462-131">password</span><span class="sxs-lookup"><span data-stu-id="7c462-131">password</span></span>|<span data-ttu-id="7c462-132">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c462-132">string</span></span>|<span data-ttu-id="7c462-p104">Opcional. Senha de proteção para a planilha.</span><span class="sxs-lookup"><span data-stu-id="7c462-p104">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="7c462-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c462-135">Response</span></span>

<span data-ttu-id="7c462-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c462-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c462-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c462-138">Example</span></span>
<span data-ttu-id="7c462-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7c462-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7c462-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c462-140">Request</span></span>
<span data-ttu-id="7c462-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c462-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookworksheetprotection_unprotect"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
Content-type: application/json
Content-length: 34

{
  "password": "password-value"
}
```

##### <a name="response"></a><span data-ttu-id="7c462-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c462-142">Response</span></span>
<span data-ttu-id="7c462-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c462-143">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7c462-144">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="7c462-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7c462-145">C#</span><span class="sxs-lookup"><span data-stu-id="7c462-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookworksheetprotection_unprotect-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7c462-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="7c462-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/workbookworksheetprotection_unprotect-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7c462-147">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7c462-147">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/workbookworksheetprotection_unprotect-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookWorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheetprotection-unprotect.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/worksheetprotection-unprotect.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/worksheetprotection-unprotect.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
