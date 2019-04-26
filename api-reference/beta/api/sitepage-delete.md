---
author: rahmit
ms.author: rahmit
ms.date: 05/07/2018
title: Excluir uma página de um site do SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: d5c38a5f5b96a100cfbae0eba30f957b079568e5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330132"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a><span data-ttu-id="f051a-102">Excluir página da lista de páginas do site de um site</span><span class="sxs-lookup"><span data-stu-id="f051a-102">Delete page from the site pages list of a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f051a-103">Remove um [sitePage][] da [lista][] de páginas do site em um [site][].</span><span class="sxs-lookup"><span data-stu-id="f051a-103">Removes a [sitePage][] from the site pages [list][] in a [site][].</span></span>

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="f051a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f051a-107">Permissions</span></span>

<span data-ttu-id="f051a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f051a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="f051a-110">**Observação:** Para excluir um item, o usuário deve ter concedido o acesso de gravação do aplicativo ao item a ser excluído.</span><span class="sxs-lookup"><span data-stu-id="f051a-110">**Note:** To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

|<span data-ttu-id="f051a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f051a-111">Permission type</span></span>      | <span data-ttu-id="f051a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f051a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f051a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f051a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f051a-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f051a-114">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f051a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f051a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f051a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f051a-116">Not supported.</span></span>    |
|<span data-ttu-id="f051a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f051a-117">Application</span></span> | <span data-ttu-id="f051a-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f051a-118">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f051a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f051a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/pages/{page-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="f051a-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="f051a-120">Optional request headers</span></span>

| <span data-ttu-id="f051a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f051a-121">Name</span></span>       | <span data-ttu-id="f051a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f051a-122">Value</span></span> | <span data-ttu-id="f051a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f051a-123">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="f051a-124">_if-match_</span><span class="sxs-lookup"><span data-stu-id="f051a-124">_if-match_</span></span> | <span data-ttu-id="f051a-125">etag</span><span class="sxs-lookup"><span data-stu-id="f051a-125">etag</span></span>  | <span data-ttu-id="f051a-126">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` será exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="f051a-126">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="f051a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f051a-127">Request body</span></span>

<span data-ttu-id="f051a-128">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="f051a-128">Do not supply a request body with this method.</span></span>
<!-- TODO: should we provide a URL to recover/undelete the file, if one exists? -->

## <a name="response"></a><span data-ttu-id="f051a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f051a-129">Response</span></span>

<span data-ttu-id="f051a-130">Se bem sucedido, esta chamada `204 No Content` retorna uma resposta para indicar que o recurso foi excluído e não houve nada para retornar.</span><span class="sxs-lookup"><span data-stu-id="f051a-130">If successful, this call returns a `204 No Content` response to indicate that the resource was deleted and there was nothing to return.</span></span>

## <a name="example"></a><span data-ttu-id="f051a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f051a-131">Example</span></span>

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a><span data-ttu-id="f051a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f051a-132">Request</span></span>

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a><span data-ttu-id="f051a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f051a-133">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Delete a page in the SitePages list in a site.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Delete",
  "suppressions": []
}
-->
