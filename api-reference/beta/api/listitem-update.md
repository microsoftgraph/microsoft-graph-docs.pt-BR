---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Atualizar um registro em uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7c5031a9f2d2729a268f26bb1b1489f3bae2c351
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536488"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="7d520-102">Atualizar um item em uma lista</span><span class="sxs-lookup"><span data-stu-id="7d520-102">Update an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d520-103">Atualizar as propriedades em um **[listItem][]**.</span><span class="sxs-lookup"><span data-stu-id="7d520-103">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d520-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="7d520-104">Permissions</span></span>

<span data-ttu-id="7d520-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d520-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d520-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d520-107">Permission type</span></span>      | <span data-ttu-id="7d520-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7d520-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d520-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d520-109">Delegated (work or school account)</span></span> | <span data-ttu-id="7d520-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d520-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7d520-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d520-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d520-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d520-112">Not supported.</span></span>    |
|<span data-ttu-id="7d520-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d520-113">Application</span></span> | <span data-ttu-id="7d520-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d520-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d520-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d520-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="7d520-116">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="7d520-116">Optional request headers</span></span>

| <span data-ttu-id="7d520-117">Nome</span><span class="sxs-lookup"><span data-stu-id="7d520-117">Name</span></span>       | <span data-ttu-id="7d520-118">Valor</span><span class="sxs-lookup"><span data-stu-id="7d520-118">Value</span></span> | <span data-ttu-id="7d520-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d520-119">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="7d520-120">_if-match_</span><span class="sxs-lookup"><span data-stu-id="7d520-120">_if-match_</span></span> | <span data-ttu-id="7d520-121">etag</span><span class="sxs-lookup"><span data-stu-id="7d520-121">etag</span></span>  | <span data-ttu-id="7d520-122">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à eTag atual no item, uma resposta `412 Precondition Failed` será exibida e o item não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="7d520-122">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="7d520-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d520-123">Request body</span></span>

<span data-ttu-id="7d520-124">No corpo da solicitação, forneça uma representação JSON de [fieldValueSet][] especificando os campos a atualizar.</span><span class="sxs-lookup"><span data-stu-id="7d520-124">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="7d520-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d520-125">Example</span></span>

<span data-ttu-id="7d520-126">Aqui está um exemplo que atualiza os campos de cor e quantidade do item de lista com novos valores.</span><span class="sxs-lookup"><span data-stu-id="7d520-126">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="7d520-127">Todos os outros valores no listItem ficam inalterados.</span><span class="sxs-lookup"><span data-stu-id="7d520-127">All other values on the listItem are left alone.</span></span> 

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```

## <a name="response"></a><span data-ttu-id="7d520-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d520-128">Response</span></span>

<span data-ttu-id="7d520-129">Se for bem-sucedido, esse método retornará um [fieldValueSet][] no corpo da resposta do item de lista atualizada.</span><span class="sxs-lookup"><span data-stu-id="7d520-129">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7d520-130">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="7d520-130">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7d520-131">C#</span><span class="sxs-lookup"><span data-stu-id="7d520-131">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create-listitem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7d520-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="7d520-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create-listitem-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/listitem-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/listitem-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
