---
title: Restaura uma versão anterior de um ListItem
description: Restaura uma versão anterior de um ListItem para ser a versão atual. Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do item.
ms.openlocfilehash: f8dc4196c40c51287e93aaa667c325e8d4f6dcfb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005214"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="766bb-104">Restaura uma versão anterior de um ListItem</span><span class="sxs-lookup"><span data-stu-id="766bb-104">Restore a previous version of a ListItem</span></span>

<span data-ttu-id="766bb-105">Restaura uma versão anterior de um ListItem para ser a versão atual.</span><span class="sxs-lookup"><span data-stu-id="766bb-105">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="766bb-106">Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do item.</span><span class="sxs-lookup"><span data-stu-id="766bb-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="766bb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="766bb-107">Permissions</span></span>

<span data-ttu-id="766bb-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="766bb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="766bb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="766bb-110">Permission type</span></span>             |         <span data-ttu-id="766bb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="766bb-111">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="766bb-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="766bb-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="766bb-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="766bb-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="766bb-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="766bb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="766bb-115">n/d</span><span class="sxs-lookup"><span data-stu-id="766bb-115">n/a</span></span>                                                          |
| <span data-ttu-id="766bb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="766bb-116">Application</span></span>                            | <span data-ttu-id="766bb-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="766bb-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="766bb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="766bb-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="766bb-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="766bb-119">Request body</span></span>

<span data-ttu-id="766bb-120">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="766bb-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="766bb-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="766bb-121">Example</span></span>

<span data-ttu-id="766bb-122">Este exemplo restaura uma versão de um listItem identificado por `{item-id}` e `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="766bb-122">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite sites.readwrite.all", "target": "action", "tags": "service.graph service.sharepoint" } -->

```http
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="766bb-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="766bb-123">Response</span></span>

<span data-ttu-id="766bb-124">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="766bb-124">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
