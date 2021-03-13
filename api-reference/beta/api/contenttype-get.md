---
author: swapnil1993
title: Obter contentType
description: Obter um tipo de conteúdo em um site ou em uma lista.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: a3dabf343ee4aef7c913cbcfa1bb6179b764fcf2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770599"
---
# <a name="get-contenttype"></a><span data-ttu-id="1f7a4-103">Obter contentType</span><span class="sxs-lookup"><span data-stu-id="1f7a4-103">Get contentType</span></span>
<span data-ttu-id="1f7a4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f7a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f7a4-105">Recupere os metadados de [um tipo de conteúdo][contentType] em um [site][] ou em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="1f7a4-105">Retrieve the metadata for a [content type][contentType] in a [site][] or a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="1f7a4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1f7a4-106">Permissions</span></span>

<span data-ttu-id="1f7a4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f7a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f7a4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f7a4-109">Permission type</span></span>      | <span data-ttu-id="1f7a4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f7a4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f7a4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f7a4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1f7a4-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="1f7a4-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="1f7a4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f7a4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f7a4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f7a4-114">Not supported.</span></span>    |
|<span data-ttu-id="1f7a4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f7a4-115">Application</span></span> | <span data-ttu-id="1f7a4-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="1f7a4-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f7a4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f7a4-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /sites/{site-id}/contentTypes/{contentType-id}

GET /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1f7a4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1f7a4-118">Optional query parameters</span></span>
<span data-ttu-id="1f7a4-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1f7a4-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1f7a4-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1f7a4-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f7a4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f7a4-121">Request headers</span></span>
|<span data-ttu-id="1f7a4-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1f7a4-122">Name</span></span>|<span data-ttu-id="1f7a4-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f7a4-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1f7a4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f7a4-124">Authorization</span></span>|<span data-ttu-id="1f7a4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f7a4-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f7a4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f7a4-127">Request body</span></span>
<span data-ttu-id="1f7a4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1f7a4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f7a4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f7a4-129">Response</span></span>

<span data-ttu-id="1f7a4-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [contentType](../resources/contenttype.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f7a4-130">If successful, this method returns a `200 OK` response code and a [contentType](../resources/contenttype.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="1f7a4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f7a4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f7a4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f7a4-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1f7a4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f7a4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contenttype"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}
```
# <a name="c"></a>[<span data-ttu-id="1f7a4-134">C#</span><span class="sxs-lookup"><span data-stu-id="1f7a4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contenttype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f7a4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f7a4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f7a4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f7a4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contenttype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1f7a4-137">Java</span><span class="sxs-lookup"><span data-stu-id="1f7a4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contenttype-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1f7a4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f7a4-138">Response</span></span>
><span data-ttu-id="1f7a4-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1f7a4-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contentType"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id":"0x0120D520",
  "description":"Create a document set when you want to manage multiple documents as a single work product.",
  "group":"Document Set Content Types",
  "hidden":false,
  "name":"Document Set",
  "base": {
        "name": "Document Set",
        "id": "0x0120D520"
   }
}
```

[contentType]: ../resources/contentType.md
[site]: ../resources/site.md
[list]: ../resources/list.md
