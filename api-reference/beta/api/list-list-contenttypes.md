---
author: swapnil1993
title: Listar contentTypes em uma lista
description: Listar tipos de conteúdo em uma lista
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: bb16750929a22634b594bf7ef862ca6104e4767a
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202496"
---
# <a name="list-contenttypes-in-a-list"></a><span data-ttu-id="49c4f-103">Listar contentTypes em uma lista</span><span class="sxs-lookup"><span data-stu-id="49c4f-103">List contentTypes in a list</span></span>
<span data-ttu-id="49c4f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49c4f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="49c4f-105">Obter a coleção de [recursos contentType][contentType] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="49c4f-105">Get the collection of [contentType][contentType] resources in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="49c4f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="49c4f-106">Permissions</span></span>

<span data-ttu-id="49c4f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="49c4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="49c4f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49c4f-109">Permission type</span></span>      | <span data-ttu-id="49c4f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="49c4f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49c4f-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49c4f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="49c4f-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="49c4f-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="49c4f-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49c4f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49c4f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49c4f-114">Not supported.</span></span>    |
|<span data-ttu-id="49c4f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49c4f-115">Application</span></span> | <span data-ttu-id="49c4f-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="49c4f-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49c4f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49c4f-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /sites/{site-id}/lists/{list-id}/contentTypes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="49c4f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="49c4f-118">Optional query parameters</span></span>

<span data-ttu-id="49c4f-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="49c4f-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="49c4f-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="49c4f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="49c4f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49c4f-121">Request headers</span></span>
|<span data-ttu-id="49c4f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="49c4f-122">Name</span></span>|<span data-ttu-id="49c4f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="49c4f-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="49c4f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="49c4f-124">Authorization</span></span>|<span data-ttu-id="49c4f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49c4f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="49c4f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49c4f-127">Request body</span></span>
<span data-ttu-id="49c4f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="49c4f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49c4f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="49c4f-129">Response</span></span>

<span data-ttu-id="49c4f-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos contentType](../resources/contenttype.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49c4f-130">If successful, this method returns a `200 OK` response code and a collection of [contentType](../resources/contenttype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49c4f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49c4f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="49c4f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49c4f-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="49c4f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="49c4f-133">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum_contentTypes"} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/contentTypes
```
# <a name="c"></a>[<span data-ttu-id="49c4f-134">C#</span><span class="sxs-lookup"><span data-stu-id="49c4f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-contenttypes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49c4f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49c4f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-contenttypes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49c4f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49c4f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-contenttypes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49c4f-137">Java</span><span class="sxs-lookup"><span data-stu-id="49c4f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-contenttypes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="49c4f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="49c4f-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.contentType)"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
        "id":"0x",
        "description":"",
        "group":"_Hidden",
        "hidden":false,
        "name":"System",
        "base": {
            "name": "System",
            "id": "0x"
        }
    },
    {
        "id":"0x00A7470EADF4194E2E9ED1031B61DA0884",
        "name": "docSet",
        "description": "custom docset",
        "hidden":false,
        "base": {
            "name": "Document Set",
            "id": "0x0120D520"
        },
        "group": "Custom Content Types"
    }
  ]
}
```


[contentType]: ../resources/contentType.md
[list]: ../resources/list.md
