---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Atualizar um registro em uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f365331b5941da48178194c9b02f61aaf1893ed6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264523"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="5e41c-102">Atualizar um item em uma lista</span><span class="sxs-lookup"><span data-stu-id="5e41c-102">Update an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e41c-103">Atualizar as propriedades em um **[listItem][]**.</span><span class="sxs-lookup"><span data-stu-id="5e41c-103">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e41c-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="5e41c-104">Permissions</span></span>

<span data-ttu-id="5e41c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e41c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e41c-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e41c-107">Permission type</span></span>      | <span data-ttu-id="5e41c-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5e41c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e41c-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e41c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="5e41c-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e41c-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="5e41c-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e41c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e41c-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e41c-112">Not supported.</span></span>    |
|<span data-ttu-id="5e41c-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e41c-113">Application</span></span> | <span data-ttu-id="5e41c-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e41c-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e41c-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e41c-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="5e41c-116">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="5e41c-116">Optional request headers</span></span>

| <span data-ttu-id="5e41c-117">Nome</span><span class="sxs-lookup"><span data-stu-id="5e41c-117">Name</span></span>       | <span data-ttu-id="5e41c-118">Valor</span><span class="sxs-lookup"><span data-stu-id="5e41c-118">Value</span></span> | <span data-ttu-id="5e41c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e41c-119">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="5e41c-120">_if-match_</span><span class="sxs-lookup"><span data-stu-id="5e41c-120">_if-match_</span></span> | <span data-ttu-id="5e41c-121">etag</span><span class="sxs-lookup"><span data-stu-id="5e41c-121">etag</span></span>  | <span data-ttu-id="5e41c-122">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à eTag atual no item, uma resposta `412 Precondition Failed` será exibida e o item não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="5e41c-122">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="5e41c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e41c-123">Request body</span></span>

<span data-ttu-id="5e41c-124">No corpo da solicitação, forneça uma representação JSON de [fieldValueSet][] especificando os campos a atualizar.</span><span class="sxs-lookup"><span data-stu-id="5e41c-124">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="5e41c-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e41c-125">Example</span></span>

<span data-ttu-id="5e41c-126">Aqui está um exemplo que atualiza os campos de cor e quantidade do item de lista com novos valores.</span><span class="sxs-lookup"><span data-stu-id="5e41c-126">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="5e41c-127">Todos os outros valores no listItem ficam inalterados.</span><span class="sxs-lookup"><span data-stu-id="5e41c-127">All other values on the listItem are left alone.</span></span> 

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```

## <a name="response"></a><span data-ttu-id="5e41c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e41c-128">Response</span></span>

<span data-ttu-id="5e41c-129">Se for bem-sucedido, esse método retornará um [fieldValueSet][] no corpo da resposta do item de lista atualizada.</span><span class="sxs-lookup"><span data-stu-id="5e41c-129">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "Name": "Widget",
  "Color": "Fuchsia",
  "Quantity": 934
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5e41c-130">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="5e41c-130">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5e41c-131">C#</span><span class="sxs-lookup"><span data-stu-id="5e41c-131">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create-listitem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5e41c-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="5e41c-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create-listitem-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5e41c-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5e41c-133">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create-listitem-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

[fieldValueSet]: ../resources/fieldvalueset.md
[listItem]: ../resources/listitem.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update",
  "suppressions": [
    "Error: /api-reference/beta/api/listitem-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/listitem-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/listitem-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
