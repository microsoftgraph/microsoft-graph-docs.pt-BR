---
title: 'TableSort: apply'
description: Execute uma operação de classificação.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c06825da7f29fcfa3adb409f391d62208461400d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35990880"
---
# <a name="tablesort-apply"></a><span data-ttu-id="50a54-103">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="50a54-103">TableSort: apply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50a54-104">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="50a54-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="50a54-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="50a54-105">Permissions</span></span>
<span data-ttu-id="50a54-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50a54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50a54-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50a54-108">Permission type</span></span>      | <span data-ttu-id="50a54-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="50a54-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50a54-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50a54-110">Delegated (work or school account)</span></span> | <span data-ttu-id="50a54-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50a54-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="50a54-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50a54-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50a54-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50a54-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="50a54-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50a54-114">Application</span></span> | <span data-ttu-id="50a54-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50a54-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="50a54-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50a54-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="50a54-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50a54-117">Request headers</span></span>
| <span data-ttu-id="50a54-118">Nome</span><span class="sxs-lookup"><span data-stu-id="50a54-118">Name</span></span>       | <span data-ttu-id="50a54-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="50a54-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="50a54-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="50a54-120">Authorization</span></span>  | <span data-ttu-id="50a54-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50a54-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="50a54-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="50a54-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="50a54-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="50a54-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="50a54-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50a54-126">Request body</span></span>
<span data-ttu-id="50a54-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50a54-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="50a54-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="50a54-128">Parameter</span></span>    | <span data-ttu-id="50a54-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="50a54-129">Type</span></span>   |<span data-ttu-id="50a54-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="50a54-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50a54-131">campos</span><span class="sxs-lookup"><span data-stu-id="50a54-131">fields</span></span>|<span data-ttu-id="50a54-132">coleção workbookSortField</span><span class="sxs-lookup"><span data-stu-id="50a54-132">workbookSortField collection</span></span>|<span data-ttu-id="50a54-133">A lista de condições para a classificação.</span><span class="sxs-lookup"><span data-stu-id="50a54-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="50a54-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="50a54-134">matchCase</span></span>|<span data-ttu-id="50a54-135">booliano</span><span class="sxs-lookup"><span data-stu-id="50a54-135">boolean</span></span>|<span data-ttu-id="50a54-p104">Opcional. Define se o uso de maiúsculas ou minúsculas afeta a ordenação da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="50a54-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="50a54-138">method</span><span class="sxs-lookup"><span data-stu-id="50a54-138">method</span></span>|<span data-ttu-id="50a54-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50a54-139">string</span></span>|<span data-ttu-id="50a54-p105">Opcional. O método de ordenação usado pelos caracteres chineses.  Os valores possíveis são: `PinYin` e `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="50a54-p105">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="50a54-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="50a54-143">Response</span></span>

<span data-ttu-id="50a54-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50a54-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50a54-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50a54-146">Example</span></span>
<span data-ttu-id="50a54-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="50a54-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="50a54-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50a54-148">Request</span></span>
<span data-ttu-id="50a54-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50a54-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="50a54-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="50a54-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablesort_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply
Content-type: application/json
Content-length: 298

{
  "fields": [
    {
      "key": 99,
      "sortOn": "sortOn-value",
      "ascending": true,
      "color": "color-value",
      "dataOption": "dataOption-value",
      "icon": {
        "set": "set-value",
        "index": 99
      }
    }
  ],
  "matchCase": true,
  "method": "method-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="50a54-151">C#</span><span class="sxs-lookup"><span data-stu-id="50a54-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="50a54-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="50a54-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="50a54-153">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="50a54-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="50a54-154">Java</span><span class="sxs-lookup"><span data-stu-id="50a54-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablesort-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="50a54-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="50a54-155">Response</span></span>
<span data-ttu-id="50a54-156">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50a54-156">Here is an example of the response.</span></span> 
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
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
