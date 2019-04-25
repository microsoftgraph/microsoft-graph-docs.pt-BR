---
title: Restaura uma versão anterior de um ListItem
description: Restaura uma versão anterior de um ListItem para ser a versão atual. Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do item.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3ba63f56838d07a0031baf613dec8e0847aaf2e6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542057"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="d885e-104">Restaura uma versão anterior de um ListItem</span><span class="sxs-lookup"><span data-stu-id="d885e-104">Restore a previous version of a ListItem</span></span>

<span data-ttu-id="d885e-105">Restaura uma versão anterior de um ListItem para ser a versão atual.</span><span class="sxs-lookup"><span data-stu-id="d885e-105">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="d885e-106">Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do item.</span><span class="sxs-lookup"><span data-stu-id="d885e-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="d885e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d885e-107">Permissions</span></span>

<span data-ttu-id="d885e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d885e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="d885e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d885e-110">Permission type</span></span>             |         <span data-ttu-id="d885e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d885e-111">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="d885e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d885e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d885e-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="d885e-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="d885e-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d885e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d885e-115">n/d</span><span class="sxs-lookup"><span data-stu-id="d885e-115">n/a</span></span>                                                          |
| <span data-ttu-id="d885e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d885e-116">Application</span></span>                            | <span data-ttu-id="d885e-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="d885e-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d885e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d885e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="d885e-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d885e-119">Request body</span></span>

<span data-ttu-id="d885e-120">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d885e-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="d885e-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d885e-121">Example</span></span>

<span data-ttu-id="d885e-122">Este exemplo restaura uma versão de um listItem identificado por `{item-id}` e `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="d885e-122">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite sites.readwrite.all", "target": "action", "tags": "service.graph service.sharepoint" } -->

```http
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="d885e-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="d885e-123">Response</span></span>

<span data-ttu-id="d885e-124">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d885e-124">If successful, the API call returns a `204 No Content`.</span></span>

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
