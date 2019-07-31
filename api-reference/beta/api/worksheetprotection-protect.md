---
title: 'workbookWorksheetProtection: proteger'
description: Protege uma planilha. Gera uma exceção se a planilha estiver protegida.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 124e94a056528adfcd2e81b138037d3651ddd32b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987193"
---
# <a name="workbookworksheetprotection-protect"></a><span data-ttu-id="35784-104">workbookWorksheetProtection: proteger</span><span class="sxs-lookup"><span data-stu-id="35784-104">workbookWorksheetProtection: protect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35784-105">Protege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="35784-105">Protect a worksheet.</span></span> <span data-ttu-id="35784-106">Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="35784-106">It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="35784-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="35784-107">Permissions</span></span>
<span data-ttu-id="35784-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35784-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35784-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35784-110">Permission type</span></span>      | <span data-ttu-id="35784-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="35784-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35784-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35784-112">Delegated (work or school account)</span></span> | <span data-ttu-id="35784-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35784-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="35784-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35784-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35784-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35784-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="35784-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35784-116">Application</span></span> | <span data-ttu-id="35784-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35784-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="35784-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35784-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="35784-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35784-119">Request headers</span></span>
| <span data-ttu-id="35784-120">Nome</span><span class="sxs-lookup"><span data-stu-id="35784-120">Name</span></span>       | <span data-ttu-id="35784-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="35784-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="35784-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="35784-122">Authorization</span></span>  | <span data-ttu-id="35784-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35784-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="35784-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="35784-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="35784-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="35784-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="35784-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35784-128">Request body</span></span>
<span data-ttu-id="35784-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="35784-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="35784-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="35784-130">Parameter</span></span>    | <span data-ttu-id="35784-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="35784-131">Type</span></span>   |<span data-ttu-id="35784-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="35784-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35784-133">options</span><span class="sxs-lookup"><span data-stu-id="35784-133">options</span></span>|[<span data-ttu-id="35784-134">workbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="35784-134">workbookWorksheetProtectionOptions</span></span>](../resources/workbookworksheetprotectionoptions.md)|<span data-ttu-id="35784-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="35784-135">Optional.</span></span> <span data-ttu-id="35784-136">Opções de proteção da planilha.</span><span class="sxs-lookup"><span data-stu-id="35784-136">sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="35784-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="35784-137">Response</span></span>

<span data-ttu-id="35784-p107">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35784-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35784-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35784-140">Example</span></span>
<span data-ttu-id="35784-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="35784-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="35784-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35784-142">Request</span></span>
<span data-ttu-id="35784-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="35784-143">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="35784-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="35784-144">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="35784-145">C#</span><span class="sxs-lookup"><span data-stu-id="35784-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookworksheetprotection-protect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="35784-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="35784-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookworksheetprotection-protect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="35784-147">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="35784-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookworksheetprotection-protect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="35784-148">Java</span><span class="sxs-lookup"><span data-stu-id="35784-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookworksheetprotection-protect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="35784-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="35784-149">Response</span></span>
<span data-ttu-id="35784-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35784-150">Here is an example of the response.</span></span> 
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
