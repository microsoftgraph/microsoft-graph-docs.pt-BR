---
author: swapnil1993
ms.date: 08/30/2020
title: Criar columnDefinition em um site
description: Criar uma coluna de site.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 1404707dc2a98b4ac60e663fd25d595c977148f7
ms.sourcegitcommit: aa18eb8a9965f99cc97680808abba8df46f31ba5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2021
ms.locfileid: "51638835"
---
# <a name="create-columndefinition-for-a-site"></a><span data-ttu-id="6ed13-103">Criar columnDefinition para um site</span><span class="sxs-lookup"><span data-stu-id="6ed13-103">Create columnDefinition for a site</span></span>
<span data-ttu-id="6ed13-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ed13-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="6ed13-105">Crie uma coluna para um [site][site] by specifying a [columnDefinition][columnDefinition] .</span><span class="sxs-lookup"><span data-stu-id="6ed13-105">Create a column for a [site][site] by specifying a [columnDefinition][columnDefinition].</span></span>

## <a name="permissions"></a><span data-ttu-id="6ed13-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="6ed13-106">Permissions</span></span>

<span data-ttu-id="6ed13-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6ed13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/concepts/permissions_reference.md).</span></span>

  

|<span data-ttu-id="6ed13-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ed13-109">Permission type</span></span> | <span data-ttu-id="6ed13-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6ed13-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ed13-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ed13-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6ed13-112">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="6ed13-112">Sites.Manage.All, Sites.FullControl.All</span></span> |
|<span data-ttu-id="6ed13-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ed13-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ed13-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ed13-114">Not supported.</span></span> |
|<span data-ttu-id="6ed13-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ed13-115">Application</span></span> | <span data-ttu-id="6ed13-116">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="6ed13-116">Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="6ed13-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ed13-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /sites/{site-id}/columns
```

## <a name="request-body"></a><span data-ttu-id="6ed13-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ed13-118">Request body</span></span>

<span data-ttu-id="6ed13-119">No corpo da solicitação, fornece uma representação JSON do [recurso columnDefinition][] a adicionar.</span><span class="sxs-lookup"><span data-stu-id="6ed13-119">In the request body, supply a JSON representation of the [columnDefinition][] resource to add.</span></span>  

## <a name="response"></a><span data-ttu-id="6ed13-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ed13-120">Response</span></span>

<span data-ttu-id="6ed13-121">Se tiver êxito, este método retornará um código de resposta e `201 Created` [um objeto columnDefinition][] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ed13-121">If successful, this method returns a `201 Created` response code and [columnDefinition][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ed13-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ed13-122">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ed13-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ed13-123">Request</span></span>
<!-- { "blockType": "request" } -->
```http
POST https://graph.microsoft.com/beta/sites/{site-id}/columns
Content-Type: application/json

{
   "description":"test",
   "enforceUniqueValues":false,
   "hidden":false,
   "indexed":false,
   "name":"Title",
   "text":{
      "allowMultipleLines":false,
      "appendChangesToExistingText":false,
      "linesForEditing":0,
      "maxLength":255
   }
}
```

### <a name="response"></a><span data-ttu-id="6ed13-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ed13-124">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.columnDefinition", "truncated": true } -->

  

```http
HTTP/1.1 201 Created
Content-type: application/json

{
   "description":"test",
   "displayName":"Title",
   "enforceUniqueValues":false,
   "hidden":false,
   "id":"99ddcf45-e2f7-4f17-82b0-6fba34445103",
   "indexed":false,
   "name":"Title",
   "text":{
      "allowMultipleLines":false,
      "appendChangesToExistingText":false,
      "linesForEditing":0,
      "maxLength":255
   }
}
```

  

[columnDefinition]: ../resources/columnDefinition.md
[site]: ../resources/site.md
  

