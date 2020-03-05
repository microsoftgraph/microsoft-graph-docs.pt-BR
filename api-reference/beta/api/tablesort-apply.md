---
title: 'TableSort: apply'
description: Execute uma operação de classificação.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 27e4708f52a0bbe0966de11fa83a26d5f2a011a9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452642"
---
# <a name="tablesort-apply"></a><span data-ttu-id="836b1-103">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="836b1-103">TableSort: apply</span></span>

<span data-ttu-id="836b1-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="836b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="836b1-105">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="836b1-105">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="836b1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="836b1-106">Permissions</span></span>
<span data-ttu-id="836b1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="836b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="836b1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="836b1-109">Permission type</span></span>      | <span data-ttu-id="836b1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="836b1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="836b1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="836b1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="836b1-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="836b1-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="836b1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="836b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="836b1-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="836b1-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="836b1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="836b1-115">Application</span></span> | <span data-ttu-id="836b1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="836b1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="836b1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="836b1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="836b1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="836b1-118">Request headers</span></span>
| <span data-ttu-id="836b1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="836b1-119">Name</span></span>       | <span data-ttu-id="836b1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="836b1-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="836b1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="836b1-121">Authorization</span></span>  | <span data-ttu-id="836b1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="836b1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="836b1-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="836b1-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="836b1-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="836b1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="836b1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="836b1-127">Request body</span></span>
<span data-ttu-id="836b1-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="836b1-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="836b1-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="836b1-129">Parameter</span></span>    | <span data-ttu-id="836b1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="836b1-130">Type</span></span>   |<span data-ttu-id="836b1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="836b1-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="836b1-132">campos</span><span class="sxs-lookup"><span data-stu-id="836b1-132">fields</span></span>|<span data-ttu-id="836b1-133">coleção workbookSortField</span><span class="sxs-lookup"><span data-stu-id="836b1-133">workbookSortField collection</span></span>|<span data-ttu-id="836b1-134">A lista de condições para a classificação.</span><span class="sxs-lookup"><span data-stu-id="836b1-134">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="836b1-135">matchCase</span><span class="sxs-lookup"><span data-stu-id="836b1-135">matchCase</span></span>|<span data-ttu-id="836b1-136">booliano</span><span class="sxs-lookup"><span data-stu-id="836b1-136">boolean</span></span>|<span data-ttu-id="836b1-p104">Opcional. Define se o uso de maiúsculas ou minúsculas afeta a ordenação da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="836b1-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="836b1-139">method</span><span class="sxs-lookup"><span data-stu-id="836b1-139">method</span></span>|<span data-ttu-id="836b1-140">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="836b1-140">string</span></span>|<span data-ttu-id="836b1-p105">Opcional. O método de ordenação usado pelos caracteres chineses.  Os valores possíveis são: `PinYin` e `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="836b1-p105">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="836b1-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="836b1-144">Response</span></span>

<span data-ttu-id="836b1-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="836b1-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="836b1-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="836b1-147">Example</span></span>
<span data-ttu-id="836b1-148">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="836b1-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="836b1-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="836b1-149">Request</span></span>
<span data-ttu-id="836b1-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="836b1-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="836b1-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="836b1-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="836b1-152">C#</span><span class="sxs-lookup"><span data-stu-id="836b1-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="836b1-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="836b1-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="836b1-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="836b1-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="836b1-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="836b1-155">Response</span></span>
<span data-ttu-id="836b1-156">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="836b1-156">Here is an example of the response.</span></span> 
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
