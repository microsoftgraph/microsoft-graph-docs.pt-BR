---
title: 'TableSort: apply'
description: Execute uma operação de classificação.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 84ea48137560c435dc36b98e3730144e2eee87c1
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637679"
---
# <a name="tablesort-apply"></a><span data-ttu-id="340bc-103">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="340bc-103">TableSort: apply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="340bc-104">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="340bc-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="340bc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="340bc-105">Permissions</span></span>
<span data-ttu-id="340bc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="340bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="340bc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="340bc-108">Permission type</span></span>      | <span data-ttu-id="340bc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="340bc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="340bc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="340bc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="340bc-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="340bc-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="340bc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="340bc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="340bc-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="340bc-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="340bc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="340bc-114">Application</span></span> | <span data-ttu-id="340bc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="340bc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="340bc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="340bc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="340bc-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="340bc-117">Request headers</span></span>
| <span data-ttu-id="340bc-118">Nome</span><span class="sxs-lookup"><span data-stu-id="340bc-118">Name</span></span>       | <span data-ttu-id="340bc-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="340bc-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="340bc-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="340bc-120">Authorization</span></span>  | <span data-ttu-id="340bc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="340bc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="340bc-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="340bc-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="340bc-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="340bc-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="340bc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="340bc-126">Request body</span></span>
<span data-ttu-id="340bc-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="340bc-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="340bc-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="340bc-128">Parameter</span></span>    | <span data-ttu-id="340bc-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="340bc-129">Type</span></span>   |<span data-ttu-id="340bc-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="340bc-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="340bc-131">campos</span><span class="sxs-lookup"><span data-stu-id="340bc-131">fields</span></span>|<span data-ttu-id="340bc-132">coleção workbookSortField</span><span class="sxs-lookup"><span data-stu-id="340bc-132">workbookSortField collection</span></span>|<span data-ttu-id="340bc-133">A lista de condições para a classificação.</span><span class="sxs-lookup"><span data-stu-id="340bc-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="340bc-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="340bc-134">matchCase</span></span>|<span data-ttu-id="340bc-135">booliano</span><span class="sxs-lookup"><span data-stu-id="340bc-135">boolean</span></span>|<span data-ttu-id="340bc-p104">Opcional. Define se o uso de maiúsculas ou minúsculas afeta a ordenação da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="340bc-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="340bc-138">method</span><span class="sxs-lookup"><span data-stu-id="340bc-138">method</span></span>|<span data-ttu-id="340bc-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="340bc-139">string</span></span>|<span data-ttu-id="340bc-p105">Opcional. O método de ordenação usado pelos caracteres chineses.  Os valores possíveis são: `PinYin` e `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="340bc-p105">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="340bc-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="340bc-143">Response</span></span>

<span data-ttu-id="340bc-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="340bc-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="340bc-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="340bc-146">Example</span></span>
<span data-ttu-id="340bc-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="340bc-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="340bc-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="340bc-148">Request</span></span>
<span data-ttu-id="340bc-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="340bc-149">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="340bc-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="340bc-150">Response</span></span>
<span data-ttu-id="340bc-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="340bc-151">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="340bc-152">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="340bc-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="340bc-153">Basic</span><span class="sxs-lookup"><span data-stu-id="340bc-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tablesort_apply-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="340bc-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="340bc-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tablesort_apply-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/tablesort-apply.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tablesort-apply.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
