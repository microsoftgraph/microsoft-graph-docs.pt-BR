---
author: swapnil1993
title: Listar columnDefinitions em uma lista
description: Listar colunas em uma lista.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: f6e1567e3fded5a1360725bf248025390d74f058
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965019"
---
# <a name="list-columns-in-a-list"></a><span data-ttu-id="65497-103">Listar colunas em uma lista</span><span class="sxs-lookup"><span data-stu-id="65497-103">List columns in a list</span></span>
<span data-ttu-id="65497-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65497-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="65497-105">Obter a coleção de colunas, representada como [columnDefinition][columnDefinition] resources, em uma [lista][list].</span><span class="sxs-lookup"><span data-stu-id="65497-105">Get the collection of columns, represented as [columnDefinition][columnDefinition] resources, in a [list][list].</span></span>

  

## <a name="permissions"></a><span data-ttu-id="65497-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="65497-106">Permissions</span></span>

  

<span data-ttu-id="65497-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="65497-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="65497-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65497-109">Permission type</span></span> | <span data-ttu-id="65497-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="65497-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65497-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65497-111">Delegated (work or school account)</span></span> | <span data-ttu-id="65497-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="65497-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="65497-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65497-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65497-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65497-114">Not supported.</span></span> |
|<span data-ttu-id="65497-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65497-115">Application</span></span> | <span data-ttu-id="65497-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="65497-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |

  

## <a name="http-request"></a><span data-ttu-id="65497-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65497-117">HTTP request</span></span>

  
<!-- {
  "blockType": "ignored"
}
-->
```http

GET /sites/{site-id}/lists/{list-id}/columns
```

  
## <a name="optional-query-parameters"></a><span data-ttu-id="65497-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="65497-118">Optional query parameters</span></span>
<span data-ttu-id="65497-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="65497-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="65497-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="65497-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="65497-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65497-121">Request headers</span></span>
|<span data-ttu-id="65497-122">Nome</span><span class="sxs-lookup"><span data-stu-id="65497-122">Name</span></span>|<span data-ttu-id="65497-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="65497-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="65497-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="65497-124">Authorization</span></span>|<span data-ttu-id="65497-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65497-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="65497-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65497-127">Request body</span></span>
<span data-ttu-id="65497-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="65497-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65497-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="65497-129">Response</span></span>

<span data-ttu-id="65497-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos columnDefinition][] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65497-130">If successful, this method returns a `200 OK` response code and a collection of [columnDefinition][] objects in the response body.</span></span>

  

## <a name="example"></a><span data-ttu-id="65497-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65497-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="65497-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65497-132">Request</span></span>

<!-- { "blockType": "request", "name": "get_columns_from_list" } -->
 

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/columns
```

### <a name="response"></a><span data-ttu-id="65497-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="65497-133">Response</span></span>
><span data-ttu-id="65497-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="65497-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.columnDefinition)"
}
-->  

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
    },
    {
      "description": "",
      "displayName": "Address",
      "id": "11dfef35-e2f7-4f17-82b0-6fba34445103",
      "indexed": false,
      "name": "Address",
      "readOnly": false,
      "required": false,
      "text": {
        "allowMultipleLines": false,
        "appendChangesToExistingText": false,
        "linesForEditing": 0,
        "maxLength": 255
      }
    }
  ]
}
```

  

[columnDefinition]: ../resources/columnDefinition.md
[list]: ../resources/list.md
 
