---
author: swapnil1993
title: Listar contentTypes em um site
description: Listar tipos de conteúdo em um site
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 0ff43805d40982f4b945c690d1324e7c0593b9ec
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965028"
---
# <a name="list-contenttypes-in-a-site"></a><span data-ttu-id="2ebea-103">Listar contentTypes em um site</span><span class="sxs-lookup"><span data-stu-id="2ebea-103">List contentTypes in a site</span></span>
<span data-ttu-id="2ebea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ebea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="2ebea-105">Obter a coleção de [recursos contentType][contentType] em um [site][].</span><span class="sxs-lookup"><span data-stu-id="2ebea-105">Get the collection of [contentType][contentType] resources in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="2ebea-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ebea-106">Permissions</span></span>

<span data-ttu-id="2ebea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2ebea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="2ebea-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ebea-109">Permission type</span></span>      | <span data-ttu-id="2ebea-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ebea-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ebea-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ebea-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2ebea-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="2ebea-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="2ebea-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ebea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ebea-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ebea-114">Not supported.</span></span>    |
|<span data-ttu-id="2ebea-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ebea-115">Application</span></span> | <span data-ttu-id="2ebea-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="2ebea-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ebea-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ebea-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /sites/{site-id}/contentTypes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ebea-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2ebea-118">Optional query parameters</span></span>

<span data-ttu-id="2ebea-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2ebea-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2ebea-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2ebea-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ebea-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ebea-121">Request headers</span></span>
|<span data-ttu-id="2ebea-122">Nome</span><span class="sxs-lookup"><span data-stu-id="2ebea-122">Name</span></span>|<span data-ttu-id="2ebea-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ebea-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2ebea-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ebea-124">Authorization</span></span>|<span data-ttu-id="2ebea-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ebea-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ebea-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ebea-127">Request body</span></span>
<span data-ttu-id="2ebea-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2ebea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ebea-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ebea-129">Response</span></span>

<span data-ttu-id="2ebea-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos contentType](../resources/contenttype.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ebea-130">If successful, this method returns a `200 OK` response code and a collection of [contentType](../resources/contenttype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ebea-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ebea-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ebea-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ebea-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2ebea-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ebea-133">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum_contentTypes"} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/contentTypes
```
# <a name="c"></a>[<span data-ttu-id="2ebea-134">C#</span><span class="sxs-lookup"><span data-stu-id="2ebea-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-contenttypes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ebea-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ebea-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-contenttypes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ebea-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ebea-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-contenttypes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ebea-137">Java</span><span class="sxs-lookup"><span data-stu-id="2ebea-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-contenttypes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2ebea-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ebea-138">Response</span></span>

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
[site]: ../resources/site.md
