---
author: rahmit
ms.author: rahmit
ms.date: 05/07/2018
title: Excluir uma página de um site do SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f855942288556fdf07e2b3af78408976c34eb052
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513022"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a><span data-ttu-id="429bd-102">Excluir página na lista de páginas de site de um site</span><span class="sxs-lookup"><span data-stu-id="429bd-102">Delete page from the site pages list of a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="429bd-103">Remove um [sitePage][] de páginas do site [lista][] em um [site][].</span><span class="sxs-lookup"><span data-stu-id="429bd-103">Removes a [sitePage][] from the site pages [list][] in a [site][].</span></span>

[sitePage]: ../resources/sitepage.md
[lista]: ../resources/list.md
[list]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="429bd-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="429bd-107">Permissions</span></span>

<span data-ttu-id="429bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="429bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="429bd-110">**Observação:** Para excluir um item, o usuário deve ter concedido ao acesso de gravação do aplicativo até o item a ser excluído.</span><span class="sxs-lookup"><span data-stu-id="429bd-110">**Note:** To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

|<span data-ttu-id="429bd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="429bd-111">Permission type</span></span>      | <span data-ttu-id="429bd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="429bd-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="429bd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="429bd-113">Delegated (work or school account)</span></span> | <span data-ttu-id="429bd-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="429bd-114">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="429bd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="429bd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="429bd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="429bd-116">Not supported.</span></span>    |
|<span data-ttu-id="429bd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="429bd-117">Application</span></span> | <span data-ttu-id="429bd-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="429bd-118">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="429bd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="429bd-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/pages/{page-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="429bd-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="429bd-120">Optional request headers</span></span>

| <span data-ttu-id="429bd-121">Nome</span><span class="sxs-lookup"><span data-stu-id="429bd-121">Name</span></span>       | <span data-ttu-id="429bd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="429bd-122">Value</span></span> | <span data-ttu-id="429bd-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="429bd-123">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="429bd-124">_if-match_</span><span class="sxs-lookup"><span data-stu-id="429bd-124">_if-match_</span></span> | <span data-ttu-id="429bd-125">etag</span><span class="sxs-lookup"><span data-stu-id="429bd-125">etag</span></span>  | <span data-ttu-id="429bd-126">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` será exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="429bd-126">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="429bd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="429bd-127">Request body</span></span>

<span data-ttu-id="429bd-128">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="429bd-128">Do not supply a request body with this method.</span></span>
<!-- TODO: should we provide a URL to recover/undelete the file, if one exists? -->

## <a name="response"></a><span data-ttu-id="429bd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="429bd-129">Response</span></span>

<span data-ttu-id="429bd-130">Se tiver êxito, essa chamada retornará um `204 No Content` resposta para indicar que o recurso foi excluído e não houve nothing para retornar.</span><span class="sxs-lookup"><span data-stu-id="429bd-130">If successful, this call returns a `204 No Content` response to indicate that the resource was deleted and there was nothing to return.</span></span>

## <a name="example"></a><span data-ttu-id="429bd-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="429bd-131">Example</span></span>

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a><span data-ttu-id="429bd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="429bd-132">Request</span></span>

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a><span data-ttu-id="429bd-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="429bd-133">Response</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/sitepage-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
