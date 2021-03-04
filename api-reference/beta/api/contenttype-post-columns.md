---
author: swapnil1993
ms.date: 08/30/2020
title: Criar columnDefinition
description: Adicione coluna a um tipo de conteúdo.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 071a855c79c055179022157b991b4a9f2789cad1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445863"
---
# <a name="create-columndefinition"></a><span data-ttu-id="2afee-103">Criar columnDefinition</span><span class="sxs-lookup"><span data-stu-id="2afee-103">Create columnDefinition</span></span>
<span data-ttu-id="2afee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2afee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="2afee-105">Adiciona coluna de coluna de site ou [lista][existenteDefinition] a um [tipo de][conteúdo contentType].</span><span class="sxs-lookup"><span data-stu-id="2afee-105">Adds existing site or list [column][columnDefinition] to a [content type][contentType].</span></span>

## <a name="permissions"></a><span data-ttu-id="2afee-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2afee-106">Permissions</span></span>

<span data-ttu-id="2afee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2afee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/concepts/permissions_reference.md).</span></span>

  

|<span data-ttu-id="2afee-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2afee-109">Permission type</span></span> | <span data-ttu-id="2afee-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2afee-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2afee-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2afee-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2afee-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="2afee-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
|<span data-ttu-id="2afee-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2afee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2afee-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2afee-114">Not supported.</span></span> |
|<span data-ttu-id="2afee-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2afee-115">Application</span></span> | <span data-ttu-id="2afee-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="2afee-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="2afee-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2afee-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /sites/{site-id}/contentTypes/{contentType-id}/columns
POST /sites/{site-id}/lists/{list-id}//contentTypes/{contentType-id}/columns
```

## <a name="request-body"></a><span data-ttu-id="2afee-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2afee-118">Request body</span></span>

<span data-ttu-id="2afee-119">No corpo da solicitação, fornece uma representação JSON do [recurso columnDefinition][] a adicionar.</span><span class="sxs-lookup"><span data-stu-id="2afee-119">In the request body, supply a JSON representation of the [columnDefinition][] resource to add.</span></span>  

## <a name="response"></a><span data-ttu-id="2afee-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="2afee-120">Response</span></span>

<span data-ttu-id="2afee-121">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [contentType][] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2afee-121">If successful, this method returns a `200 OK` response code and [contentType][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2afee-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2afee-122">Example</span></span>

### <a name="request"></a><span data-ttu-id="2afee-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2afee-123">Request</span></span>
<!-- { "blockType": "request" } -->
```http
POST https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}/columns
Content-Type: application/json

{
    "sourceColumn@odata.bind": "https://graph.microsoft.com/beta/sites/root/columns/99ddcf45-e2f7-4f17-82b0-6fba34445103",
}
```

### <a name="response"></a><span data-ttu-id="2afee-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="2afee-124">Response</span></span>

<span data-ttu-id="2afee-125">A resposta retorna uma lista de todas as colunas adicionadas a um tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="2afee-125">The response returns a list of all columns added to a content type.</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.columnDefinition", "truncated": true, "scopes": "sites.readwrite.all" } -->

  

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "",
  "displayName": "Title",
  "enforceUniqueValues": false,
  "hidden": false,
  "id": "99ddcf45-e2f7-4f17-82b0-6fba34445103",
  "indexed": false,
  "name": "Title",
  "text": {
    "allowMultipleLines": false,
    "appendChangesToExistingText": false,
    "linesForEditing": 0,
    "maxLength": 255
  }
}

```

  

[columnDefinition]: ../resources/columnDefinition.md
[contentType]: ../resources/contentType.md
  

