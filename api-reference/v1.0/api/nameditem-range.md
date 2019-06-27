---
title: 'NamedItem: Range'
description: Retorna o objeto Range associado ao nome. Gera uma exceção quando o tipo de item nomeado não é um intervalo.
localization_priority: Normal
ms.openlocfilehash: d6ada5c4a5dce8c5a2ddb1510e69aba38f373134
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276661"
---
# <a name="nameditem-range"></a><span data-ttu-id="40d65-104">NamedItem: Range</span><span class="sxs-lookup"><span data-stu-id="40d65-104">NamedItem: Range</span></span>

<span data-ttu-id="40d65-p102">Retorna o objeto Range associado ao nome. Gera uma exceção quando o tipo de item nomeado não é um intervalo.</span><span class="sxs-lookup"><span data-stu-id="40d65-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>
## <a name="permissions"></a><span data-ttu-id="40d65-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="40d65-107">Permissions</span></span>
<span data-ttu-id="40d65-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40d65-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40d65-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40d65-110">Permission type</span></span>      | <span data-ttu-id="40d65-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40d65-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40d65-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40d65-112">Delegated (work or school account)</span></span> | <span data-ttu-id="40d65-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40d65-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="40d65-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40d65-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40d65-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40d65-115">Not supported.</span></span>    |
|<span data-ttu-id="40d65-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40d65-116">Application</span></span> | <span data-ttu-id="40d65-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40d65-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="40d65-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40d65-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range

```
## <a name="request-headers"></a><span data-ttu-id="40d65-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40d65-119">Request headers</span></span>
| <span data-ttu-id="40d65-120">Nome</span><span class="sxs-lookup"><span data-stu-id="40d65-120">Name</span></span>       | <span data-ttu-id="40d65-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="40d65-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="40d65-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="40d65-122">Authorization</span></span>  | <span data-ttu-id="40d65-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40d65-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="40d65-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="40d65-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="40d65-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="40d65-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="40d65-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40d65-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="40d65-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="40d65-129">Response</span></span>

<span data-ttu-id="40d65-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40d65-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40d65-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40d65-131">Example</span></span>
<span data-ttu-id="40d65-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="40d65-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="40d65-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40d65-133">Request</span></span>
<span data-ttu-id="40d65-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40d65-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "idempotent": true,
  "name": "nameditem_range"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range
```

##### <a name="response"></a><span data-ttu-id="40d65-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="40d65-135">Response</span></span>
<span data-ttu-id="40d65-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40d65-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="40d65-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="40d65-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="40d65-140">C#</span><span class="sxs-lookup"><span data-stu-id="40d65-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/nameditem_range-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="40d65-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="40d65-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/nameditem_range-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="40d65-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="40d65-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/nameditem_range-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/nameditem-range.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/nameditem-range.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/nameditem-range.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
