---
author: swapnil1993
title: Excluir columnDefinition
description: Exclua uma coluna de um tipo de conteúdo.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: fb5df6389c4723cf48185a74f72c1009a3ac031b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445876"
---
# <a name="delete-columndefinition"></a><span data-ttu-id="518f9-103">Excluir columnDefinition</span><span class="sxs-lookup"><span data-stu-id="518f9-103">Delete columnDefinition</span></span>
<span data-ttu-id="518f9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="518f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="518f9-105">Remova uma [coluna de][columndefinition] uma [lista ou][] de um tipo [de conteúdo][] [de site.][contentType]</span><span class="sxs-lookup"><span data-stu-id="518f9-105">Remove a [column][columndefinition] from a [list][] or a [site][] [content type][contentType].</span></span>


## <a name="permissions"></a><span data-ttu-id="518f9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="518f9-106">Permissions</span></span>
<span data-ttu-id="518f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="518f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="518f9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="518f9-109">Permission type</span></span>      | <span data-ttu-id="518f9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="518f9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="518f9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="518f9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="518f9-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="518f9-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="518f9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="518f9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="518f9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="518f9-114">Not supported.</span></span>    |
|<span data-ttu-id="518f9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="518f9-115">Application</span></span> | <span data-ttu-id="518f9-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="518f9-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="518f9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="518f9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
DELETE /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns/{column-id}
```
## <a name="request-headers"></a><span data-ttu-id="518f9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="518f9-118">Request headers</span></span>
|<span data-ttu-id="518f9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="518f9-119">Name</span></span>|<span data-ttu-id="518f9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="518f9-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="518f9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="518f9-121">Authorization</span></span>|<span data-ttu-id="518f9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="518f9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="518f9-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="518f9-124">Request body</span></span>
<span data-ttu-id="518f9-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="518f9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="518f9-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="518f9-126">Response</span></span>

<span data-ttu-id="518f9-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="518f9-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="518f9-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="518f9-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="518f9-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="518f9-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_columns_from_contenttype"
}
-->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
```

### <a name="response"></a><span data-ttu-id="518f9-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="518f9-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
```http
HTTP/1.1 204 No Content
```

[list]: ../resources/list.md
[columndefinition]: ../resources/columndefinition.md
[contentType]: ../resources/contentType.md
[site]: ../resources/site.md
