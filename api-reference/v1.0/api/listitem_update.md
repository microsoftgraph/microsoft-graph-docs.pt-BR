---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Atualizar um registro em uma lista do SharePoint
ms.openlocfilehash: fc025ef8c38a7d0768240038955187ee551d6b42
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="9d3d5-102">Atualizar um item em uma lista</span><span class="sxs-lookup"><span data-stu-id="9d3d5-102">Update an item in a list</span></span>

<span data-ttu-id="9d3d5-103">Atualizar as propriedades em um **[listItem][]**.</span><span class="sxs-lookup"><span data-stu-id="9d3d5-103">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d3d5-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="9d3d5-104">Permissions</span></span>

<span data-ttu-id="9d3d5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9d3d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9d3d5-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d3d5-107">Permission type</span></span>      | <span data-ttu-id="9d3d5-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9d3d5-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d3d5-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d3d5-109">Delegated (work or school account)</span></span> | <span data-ttu-id="9d3d5-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d3d5-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9d3d5-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d3d5-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d3d5-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d3d5-112">Not supported.</span></span>    |
|<span data-ttu-id="9d3d5-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d3d5-113">Application</span></span> | <span data-ttu-id="9d3d5-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d3d5-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d3d5-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d3d5-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="9d3d5-116">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="9d3d5-116">Optional request headers</span></span>

| <span data-ttu-id="9d3d5-117">Nome</span><span class="sxs-lookup"><span data-stu-id="9d3d5-117">Name</span></span>       | <span data-ttu-id="9d3d5-118">Valor</span><span class="sxs-lookup"><span data-stu-id="9d3d5-118">Value</span></span> | <span data-ttu-id="9d3d5-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d3d5-119">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="9d3d5-120">_if-match_</span><span class="sxs-lookup"><span data-stu-id="9d3d5-120">_if-match_</span></span> | <span data-ttu-id="9d3d5-121">etag</span><span class="sxs-lookup"><span data-stu-id="9d3d5-121">etag</span></span>  | <span data-ttu-id="9d3d5-122">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à eTag atual no item, uma resposta `412 Precondition Failed` será exibida e o item não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="9d3d5-122">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>


## <a name="request-body"></a><span data-ttu-id="9d3d5-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d3d5-123">Request body</span></span>

<span data-ttu-id="9d3d5-124">No corpo da solicitação, forneça uma representação JSON de [fieldValueSet][] especificando os campos a atualizar.</span><span class="sxs-lookup"><span data-stu-id="9d3d5-124">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="9d3d5-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d3d5-125">Example</span></span>

<span data-ttu-id="9d3d5-126">Aqui está um exemplo que atualiza os campos de cor e quantidade do item de lista com novos valores.</span><span class="sxs-lookup"><span data-stu-id="9d3d5-126">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="9d3d5-127">Todos os outros valores no listItem ficam inalterados.</span><span class="sxs-lookup"><span data-stu-id="9d3d5-127">All other values on the listItem are left alone.</span></span> 

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```

## <a name="response"></a><span data-ttu-id="9d3d5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d3d5-128">Response</span></span>

<span data-ttu-id="9d3d5-129">Se for bem-sucedido, esse método retornará um [fieldValueSet][] no corpo da resposta do item de lista atualizada.</span><span class="sxs-lookup"><span data-stu-id="9d3d5-129">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

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

[fieldValueSet]: ../resources/fieldValueSet.md
[listItem]: ../resources/listItem.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update"
} -->
