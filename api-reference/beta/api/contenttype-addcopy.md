---
author: swapnil1993
title: 'contentType: addCopy'
description: Adicione uma cópia de um tipo de conteúdo de site a uma lista.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 955afab160cb5c927771db4132ec208b85e80b2a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445883"
---
# <a name="contenttype-addcopy"></a><span data-ttu-id="9cc02-103">contentType: addCopy</span><span class="sxs-lookup"><span data-stu-id="9cc02-103">contentType: addCopy</span></span>
<span data-ttu-id="9cc02-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cc02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="9cc02-105">Adicione uma cópia de um [tipo de conteúdo de site][site] [][contentType] a uma [lista][list].</span><span class="sxs-lookup"><span data-stu-id="9cc02-105">Add a copy of a [site][site] [content type][contentType] to a [list][list].</span></span>
 
  

## <a name="permissions"></a><span data-ttu-id="9cc02-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9cc02-106">Permissions</span></span>  

<span data-ttu-id="9cc02-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9cc02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="9cc02-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9cc02-109">Permission type</span></span> | <span data-ttu-id="9cc02-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9cc02-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9cc02-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9cc02-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9cc02-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="9cc02-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="9cc02-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9cc02-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cc02-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cc02-114">Not supported.</span></span> |
|<span data-ttu-id="9cc02-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9cc02-115">Application</span></span> | <span data-ttu-id="9cc02-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="9cc02-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="9cc02-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9cc02-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http

POST /sites/{site-id}/lists/{list-id}/contentTypes/addCopy
```

## <a name="request-headers"></a><span data-ttu-id="9cc02-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9cc02-118">Request headers</span></span>
|<span data-ttu-id="9cc02-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9cc02-119">Name</span></span>|<span data-ttu-id="9cc02-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cc02-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9cc02-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9cc02-121">Authorization</span></span>|<span data-ttu-id="9cc02-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cc02-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9cc02-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9cc02-124">Content-Type</span></span>|<span data-ttu-id="9cc02-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cc02-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cc02-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9cc02-127">Request body</span></span>
<span data-ttu-id="9cc02-128">No corpo da solicitação, fornece uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="9cc02-128">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="9cc02-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="9cc02-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9cc02-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9cc02-130">Parameter</span></span>|<span data-ttu-id="9cc02-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cc02-131">Type</span></span>|<span data-ttu-id="9cc02-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cc02-132">Description</span></span>|
|-|-|-|
|<span data-ttu-id="9cc02-133">contentType</span><span class="sxs-lookup"><span data-stu-id="9cc02-133">contentType</span></span>| <span data-ttu-id="9cc02-134">string</span><span class="sxs-lookup"><span data-stu-id="9cc02-134">string</span></span> | <span data-ttu-id="9cc02-135">URL canônica para o tipo de conteúdo do site que será copiado para a lista.</span><span class="sxs-lookup"><span data-stu-id="9cc02-135">Canonical URL to the site content type that will be copied to the list.</span></span> <span data-ttu-id="9cc02-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cc02-136">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="9cc02-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cc02-137">Response</span></span>

<span data-ttu-id="9cc02-138">Se tiver êxito, essa chamada retornará uma `204 No Content` resposta.</span><span class="sxs-lookup"><span data-stu-id="9cc02-138">If successful, this call returns a `204 No Content` response.</span></span>

## <a name="example"></a><span data-ttu-id="9cc02-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9cc02-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="9cc02-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9cc02-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "contenttype_addcopy"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/id/lists/{list-id}/contentTypes/addCopy
Content-Type: application/json

{
  "contentType": "https://graph.microsoft.com/beta/sites/id/contentTypes/0x0101"
}
```



### <a name="response"></a><span data-ttu-id="9cc02-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cc02-141">Response</span></span>


<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content

```

[site]: ../resources/site.md
[list]: ../resources/list.md
[contentType]: ../resources/contentType.md
