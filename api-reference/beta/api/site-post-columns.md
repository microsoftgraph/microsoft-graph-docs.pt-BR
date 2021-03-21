---
author: swapnil1993
ms.date: 08/30/2020
title: Criar columnDefinition em um site
description: Criar uma coluna de site.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 9198bd0841fde42ef3d96e96db89515341040e9e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965015"
---
# <a name="create-columndefinition-for-a-site"></a><span data-ttu-id="c78cb-103">Criar columnDefinition para um site</span><span class="sxs-lookup"><span data-stu-id="c78cb-103">Create columnDefinition for a site</span></span>
<span data-ttu-id="c78cb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c78cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="c78cb-105">Crie uma coluna para um [site][site] by specifying a [columnDefinition][columnDefinition] .</span><span class="sxs-lookup"><span data-stu-id="c78cb-105">Create a column for a [site][site] by specifying a [columnDefinition][columnDefinition].</span></span>

## <a name="permissions"></a><span data-ttu-id="c78cb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c78cb-106">Permissions</span></span>

<span data-ttu-id="c78cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c78cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/concepts/permissions_reference.md).</span></span>

  

|<span data-ttu-id="c78cb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c78cb-109">Permission type</span></span> | <span data-ttu-id="c78cb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c78cb-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c78cb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c78cb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c78cb-112">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="c78cb-112">Sites.Manage.All, Sites.FullControl.All</span></span> |
|<span data-ttu-id="c78cb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c78cb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c78cb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c78cb-114">Not supported.</span></span> |
|<span data-ttu-id="c78cb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c78cb-115">Application</span></span> | <span data-ttu-id="c78cb-116">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="c78cb-116">Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="c78cb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c78cb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /sites/{site-id}/columns
```

## <a name="request-body"></a><span data-ttu-id="c78cb-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c78cb-118">Request body</span></span>

<span data-ttu-id="c78cb-119">No corpo da solicitação, fornece uma representação JSON do [recurso columnDefinition][] a adicionar.</span><span class="sxs-lookup"><span data-stu-id="c78cb-119">In the request body, supply a JSON representation of the [columnDefinition][] resource to add.</span></span>  

## <a name="response"></a><span data-ttu-id="c78cb-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="c78cb-120">Response</span></span>

<span data-ttu-id="c78cb-121">Se tiver êxito, este método retornará um código de resposta e `201 Created` [um objeto columnDefinition][] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c78cb-121">If successful, this method returns a `201 Created` response code and [columnDefinition][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c78cb-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c78cb-122">Example</span></span>

### <a name="request"></a><span data-ttu-id="c78cb-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c78cb-123">Request</span></span>
<!-- { "blockType": "request" } -->
```http
POST https://graph.microsoft.com/beta/sites/{site-id}/columns
Content-Type: application/json

{
  "description": "test",
  "enforceUniqueValues": false,
  "hidden": false,
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

### <a name="response"></a><span data-ttu-id="c78cb-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="c78cb-124">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.columnDefinition", "truncated": true } -->

  

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "description": "test",
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
[site]: ../resources/site.md
  

