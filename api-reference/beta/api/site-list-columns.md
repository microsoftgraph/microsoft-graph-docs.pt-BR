---
author: swapnil1993
title: Listar colunas em um site
description: Listar colunas em um site.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 30cb4348c1203d188a62f72d0545cd9d95de4112
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200767"
---
# <a name="list-columns-in-a-site"></a><span data-ttu-id="006a4-103">Listar colunas em um site</span><span class="sxs-lookup"><span data-stu-id="006a4-103">List columns in a site</span></span>
<span data-ttu-id="006a4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="006a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="006a4-105">Obter o conjunto de colunas, representado como [columnDefinition][columnDefinition] resources, in a [site][site].</span><span class="sxs-lookup"><span data-stu-id="006a4-105">Get the collection of columns, represented as [columnDefinition][columnDefinition] resources, in a [site][site].</span></span>

  

## <a name="permissions"></a><span data-ttu-id="006a4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="006a4-106">Permissions</span></span>

  

<span data-ttu-id="006a4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="006a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="006a4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="006a4-109">Permission type</span></span> | <span data-ttu-id="006a4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="006a4-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="006a4-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="006a4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="006a4-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="006a4-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="006a4-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="006a4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="006a4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="006a4-114">Not supported.</span></span> |
|<span data-ttu-id="006a4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="006a4-115">Application</span></span> | <span data-ttu-id="006a4-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="006a4-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |

  

## <a name="http-request"></a><span data-ttu-id="006a4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="006a4-117">HTTP request</span></span>

  
<!-- {
  "blockType": "ignored"
}
-->
```http

GET /sites/{site-id}/columns
```

  
## <a name="optional-query-parameters"></a><span data-ttu-id="006a4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="006a4-118">Optional query parameters</span></span>
<span data-ttu-id="006a4-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="006a4-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="006a4-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="006a4-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="006a4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="006a4-121">Request headers</span></span>
|<span data-ttu-id="006a4-122">Nome</span><span class="sxs-lookup"><span data-stu-id="006a4-122">Name</span></span>|<span data-ttu-id="006a4-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="006a4-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="006a4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="006a4-124">Authorization</span></span>|<span data-ttu-id="006a4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="006a4-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="006a4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="006a4-127">Request body</span></span>
<span data-ttu-id="006a4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="006a4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="006a4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="006a4-129">Response</span></span>

<span data-ttu-id="006a4-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos columnDefinition][] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="006a4-130">If successful, this method returns a `200 OK` response code and a collection of [columnDefinition][] objects in the response body.</span></span>

  

## <a name="example"></a><span data-ttu-id="006a4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="006a4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="006a4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="006a4-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="006a4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="006a4-133">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get_columns_from_site" } -->
 

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/columns
```
# <a name="c"></a>[<span data-ttu-id="006a4-134">C#</span><span class="sxs-lookup"><span data-stu-id="006a4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-columns-from-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="006a4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="006a4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-columns-from-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="006a4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="006a4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-columns-from-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="006a4-137">Java</span><span class="sxs-lookup"><span data-stu-id="006a4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-columns-from-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="006a4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="006a4-138">Response</span></span>
><span data-ttu-id="006a4-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="006a4-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
[site]: ../resources/site.md
 
