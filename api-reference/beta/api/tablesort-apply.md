---
title: 'TableSort: apply'
description: Execute uma operação de classificação.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: dec0364db914f9c834b8507de52c7809f44c3fba
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575347"
---
# <a name="tablesort-apply"></a><span data-ttu-id="38cf9-103">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="38cf9-103">TableSort: apply</span></span>

<span data-ttu-id="38cf9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38cf9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38cf9-105">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="38cf9-105">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="38cf9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="38cf9-106">Permissions</span></span>
<span data-ttu-id="38cf9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38cf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38cf9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38cf9-109">Permission type</span></span>      | <span data-ttu-id="38cf9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38cf9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38cf9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38cf9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="38cf9-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38cf9-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="38cf9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38cf9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38cf9-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38cf9-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="38cf9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38cf9-115">Application</span></span> | <span data-ttu-id="38cf9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38cf9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="38cf9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38cf9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/sort/apply
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/sort/apply
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/sort/apply
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="38cf9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38cf9-118">Request headers</span></span>
| <span data-ttu-id="38cf9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="38cf9-119">Name</span></span>       | <span data-ttu-id="38cf9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="38cf9-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="38cf9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="38cf9-121">Authorization</span></span>  | <span data-ttu-id="38cf9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38cf9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="38cf9-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="38cf9-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="38cf9-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="38cf9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="38cf9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38cf9-127">Request body</span></span>
<span data-ttu-id="38cf9-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38cf9-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="38cf9-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="38cf9-129">Parameter</span></span>    | <span data-ttu-id="38cf9-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="38cf9-130">Type</span></span>   |<span data-ttu-id="38cf9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="38cf9-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38cf9-132">campos</span><span class="sxs-lookup"><span data-stu-id="38cf9-132">fields</span></span>|<span data-ttu-id="38cf9-133">workbookSortField collection</span><span class="sxs-lookup"><span data-stu-id="38cf9-133">workbookSortField collection</span></span>|<span data-ttu-id="38cf9-134">A lista de condições para a classificação.</span><span class="sxs-lookup"><span data-stu-id="38cf9-134">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="38cf9-135">matchCase</span><span class="sxs-lookup"><span data-stu-id="38cf9-135">matchCase</span></span>|<span data-ttu-id="38cf9-136">booliano</span><span class="sxs-lookup"><span data-stu-id="38cf9-136">boolean</span></span>|<span data-ttu-id="38cf9-p104">Opcional. Define se o uso de maiúsculas ou minúsculas afeta a ordenação da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="38cf9-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="38cf9-139">method</span><span class="sxs-lookup"><span data-stu-id="38cf9-139">method</span></span>|<span data-ttu-id="38cf9-140">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38cf9-140">string</span></span>|<span data-ttu-id="38cf9-p105">Opcional. O método de ordenação usado pelos caracteres chineses.  Os valores possíveis são: `PinYin` e `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="38cf9-p105">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="38cf9-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="38cf9-144">Response</span></span>

<span data-ttu-id="38cf9-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38cf9-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38cf9-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38cf9-147">Example</span></span>
<span data-ttu-id="38cf9-148">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="38cf9-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="38cf9-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38cf9-149">Request</span></span>
<span data-ttu-id="38cf9-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38cf9-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="38cf9-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="38cf9-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="38cf9-152">C#</span><span class="sxs-lookup"><span data-stu-id="38cf9-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="38cf9-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38cf9-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="38cf9-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38cf9-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="38cf9-155">Java</span><span class="sxs-lookup"><span data-stu-id="38cf9-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablesort-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="38cf9-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="38cf9-156">Response</span></span>
<span data-ttu-id="38cf9-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38cf9-157">Here is an example of the response.</span></span> 
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


