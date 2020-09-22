---
author: rahmit
description: Remove um sitePage da lista de páginas do site em um site.
ms.date: 05/07/2018
title: Excluir uma página de um site do SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: d573553ee87b70adfd1f2cde575ce6182dedf8b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044484"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a><span data-ttu-id="ee163-103">Excluir página da lista de páginas do site de um site</span><span class="sxs-lookup"><span data-stu-id="ee163-103">Delete page from the site pages list of a site</span></span>

<span data-ttu-id="ee163-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee163-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee163-105">Remove um [sitePage][] da [lista][] de páginas do site em um [site][].</span><span class="sxs-lookup"><span data-stu-id="ee163-105">Removes a [sitePage][] from the site pages [list][] in a [site][].</span></span>

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="ee163-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee163-109">Permissions</span></span>

<span data-ttu-id="ee163-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee163-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="ee163-112">**Observação:** Para excluir um item, o usuário deve ter concedido o acesso de gravação do aplicativo ao item a ser excluído.</span><span class="sxs-lookup"><span data-stu-id="ee163-112">**Note:** To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

|<span data-ttu-id="ee163-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee163-113">Permission type</span></span>      | <span data-ttu-id="ee163-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee163-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee163-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee163-115">Delegated (work or school account)</span></span> | <span data-ttu-id="ee163-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee163-116">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ee163-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee163-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee163-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee163-118">Not supported.</span></span>    |
|<span data-ttu-id="ee163-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee163-119">Application</span></span> | <span data-ttu-id="ee163-120">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee163-120">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee163-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee163-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/pages/{page-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="ee163-122">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="ee163-122">Optional request headers</span></span>

| <span data-ttu-id="ee163-123">Nome</span><span class="sxs-lookup"><span data-stu-id="ee163-123">Name</span></span>       | <span data-ttu-id="ee163-124">Valor</span><span class="sxs-lookup"><span data-stu-id="ee163-124">Value</span></span> | <span data-ttu-id="ee163-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee163-125">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="ee163-126">_if-match_</span><span class="sxs-lookup"><span data-stu-id="ee163-126">_if-match_</span></span> | <span data-ttu-id="ee163-127">etag</span><span class="sxs-lookup"><span data-stu-id="ee163-127">etag</span></span>  | <span data-ttu-id="ee163-128">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` será exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="ee163-128">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="ee163-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee163-129">Request body</span></span>

<span data-ttu-id="ee163-130">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="ee163-130">Do not supply a request body with this method.</span></span>
<!-- TODO: should we provide a URL to recover/undelete the file, if one exists? -->

## <a name="response"></a><span data-ttu-id="ee163-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee163-131">Response</span></span>

<span data-ttu-id="ee163-132">Se bem sucedido, esta chamada retorna uma `204 No Content` resposta para indicar que o recurso foi excluído e não houve nada para retornar.</span><span class="sxs-lookup"><span data-stu-id="ee163-132">If successful, this call returns a `204 No Content` response to indicate that the resource was deleted and there was nothing to return.</span></span>

## <a name="example"></a><span data-ttu-id="ee163-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee163-133">Example</span></span>

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a><span data-ttu-id="ee163-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee163-134">Request</span></span>

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a><span data-ttu-id="ee163-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee163-135">Response</span></span>

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


