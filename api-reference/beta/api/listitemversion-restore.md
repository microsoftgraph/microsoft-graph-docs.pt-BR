---
author: JeremyKelley
description: Restaura uma versão anterior de um ListItem para ser a versão atual. Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do item.
ms.date: 09/10/2017
title: Restaurar uma versão anterior de um item de lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 25e244c9dee5adb3b756f2c4bae38b292dc16679
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457087"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="6ddc1-104">Restaura uma versão anterior de um ListItem</span><span class="sxs-lookup"><span data-stu-id="6ddc1-104">Restore a previous version of a ListItem</span></span>

<span data-ttu-id="6ddc1-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6ddc1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ddc1-106">Restaura uma versão anterior de um ListItem para ser a versão atual.</span><span class="sxs-lookup"><span data-stu-id="6ddc1-106">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="6ddc1-107">Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do item.</span><span class="sxs-lookup"><span data-stu-id="6ddc1-107">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ddc1-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="6ddc1-108">Permissions</span></span>

<span data-ttu-id="6ddc1-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ddc1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="6ddc1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ddc1-111">Permission type</span></span>             |         <span data-ttu-id="6ddc1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6ddc1-112">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="6ddc1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ddc1-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6ddc1-114">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="6ddc1-114">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="6ddc1-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ddc1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ddc1-116">n/d</span><span class="sxs-lookup"><span data-stu-id="6ddc1-116">n/a</span></span>                                                          |
| <span data-ttu-id="6ddc1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ddc1-117">Application</span></span>                            | <span data-ttu-id="6ddc1-118">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="6ddc1-118">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ddc1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ddc1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="6ddc1-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ddc1-120">Request body</span></span>

<span data-ttu-id="6ddc1-121">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ddc1-121">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="6ddc1-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ddc1-122">Example</span></span>

<span data-ttu-id="6ddc1-123">Este exemplo restaura uma versão de um listItem identificado por `{item-id}` e `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="6ddc1-123">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="6ddc1-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ddc1-124">Response</span></span>

<span data-ttu-id="6ddc1-125">Se tiver êxito, a chamada API retorna um código `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="6ddc1-125">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": []
}
-->
