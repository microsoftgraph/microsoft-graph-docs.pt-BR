---
author: rahmit
ms.author: rahmit
ms.date: 05/07/2018
title: Excluir uma página de um site do SharePoint
localization_priority: Normal
ms.openlocfilehash: 1089bd904167f4c86ee1f6becede2824a2b6f2f9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815110"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a><span data-ttu-id="59f17-102">Excluir página na lista de páginas de site de um site</span><span class="sxs-lookup"><span data-stu-id="59f17-102">Delete page from the site pages list of a site</span></span>

> <span data-ttu-id="59f17-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="59f17-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59f17-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="59f17-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="59f17-105">Remove um [sitePage][] de páginas do site [lista][] em um [site][].</span><span class="sxs-lookup"><span data-stu-id="59f17-105">Removes a [sitePage][] from the site pages [list][] in a [site][].</span></span>

[sitePage]: ../resources/sitepage.md
[lista]: ../resources/list.md
[list]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="59f17-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="59f17-109">Permissions</span></span>

<span data-ttu-id="59f17-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59f17-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="59f17-112">**Observação:** Para excluir um item, o usuário deve ter concedido ao acesso de gravação do aplicativo até o item a ser excluído.</span><span class="sxs-lookup"><span data-stu-id="59f17-112">**Note:** To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

|<span data-ttu-id="59f17-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59f17-113">Permission type</span></span>      | <span data-ttu-id="59f17-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59f17-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59f17-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59f17-115">Delegated (work or school account)</span></span> | <span data-ttu-id="59f17-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59f17-116">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="59f17-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59f17-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59f17-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59f17-118">Not supported.</span></span>    |
|<span data-ttu-id="59f17-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59f17-119">Application</span></span> | <span data-ttu-id="59f17-120">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59f17-120">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="59f17-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59f17-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/pages/{page-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="59f17-122">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="59f17-122">Optional request headers</span></span>

| <span data-ttu-id="59f17-123">Nome</span><span class="sxs-lookup"><span data-stu-id="59f17-123">Name</span></span>       | <span data-ttu-id="59f17-124">Valor</span><span class="sxs-lookup"><span data-stu-id="59f17-124">Value</span></span> | <span data-ttu-id="59f17-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="59f17-125">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="59f17-126">_if-match_</span><span class="sxs-lookup"><span data-stu-id="59f17-126">_if-match_</span></span> | <span data-ttu-id="59f17-127">etag</span><span class="sxs-lookup"><span data-stu-id="59f17-127">etag</span></span>  | <span data-ttu-id="59f17-128">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` será exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="59f17-128">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="59f17-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59f17-129">Request body</span></span>

<span data-ttu-id="59f17-130">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="59f17-130">Do not supply a request body with this method.</span></span>
<!-- TODO: should we provide a URL to recover/undelete the file, if one exists? -->

## <a name="response"></a><span data-ttu-id="59f17-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="59f17-131">Response</span></span>

<span data-ttu-id="59f17-132">Se tiver êxito, essa chamada retornará um `204 No Content` resposta para indicar que o recurso foi excluído e não houve nothing para retornar.</span><span class="sxs-lookup"><span data-stu-id="59f17-132">If successful, this call returns a `204 No Content` response to indicate that the resource was deleted and there was nothing to return.</span></span>

## <a name="example"></a><span data-ttu-id="59f17-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59f17-133">Example</span></span>

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a><span data-ttu-id="59f17-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59f17-134">Request</span></span>

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a><span data-ttu-id="59f17-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="59f17-135">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Delete a page in the SitePages list in a site.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Delete"
} -->
