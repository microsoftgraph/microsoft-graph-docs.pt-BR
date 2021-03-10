---
title: 'WorksheetProtection: protect'
description: Protege uma planilha. Gera uma exceção se a planilha estiver protegida.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 82917ab1b2c1fa20b6331182512ef78c847a426a
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577482"
---
# <a name="worksheetprotection-protect"></a><span data-ttu-id="b9b09-104">WorksheetProtection: protect</span><span class="sxs-lookup"><span data-stu-id="b9b09-104">WorksheetProtection: protect</span></span>

<span data-ttu-id="b9b09-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9b09-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b9b09-106">Protege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="b9b09-106">Protect a worksheet.</span></span> <span data-ttu-id="b9b09-107">Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="b9b09-107">It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="b9b09-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b9b09-108">Permissions</span></span>
<span data-ttu-id="b9b09-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9b09-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9b09-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9b09-111">Permission type</span></span>      | <span data-ttu-id="b9b09-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9b09-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9b09-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9b09-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b9b09-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9b09-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b9b09-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9b09-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9b09-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9b09-116">Not supported.</span></span>    |
|<span data-ttu-id="b9b09-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9b09-117">Application</span></span> | <span data-ttu-id="b9b09-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9b09-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9b09-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9b09-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/protection/protect
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="b9b09-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9b09-120">Request headers</span></span>
| <span data-ttu-id="b9b09-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b9b09-121">Name</span></span>       | <span data-ttu-id="b9b09-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9b09-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b9b09-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9b09-123">Authorization</span></span>  | <span data-ttu-id="b9b09-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9b09-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b9b09-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b9b09-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="b9b09-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="b9b09-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9b09-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9b09-129">Request body</span></span>
<span data-ttu-id="b9b09-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9b09-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b9b09-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b9b09-131">Parameter</span></span>    | <span data-ttu-id="b9b09-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9b09-132">Type</span></span>   |<span data-ttu-id="b9b09-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9b09-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9b09-134">options</span><span class="sxs-lookup"><span data-stu-id="b9b09-134">options</span></span>|<span data-ttu-id="b9b09-135">WorkbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="b9b09-135">WorkbookWorksheetProtectionOptions</span></span>|<span data-ttu-id="b9b09-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b9b09-136">Optional.</span></span> <span data-ttu-id="b9b09-137">Opções de proteção da planilha.</span><span class="sxs-lookup"><span data-stu-id="b9b09-137">sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="b9b09-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9b09-138">Response</span></span>

<span data-ttu-id="b9b09-p107">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9b09-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9b09-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9b09-141">Example</span></span>
<span data-ttu-id="b9b09-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b9b09-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b9b09-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9b09-143">Request</span></span>
<span data-ttu-id="b9b09-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9b09-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b9b09-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9b09-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b9b09-146">C#</span><span class="sxs-lookup"><span data-stu-id="b9b09-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheetprotection-protect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9b09-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9b09-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheetprotection-protect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9b09-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9b09-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheetprotection-protect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9b09-149">Java</span><span class="sxs-lookup"><span data-stu-id="b9b09-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheetprotection-protect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b9b09-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9b09-150">Response</span></span>
<span data-ttu-id="b9b09-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9b09-151">Here is an example of the response.</span></span> 
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

