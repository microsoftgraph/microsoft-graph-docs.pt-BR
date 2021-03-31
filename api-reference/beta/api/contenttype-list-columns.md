---
author: swapnil1993
title: Listar columnDefinitions em um tipo de conteúdo
description: Listar colunas em um tipo de conteúdo.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 49a47efbeb59869dfc4f1b83946f9b6a8f178924
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468902"
---
# <a name="list-columns-in-a-content-type"></a><span data-ttu-id="e8603-103">Listar colunas em um tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="e8603-103">List columns in a content type</span></span>
<span data-ttu-id="e8603-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8603-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="e8603-105">Obter a coleção de colunas, representada como [columnDefinition][columnDefinition] resources, em um [tipo de conteúdo][contentType].</span><span class="sxs-lookup"><span data-stu-id="e8603-105">Get the collection of columns, represented as [columnDefinition][columnDefinition] resources, in a [content type][contentType].</span></span>

  

## <a name="permissions"></a><span data-ttu-id="e8603-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8603-106">Permissions</span></span>

  

<span data-ttu-id="e8603-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e8603-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="e8603-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8603-109">Permission type</span></span> | <span data-ttu-id="e8603-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8603-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8603-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8603-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e8603-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="e8603-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="e8603-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8603-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8603-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8603-114">Not supported.</span></span> |
|<span data-ttu-id="e8603-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8603-115">Application</span></span> | <span data-ttu-id="e8603-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="e8603-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |

  

## <a name="http-request"></a><span data-ttu-id="e8603-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8603-117">HTTP request</span></span>

  
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /sites/{site-id}/contentTypes/{contentType-id}/columns
GET /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns
```

  
## <a name="optional-query-parameters"></a><span data-ttu-id="e8603-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e8603-118">Optional query parameters</span></span>
<span data-ttu-id="e8603-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e8603-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e8603-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e8603-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8603-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8603-121">Request headers</span></span>
|<span data-ttu-id="e8603-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e8603-122">Name</span></span>|<span data-ttu-id="e8603-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8603-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e8603-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8603-124">Authorization</span></span>|<span data-ttu-id="e8603-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8603-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8603-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8603-127">Request body</span></span>
<span data-ttu-id="e8603-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8603-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8603-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8603-129">Response</span></span>

<span data-ttu-id="e8603-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos columnDefinition][] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8603-130">If successful, this method returns a `200 OK` response code and a collection of [columnDefinition][] objects in the response body.</span></span>

  

## <a name="example"></a><span data-ttu-id="e8603-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8603-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8603-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8603-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e8603-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8603-133">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get_columns_from_contenttype" } -->
 

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}/columns
```
# <a name="c"></a>[<span data-ttu-id="e8603-134">C#</span><span class="sxs-lookup"><span data-stu-id="e8603-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-columns-from-contenttype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8603-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8603-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-columns-from-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8603-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8603-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-columns-from-contenttype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e8603-137">Java</span><span class="sxs-lookup"><span data-stu-id="e8603-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-columns-from-contenttype-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e8603-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8603-138">Response</span></span>
><span data-ttu-id="e8603-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e8603-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
   "value":[
      {
         "description":"",
         "displayName":"Title",
         "hidden":false,
         "id":"99ddcf45-e2f7-4f17-82b0-6fba34445103",
         "indexed":false,
         "name":"Title",
         "readOnly":false,
         "required":false,
         "text":{
            "allowMultipleLines":false,
            "appendChangesToExistingText":false,
            "linesForEditing":0,
            "maxLength":255
         }
      },
      {
         "description":"",
         "displayName":"Address",
         "id":"11dfef35-e2f7-4f17-82b0-6fba34445103",
         "indexed":false,
         "name":"Address",
         "readOnly":false,
         "required":false,
         "text":{
            "allowMultipleLines":false,
            "appendChangesToExistingText":false,
            "linesForEditing":0,
            "maxLength":255
         }
      }
   ]
}
```

  

[columnDefinition]: ../resources/columnDefinition.md
[contentType]: ../resources/contentType.md
 
