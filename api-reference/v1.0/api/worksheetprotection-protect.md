---
title: 'WorksheetProtection: protect'
description: Protege uma planilha. Gera uma exceção se a planilha estiver protegida.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: af6fa058063572bc8951bfbf5149123789c7f7a5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372360"
---
# <a name="worksheetprotection-protect"></a><span data-ttu-id="60aab-104">WorksheetProtection: protect</span><span class="sxs-lookup"><span data-stu-id="60aab-104">WorksheetProtection: protect</span></span>

<span data-ttu-id="60aab-105">Protege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="60aab-105">Protect a worksheet.</span></span> <span data-ttu-id="60aab-106">Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="60aab-106">It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="60aab-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="60aab-107">Permissions</span></span>
<span data-ttu-id="60aab-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60aab-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60aab-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60aab-110">Permission type</span></span>      | <span data-ttu-id="60aab-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60aab-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60aab-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60aab-112">Delegated (work or school account)</span></span> | <span data-ttu-id="60aab-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60aab-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="60aab-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60aab-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60aab-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60aab-115">Not supported.</span></span>    |
|<span data-ttu-id="60aab-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60aab-116">Application</span></span> | <span data-ttu-id="60aab-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60aab-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="60aab-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60aab-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="60aab-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60aab-119">Request headers</span></span>
| <span data-ttu-id="60aab-120">Nome</span><span class="sxs-lookup"><span data-stu-id="60aab-120">Name</span></span>       | <span data-ttu-id="60aab-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="60aab-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="60aab-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="60aab-122">Authorization</span></span>  | <span data-ttu-id="60aab-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60aab-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="60aab-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="60aab-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="60aab-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="60aab-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="60aab-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60aab-128">Request body</span></span>
<span data-ttu-id="60aab-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60aab-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="60aab-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="60aab-130">Parameter</span></span>    | <span data-ttu-id="60aab-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="60aab-131">Type</span></span>   |<span data-ttu-id="60aab-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="60aab-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60aab-133">options</span><span class="sxs-lookup"><span data-stu-id="60aab-133">options</span></span>|<span data-ttu-id="60aab-134">WorkbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="60aab-134">WorkbookWorksheetProtectionOptions</span></span>|<span data-ttu-id="60aab-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="60aab-135">Optional.</span></span> <span data-ttu-id="60aab-136">Opções de proteção da planilha.</span><span class="sxs-lookup"><span data-stu-id="60aab-136">sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="60aab-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="60aab-137">Response</span></span>

<span data-ttu-id="60aab-p107">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60aab-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60aab-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60aab-140">Example</span></span>
<span data-ttu-id="60aab-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="60aab-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="60aab-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60aab-142">Request</span></span>
<span data-ttu-id="60aab-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60aab-143">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="60aab-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="60aab-144">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="60aab-145">C#</span><span class="sxs-lookup"><span data-stu-id="60aab-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheetprotection-protect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60aab-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60aab-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheetprotection-protect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="60aab-147">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="60aab-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheetprotection-protect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="60aab-148">Java</span><span class="sxs-lookup"><span data-stu-id="60aab-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheetprotection-protect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="60aab-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="60aab-149">Response</span></span>
<span data-ttu-id="60aab-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60aab-150">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
