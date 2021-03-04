---
author: swapnil1993
title: Atualizar columnDefinition
description: Atualizar uma coluna de tipo de conteúdo
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 63c8ce763a3ea326664189869049fe6883c1be0d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445858"
---
# <a name="update-columndefinition"></a><span data-ttu-id="b98a7-103">Atualizar columnDefinition</span><span class="sxs-lookup"><span data-stu-id="b98a7-103">Update columnDefinition</span></span>
<span data-ttu-id="b98a7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b98a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="b98a7-105">Atualizar um [tipo de conteúdo][contentType] [column][columnDefinition] .</span><span class="sxs-lookup"><span data-stu-id="b98a7-105">Update a [content type][contentType] [column][columnDefinition].</span></span>
  

## <a name="permissions"></a><span data-ttu-id="b98a7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b98a7-106">Permissions</span></span>  

<span data-ttu-id="b98a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b98a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="b98a7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b98a7-109">Permission type</span></span> | <span data-ttu-id="b98a7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b98a7-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b98a7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b98a7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b98a7-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="b98a7-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="b98a7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b98a7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b98a7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b98a7-114">Not supported.</span></span> |
|<span data-ttu-id="b98a7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b98a7-115">Application</span></span> | <span data-ttu-id="b98a7-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="b98a7-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="b98a7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b98a7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
PATCH /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
PATCH /sites/{site-id}/lists/{list-id}//contentTypes/{contentType-id}/columns/{column-id}
```


## <a name="request-headers"></a><span data-ttu-id="b98a7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b98a7-118">Request headers</span></span>
|<span data-ttu-id="b98a7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b98a7-119">Name</span></span>|<span data-ttu-id="b98a7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b98a7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b98a7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b98a7-121">Authorization</span></span>|<span data-ttu-id="b98a7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b98a7-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b98a7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b98a7-124">Content-Type</span></span>|<span data-ttu-id="b98a7-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b98a7-p103">application/json. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="b98a7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b98a7-127">Request body</span></span>

<span data-ttu-id="b98a7-128">No corpo da solicitação, fornece uma representação JSON do [recurso columnDefinition][] a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="b98a7-128">In the request body, supply a JSON representation of the [columnDefinition][] resource to update.</span></span>  

><span data-ttu-id="b98a7-129">**Observação:** Somente as propriedades necessárias e ocultas podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="b98a7-129">**Note:** Only required and hidden properties can be updated.</span></span>

## <a name="response"></a><span data-ttu-id="b98a7-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b98a7-130">Response</span></span>

<span data-ttu-id="b98a7-131">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [columnDefinition][] atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b98a7-131">If successful, this method returns a `200 OK` response code and an updated [columnDefinition][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b98a7-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b98a7-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b98a7-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b98a7-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contenttype_column"
}
-->
```http
PATCH /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
Content-Type: application/json

{
  "required": true,
  "hidden": false,
  "propagateChanges": false     
}
```

### <a name="response"></a><span data-ttu-id="b98a7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b98a7-134">Response</span></span>
><span data-ttu-id="b98a7-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b98a7-135">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.columnDefinition"
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "",
  "displayName": "Custom Column",
  "enforceUniqueValues": false,
  "hidden": false,
  "id": "11dfef35-e2f7-4f17-82b0-6fba34445103",
  "indexed": false,
  "name": "Custom Column",
  "readOnly": false,
  "required": true,
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
