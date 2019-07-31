---
author: rahmit
description: Remove um sitePage da lista de páginas do site em um site.
ms.date: 05/07/2018
title: Excluir uma página de um site do SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: bdf3dacabb99d5dfcfe47dcb954ff1cfd0b62ccb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977857"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a><span data-ttu-id="7f2a3-103">Excluir página da lista de páginas do site de um site</span><span class="sxs-lookup"><span data-stu-id="7f2a3-103">Delete page from the site pages list of a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f2a3-104">Remove um [sitePage][] da [lista][] de páginas do site em um [site][].</span><span class="sxs-lookup"><span data-stu-id="7f2a3-104">Removes a [sitePage][] from the site pages [list][] in a [site][].</span></span>

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="7f2a3-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="7f2a3-108">Permissions</span></span>

<span data-ttu-id="7f2a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f2a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="7f2a3-111">**Observação:** Para excluir um item, o usuário deve ter concedido o acesso de gravação do aplicativo ao item a ser excluído.</span><span class="sxs-lookup"><span data-stu-id="7f2a3-111">**Note:** To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

|<span data-ttu-id="7f2a3-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f2a3-112">Permission type</span></span>      | <span data-ttu-id="7f2a3-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f2a3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f2a3-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f2a3-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7f2a3-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f2a3-115">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7f2a3-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f2a3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f2a3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f2a3-117">Not supported.</span></span>    |
|<span data-ttu-id="7f2a3-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f2a3-118">Application</span></span> | <span data-ttu-id="7f2a3-119">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f2a3-119">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f2a3-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f2a3-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/pages/{page-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="7f2a3-121">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="7f2a3-121">Optional request headers</span></span>

| <span data-ttu-id="7f2a3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="7f2a3-122">Name</span></span>       | <span data-ttu-id="7f2a3-123">Valor</span><span class="sxs-lookup"><span data-stu-id="7f2a3-123">Value</span></span> | <span data-ttu-id="7f2a3-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f2a3-124">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="7f2a3-125">_if-match_</span><span class="sxs-lookup"><span data-stu-id="7f2a3-125">_if-match_</span></span> | <span data-ttu-id="7f2a3-126">etag</span><span class="sxs-lookup"><span data-stu-id="7f2a3-126">etag</span></span>  | <span data-ttu-id="7f2a3-127">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` será exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="7f2a3-127">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="7f2a3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f2a3-128">Request body</span></span>

<span data-ttu-id="7f2a3-129">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="7f2a3-129">Do not supply a request body with this method.</span></span>
<!-- TODO: should we provide a URL to recover/undelete the file, if one exists? -->

## <a name="response"></a><span data-ttu-id="7f2a3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f2a3-130">Response</span></span>

<span data-ttu-id="7f2a3-131">Se bem sucedido, esta chamada `204 No Content` retorna uma resposta para indicar que o recurso foi excluído e não houve nada para retornar.</span><span class="sxs-lookup"><span data-stu-id="7f2a3-131">If successful, this call returns a `204 No Content` response to indicate that the resource was deleted and there was nothing to return.</span></span>

## <a name="example"></a><span data-ttu-id="7f2a3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f2a3-132">Example</span></span>

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a><span data-ttu-id="7f2a3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f2a3-133">Request</span></span>

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a><span data-ttu-id="7f2a3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f2a3-134">Response</span></span>

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
