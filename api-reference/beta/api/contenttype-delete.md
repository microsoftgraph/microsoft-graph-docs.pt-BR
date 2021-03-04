---
author: swapnil1993
title: Excluir contentType
description: Exclua um tipo de conteúdo de uma lista do sharepoint ou de um site.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 8c27cfd2e16fc4c3bd7fade3f5546c08951f38c5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445875"
---
# <a name="delete-contenttype"></a><span data-ttu-id="048a6-103">Excluir contentType</span><span class="sxs-lookup"><span data-stu-id="048a6-103">Delete contentType</span></span>
<span data-ttu-id="048a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="048a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="048a6-105">Remover um [tipo de conteúdo][contentType] de uma [lista][] ou de um [site][].</span><span class="sxs-lookup"><span data-stu-id="048a6-105">Remove a [content type][contentType] from a [list][] or a [site][].</span></span>


## <a name="permissions"></a><span data-ttu-id="048a6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="048a6-106">Permissions</span></span>
<span data-ttu-id="048a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="048a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="048a6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="048a6-109">Permission type</span></span>      | <span data-ttu-id="048a6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="048a6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="048a6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="048a6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="048a6-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="048a6-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="048a6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="048a6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="048a6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="048a6-114">Not supported.</span></span>    |
|<span data-ttu-id="048a6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="048a6-115">Application</span></span> | <span data-ttu-id="048a6-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="048a6-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="048a6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="048a6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/contentTypes/{contentType-id}
DELETE /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}
```

## <a name="request-headers"></a><span data-ttu-id="048a6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="048a6-118">Request headers</span></span>
|<span data-ttu-id="048a6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="048a6-119">Name</span></span>|<span data-ttu-id="048a6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="048a6-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="048a6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="048a6-121">Authorization</span></span>|<span data-ttu-id="048a6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="048a6-p102">Bearer {token}. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="048a6-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="048a6-124">Request body</span></span>

<span data-ttu-id="048a6-125">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="048a6-125">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="048a6-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="048a6-126">Response</span></span>

<span data-ttu-id="048a6-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="048a6-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="048a6-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="048a6-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="048a6-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="048a6-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contenttype"
}
-->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}
```

### <a name="response"></a><span data-ttu-id="048a6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="048a6-130">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 No Content
```

[list]: ../resources/list.md
[contentType]: ../resources/contentType.md
[site]: ../resources/site.md
