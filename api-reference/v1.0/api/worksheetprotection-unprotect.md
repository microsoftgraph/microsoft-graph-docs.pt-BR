---
title: 'WorksheetProtection: unprotect'
description: Desprotege uma planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 71f6ded64f4845619ded39faf693cdf2f7fd305e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455011"
---
# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="f1f97-103">WorksheetProtection: unprotect</span><span class="sxs-lookup"><span data-stu-id="f1f97-103">WorksheetProtection: unprotect</span></span>

<span data-ttu-id="f1f97-104">Desprotege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="f1f97-104">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="f1f97-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1f97-105">Permissions</span></span>
<span data-ttu-id="f1f97-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1f97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1f97-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1f97-108">Permission type</span></span>      | <span data-ttu-id="f1f97-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1f97-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1f97-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1f97-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f1f97-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1f97-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f1f97-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1f97-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1f97-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1f97-113">Not supported.</span></span>    |
|<span data-ttu-id="f1f97-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1f97-114">Application</span></span> | <span data-ttu-id="f1f97-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1f97-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1f97-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1f97-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="f1f97-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1f97-117">Request headers</span></span>
| <span data-ttu-id="f1f97-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f1f97-118">Name</span></span>       | <span data-ttu-id="f1f97-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1f97-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f1f97-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1f97-120">Authorization</span></span>  | <span data-ttu-id="f1f97-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1f97-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f1f97-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f1f97-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="f1f97-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f1f97-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1f97-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1f97-126">Request body</span></span>
<span data-ttu-id="f1f97-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1f97-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f1f97-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f1f97-128">Parameter</span></span>    | <span data-ttu-id="f1f97-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1f97-129">Type</span></span>   |<span data-ttu-id="f1f97-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1f97-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1f97-131">password</span><span class="sxs-lookup"><span data-stu-id="f1f97-131">password</span></span>|<span data-ttu-id="f1f97-132">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1f97-132">string</span></span>|<span data-ttu-id="f1f97-p104">Opcional. Senha de proteção para a planilha.</span><span class="sxs-lookup"><span data-stu-id="f1f97-p104">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="f1f97-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1f97-135">Response</span></span>

<span data-ttu-id="f1f97-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1f97-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1f97-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1f97-138">Example</span></span>
<span data-ttu-id="f1f97-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f1f97-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f1f97-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1f97-140">Request</span></span>
<span data-ttu-id="f1f97-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1f97-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f1f97-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1f97-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_unprotect"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
Content-type: application/json
Content-length: 34

{
  "password": "password-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f1f97-143">C#</span><span class="sxs-lookup"><span data-stu-id="f1f97-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheetprotection-unprotect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f1f97-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="f1f97-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheetprotection-unprotect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f1f97-145">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f1f97-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheetprotection-unprotect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f1f97-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1f97-146">Response</span></span>
<span data-ttu-id="f1f97-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1f97-147">Here is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
