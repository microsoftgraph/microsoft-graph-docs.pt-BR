---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Atualizar um registro em uma lista do SharePoint
localization_priority: Priority
ms.openlocfilehash: e96bcc25af715b644a1e3670514c85f8f6fd0e8f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805438"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="7ab42-102">Atualizar um item em uma lista</span><span class="sxs-lookup"><span data-stu-id="7ab42-102">Update an item in a list</span></span>

<span data-ttu-id="7ab42-103">Atualizar as propriedades em um **[listItem][]**.</span><span class="sxs-lookup"><span data-stu-id="7ab42-103">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ab42-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="7ab42-104">Permissions</span></span>

<span data-ttu-id="7ab42-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ab42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ab42-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ab42-107">Permission type</span></span>      | <span data-ttu-id="7ab42-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7ab42-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ab42-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ab42-109">Delegated (work or school account)</span></span> | <span data-ttu-id="7ab42-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ab42-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7ab42-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ab42-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ab42-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ab42-112">Not supported.</span></span>    |
|<span data-ttu-id="7ab42-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ab42-113">Application</span></span> | <span data-ttu-id="7ab42-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ab42-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ab42-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ab42-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="7ab42-116">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="7ab42-116">Optional request headers</span></span>

| <span data-ttu-id="7ab42-117">Nome</span><span class="sxs-lookup"><span data-stu-id="7ab42-117">Name</span></span>       | <span data-ttu-id="7ab42-118">Valor</span><span class="sxs-lookup"><span data-stu-id="7ab42-118">Value</span></span> | <span data-ttu-id="7ab42-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ab42-119">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="7ab42-120">_if-match_</span><span class="sxs-lookup"><span data-stu-id="7ab42-120">_if-match_</span></span> | <span data-ttu-id="7ab42-121">etag</span><span class="sxs-lookup"><span data-stu-id="7ab42-121">etag</span></span>  | <span data-ttu-id="7ab42-122">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à eTag atual no item, uma resposta `412 Precondition Failed` será exibida e o item não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="7ab42-122">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="7ab42-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ab42-123">Request body</span></span>

<span data-ttu-id="7ab42-124">No corpo da solicitação, forneça uma representação JSON de [fieldValueSet][] especificando os campos a atualizar.</span><span class="sxs-lookup"><span data-stu-id="7ab42-124">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="7ab42-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ab42-125">Example</span></span>

<span data-ttu-id="7ab42-126">Aqui está um exemplo que atualiza os campos de cor e quantidade do item de lista com novos valores.</span><span class="sxs-lookup"><span data-stu-id="7ab42-126">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="7ab42-127">Todos os outros valores no listItem ficam inalterados.</span><span class="sxs-lookup"><span data-stu-id="7ab42-127">All other values on the listItem are left alone.</span></span> 

<!-- { "blockType": "request", "name": "update-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```

## <a name="response"></a><span data-ttu-id="7ab42-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ab42-128">Response</span></span>

<span data-ttu-id="7ab42-129">Se for bem-sucedido, esse método retornará um [fieldValueSet][] no corpo da resposta do item de lista atualizada.</span><span class="sxs-lookup"><span data-stu-id="7ab42-129">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.fieldValueSet", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "Name": "Widget",
  "Color": "Fuchsia",
  "Quantity": 934
}
```

[fieldValueSet]: ../resources/fieldvalueset.md
[listItem]: ../resources/listitem.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update"
} -->
