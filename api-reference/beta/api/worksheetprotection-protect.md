---
title: 'workbookWorksheetProtection: proteger'
description: Protege uma planilha. Gera uma exceção se a planilha estiver protegida.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1ee9aff7f3f49da0c1b82ab4b953c4f3ae1a25e9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089886"
---
# <a name="workbookworksheetprotection-protect"></a><span data-ttu-id="63c1a-104">workbookWorksheetProtection: proteger</span><span class="sxs-lookup"><span data-stu-id="63c1a-104">workbookWorksheetProtection: protect</span></span>

<span data-ttu-id="63c1a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63c1a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63c1a-106">Protege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="63c1a-106">Protect a worksheet.</span></span> <span data-ttu-id="63c1a-107">Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="63c1a-107">It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="63c1a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="63c1a-108">Permissions</span></span>
<span data-ttu-id="63c1a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63c1a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63c1a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63c1a-111">Permission type</span></span>      | <span data-ttu-id="63c1a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63c1a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63c1a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63c1a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="63c1a-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63c1a-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="63c1a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63c1a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63c1a-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63c1a-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="63c1a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63c1a-117">Application</span></span> | <span data-ttu-id="63c1a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63c1a-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="63c1a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63c1a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="63c1a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63c1a-120">Request headers</span></span>
| <span data-ttu-id="63c1a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="63c1a-121">Name</span></span>       | <span data-ttu-id="63c1a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="63c1a-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="63c1a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="63c1a-123">Authorization</span></span>  | <span data-ttu-id="63c1a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63c1a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="63c1a-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="63c1a-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="63c1a-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="63c1a-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="63c1a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63c1a-129">Request body</span></span>
<span data-ttu-id="63c1a-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63c1a-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="63c1a-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="63c1a-131">Parameter</span></span>    | <span data-ttu-id="63c1a-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="63c1a-132">Type</span></span>   |<span data-ttu-id="63c1a-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="63c1a-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63c1a-134">options</span><span class="sxs-lookup"><span data-stu-id="63c1a-134">options</span></span>|[<span data-ttu-id="63c1a-135">workbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="63c1a-135">workbookWorksheetProtectionOptions</span></span>](../resources/workbookworksheetprotectionoptions.md)|<span data-ttu-id="63c1a-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="63c1a-136">Optional.</span></span> <span data-ttu-id="63c1a-137">Opções de proteção da planilha.</span><span class="sxs-lookup"><span data-stu-id="63c1a-137">sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="63c1a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="63c1a-138">Response</span></span>

<span data-ttu-id="63c1a-p107">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63c1a-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63c1a-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63c1a-141">Example</span></span>
<span data-ttu-id="63c1a-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="63c1a-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="63c1a-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63c1a-143">Request</span></span>
<span data-ttu-id="63c1a-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63c1a-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="63c1a-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="63c1a-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookworksheetprotection_protect"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/protect
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
# <a name="c"></a>[<span data-ttu-id="63c1a-146">C#</span><span class="sxs-lookup"><span data-stu-id="63c1a-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookworksheetprotection-protect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63c1a-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63c1a-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookworksheetprotection-protect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63c1a-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63c1a-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookworksheetprotection-protect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="63c1a-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="63c1a-149">Response</span></span>
<span data-ttu-id="63c1a-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63c1a-150">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookWorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


