---
author: swapnil1993
title: Obter columnDefinition
description: " Obter uma coluna de tipo de conteúdo."
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 8fa2da27e03ad5d174d1c6bcc19b7b82201fb581
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445872"
---
# <a name="get-columndefinition"></a><span data-ttu-id="aae6c-103">Obter columnDefinition</span><span class="sxs-lookup"><span data-stu-id="aae6c-103">Get columnDefinition</span></span>
<span data-ttu-id="aae6c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aae6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="aae6c-105">Recupere os metadados de uma [coluna contentType][] [.][columnDefinition]</span><span class="sxs-lookup"><span data-stu-id="aae6c-105">Retrieve the metadata for a [contentType][] [column][columnDefinition].</span></span>

  

## <a name="permissions"></a><span data-ttu-id="aae6c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="aae6c-106">Permissions</span></span>

  

<span data-ttu-id="aae6c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aae6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="aae6c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aae6c-109">Permission type</span></span> | <span data-ttu-id="aae6c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aae6c-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aae6c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aae6c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aae6c-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="aae6c-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="aae6c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aae6c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aae6c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aae6c-114">Not supported.</span></span> |
|<span data-ttu-id="aae6c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aae6c-115">Application</span></span> | <span data-ttu-id="aae6c-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="aae6c-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |

  

## <a name="http-request"></a><span data-ttu-id="aae6c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aae6c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http

GET /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
GET /sites/{site-id}/lists/{list-id}//contentTypes/{contentType-id}/columns/{column-id}
```

## <a name="request-headers"></a><span data-ttu-id="aae6c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aae6c-118">Request headers</span></span>
|<span data-ttu-id="aae6c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="aae6c-119">Name</span></span>|<span data-ttu-id="aae6c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="aae6c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="aae6c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="aae6c-121">Authorization</span></span>|<span data-ttu-id="aae6c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aae6c-p102">Bearer {token}. Required.</span></span>|  

## <a name="request-body"></a><span data-ttu-id="aae6c-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aae6c-124">Request body</span></span>

  

<span data-ttu-id="aae6c-125">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="aae6c-125">Do not supply a request body with this method.</span></span>

  

## <a name="example"></a><span data-ttu-id="aae6c-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aae6c-126">Example</span></span>

  

### <a name="request"></a><span data-ttu-id="aae6c-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aae6c-127">Request</span></span>

  

<!-- { "blockType": "request", "name": "get_column_from_contenttype" } -->

  

```http
GET /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
```

  

#### <a name="response"></a><span data-ttu-id="aae6c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="aae6c-128">Response</span></span>

  

<!-- { "blockType": "response", "@type": "microsoft.graph.columnDefinition", "truncated": true } -->

  

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "",
  "displayName": "Title",
  "hidden": false,
  "id": "99ddcf45-e2f7-4f17-82b0-6fba34445103",
  "indexed": false,
  "name": "Title",
  "readOnly": false,
  "required": false,
  "text": {
    "allowMultipleLines": false,
    "appendChangesToExistingText": false,
    "linesForEditing": 0,
    "maxLength": 255
  }
}
```

  

[columnDefinition]: ../resources/columnDefinition.md

[list]: ../resources/list.md

[site]: ../resources/site.md

[contentType]: ../resources/contentType.md
  
