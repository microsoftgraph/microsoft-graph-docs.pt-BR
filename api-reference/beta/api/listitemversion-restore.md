---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Restaurar uma versão anterior de um item de lista do SharePoint
ms.openlocfilehash: 7c09f618bec1f6d20993e1b6cf974b8a53a3d3e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033756"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="0029b-102">Restaura uma versão anterior de um ListItem</span><span class="sxs-lookup"><span data-stu-id="0029b-102">Restore a previous version of a ListItem</span></span>

> <span data-ttu-id="0029b-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0029b-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0029b-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0029b-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0029b-105">Restaura uma versão anterior de um ListItem para ser a versão atual.</span><span class="sxs-lookup"><span data-stu-id="0029b-105">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="0029b-106">Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do item.</span><span class="sxs-lookup"><span data-stu-id="0029b-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="0029b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0029b-107">Permissions</span></span>

<span data-ttu-id="0029b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0029b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="0029b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0029b-110">Permission type</span></span>             |         <span data-ttu-id="0029b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0029b-111">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="0029b-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0029b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0029b-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="0029b-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="0029b-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0029b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0029b-115">n/d</span><span class="sxs-lookup"><span data-stu-id="0029b-115">n/a</span></span>                                                          |
| <span data-ttu-id="0029b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0029b-116">Application</span></span>                            | <span data-ttu-id="0029b-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="0029b-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0029b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0029b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="0029b-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0029b-119">Request body</span></span>

<span data-ttu-id="0029b-120">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0029b-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="0029b-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0029b-121">Example</span></span>

<span data-ttu-id="0029b-122">Este exemplo restaura uma versão de um listItem identificado por `{item-id}` e `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="0029b-122">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="0029b-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="0029b-123">Response</span></span>

<span data-ttu-id="0029b-124">Se tiver êxito, a chamada API retorna um código `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="0029b-124">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
