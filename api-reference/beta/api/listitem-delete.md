---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Excluir uma entrada de uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 13c6504753eb5987db8c0282ef2f59bca72a8d43
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530143"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="093d0-102">Excluir um item de uma lista.</span><span class="sxs-lookup"><span data-stu-id="093d0-102">Delete an item from a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="093d0-103">Remover um item de uma [list][].</span><span class="sxs-lookup"><span data-stu-id="093d0-103">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="093d0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="093d0-105">Permissions</span></span>

<span data-ttu-id="093d0-106">Para excluir um item, o usuário deve ter concedido o acesso de gravação do aplicativo para o item a ser excluído.</span><span class="sxs-lookup"><span data-stu-id="093d0-106">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="093d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="093d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="093d0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="093d0-109">Permission type</span></span>      | <span data-ttu-id="093d0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="093d0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="093d0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="093d0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="093d0-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="093d0-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="093d0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="093d0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="093d0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="093d0-114">Not supported.</span></span>    |
|<span data-ttu-id="093d0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="093d0-115">Application</span></span> | <span data-ttu-id="093d0-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="093d0-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="093d0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="093d0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="093d0-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="093d0-118">Optional request headers</span></span>

| <span data-ttu-id="093d0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="093d0-119">Name</span></span>       | <span data-ttu-id="093d0-120">Valor</span><span class="sxs-lookup"><span data-stu-id="093d0-120">Value</span></span> | <span data-ttu-id="093d0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="093d0-121">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="093d0-122">_if-match_</span><span class="sxs-lookup"><span data-stu-id="093d0-122">_if-match_</span></span> | <span data-ttu-id="093d0-123">etag</span><span class="sxs-lookup"><span data-stu-id="093d0-123">etag</span></span>  | <span data-ttu-id="093d0-124">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` será exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="093d0-124">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="093d0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="093d0-125">Request body</span></span>

<span data-ttu-id="093d0-126">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="093d0-126">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="093d0-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="093d0-127">Example</span></span>

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="093d0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="093d0-128">Response</span></span>

<span data-ttu-id="093d0-129">Se bem sucedida, esta chamada retorna uma resposta `204 No Content` para indicar que o recurso foi excluído e que não havia nada a retornar.</span><span class="sxs-lookup"><span data-stu-id="093d0-129">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Delete",
  "suppressions": [
    "Error: /api-reference/beta/api/listitem-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
