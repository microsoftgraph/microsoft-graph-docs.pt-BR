---
title: 'workbookWorksheetProtection: unprotect'
description: Desprotege uma planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 3201961496da64d917f59d8305cee98a0ab9ebfc
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578084"
---
# <a name="workbookworksheetprotection-unprotect"></a><span data-ttu-id="3fc00-103">workbookWorksheetProtection: unprotect</span><span class="sxs-lookup"><span data-stu-id="3fc00-103">workbookWorksheetProtection: unprotect</span></span>

<span data-ttu-id="3fc00-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fc00-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3fc00-105">Desprotege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="3fc00-105">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="3fc00-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3fc00-106">Permissions</span></span>
<span data-ttu-id="3fc00-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fc00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fc00-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3fc00-109">Permission type</span></span>      | <span data-ttu-id="3fc00-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3fc00-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3fc00-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3fc00-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3fc00-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fc00-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3fc00-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3fc00-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3fc00-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fc00-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3fc00-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3fc00-115">Application</span></span> | <span data-ttu-id="3fc00-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3fc00-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3fc00-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3fc00-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="3fc00-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3fc00-118">Request headers</span></span>
| <span data-ttu-id="3fc00-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3fc00-119">Name</span></span>       | <span data-ttu-id="3fc00-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fc00-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3fc00-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3fc00-121">Authorization</span></span>  | <span data-ttu-id="3fc00-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3fc00-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3fc00-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3fc00-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="3fc00-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="3fc00-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fc00-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3fc00-127">Request body</span></span>
<span data-ttu-id="3fc00-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3fc00-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3fc00-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3fc00-129">Parameter</span></span>    | <span data-ttu-id="3fc00-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3fc00-130">Type</span></span>   |<span data-ttu-id="3fc00-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fc00-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3fc00-132">password</span><span class="sxs-lookup"><span data-stu-id="3fc00-132">password</span></span>|<span data-ttu-id="3fc00-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3fc00-133">string</span></span>|<span data-ttu-id="3fc00-p104">Opcional. Senha de proteção para a planilha.</span><span class="sxs-lookup"><span data-stu-id="3fc00-p104">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="3fc00-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fc00-136">Response</span></span>

<span data-ttu-id="3fc00-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3fc00-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fc00-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3fc00-139">Example</span></span>
<span data-ttu-id="3fc00-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="3fc00-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3fc00-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3fc00-141">Request</span></span>
<span data-ttu-id="3fc00-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3fc00-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3fc00-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="3fc00-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3fc00-144">C#</span><span class="sxs-lookup"><span data-stu-id="3fc00-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookworksheetprotection-unprotect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3fc00-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3fc00-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookworksheetprotection-unprotect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3fc00-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3fc00-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookworksheetprotection-unprotect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3fc00-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fc00-147">Response</span></span>
<span data-ttu-id="3fc00-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3fc00-148">Here is an example of the response.</span></span> 
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
  "description": "workbookWorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


