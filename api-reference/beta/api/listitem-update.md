---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Atualizar um registro em uma lista do SharePoint
ms.openlocfilehash: a3d5ca140f56da1de5f4134fbe76f55b350e83a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033419"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="751db-102">Atualizar um item em uma lista</span><span class="sxs-lookup"><span data-stu-id="751db-102">Update an item in a list</span></span>

> <span data-ttu-id="751db-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="751db-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="751db-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="751db-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="751db-105">Atualizar as propriedades em um **[listItem][]**.</span><span class="sxs-lookup"><span data-stu-id="751db-105">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="751db-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="751db-106">Permissions</span></span>

<span data-ttu-id="751db-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="751db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="751db-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="751db-109">Permission type</span></span>      | <span data-ttu-id="751db-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="751db-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="751db-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="751db-111">Delegated (work or school account)</span></span> | <span data-ttu-id="751db-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="751db-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="751db-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="751db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="751db-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="751db-114">Not supported.</span></span>    |
|<span data-ttu-id="751db-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="751db-115">Application</span></span> | <span data-ttu-id="751db-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="751db-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="751db-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="751db-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="751db-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="751db-118">Optional request headers</span></span>

| <span data-ttu-id="751db-119">Nome</span><span class="sxs-lookup"><span data-stu-id="751db-119">Name</span></span>       | <span data-ttu-id="751db-120">Valor</span><span class="sxs-lookup"><span data-stu-id="751db-120">Value</span></span> | <span data-ttu-id="751db-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="751db-121">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="751db-122">_if-match_</span><span class="sxs-lookup"><span data-stu-id="751db-122">_if-match_</span></span> | <span data-ttu-id="751db-123">etag</span><span class="sxs-lookup"><span data-stu-id="751db-123">etag</span></span>  | <span data-ttu-id="751db-124">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à eTag atual no item, uma resposta `412 Precondition Failed` será exibida e o item não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="751db-124">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="751db-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="751db-125">Request body</span></span>

<span data-ttu-id="751db-126">No corpo da solicitação, forneça uma representação JSON de [fieldValueSet][] especificando os campos a atualizar.</span><span class="sxs-lookup"><span data-stu-id="751db-126">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="751db-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="751db-127">Example</span></span>

<span data-ttu-id="751db-128">Aqui está um exemplo que atualiza os campos de cor e quantidade do item de lista com novos valores.</span><span class="sxs-lookup"><span data-stu-id="751db-128">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="751db-129">Todos os outros valores no listItem ficam inalterados.</span><span class="sxs-lookup"><span data-stu-id="751db-129">All other values on the listItem are left alone.</span></span> 

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```

## <a name="response"></a><span data-ttu-id="751db-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="751db-130">Response</span></span>

<span data-ttu-id="751db-131">Se for bem-sucedido, esse método retornará um [fieldValueSet][] no corpo da resposta do item de lista atualizada.</span><span class="sxs-lookup"><span data-stu-id="751db-131">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

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

[fieldValueSet]: ../resources/fieldvalueset.md
[listItem]: ../resources/listitem.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update"
} -->
