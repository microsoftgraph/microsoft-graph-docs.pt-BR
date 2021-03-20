---
author: swapnil1993
title: 'contentType: associateWithHubSites'
description: Associe um tipo de conteúdo à lista de hubsites.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: dbddfcd4f2f3fc94c9be4ebf30aeb0c8522ea855
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947011"
---
# <a name="contenttype-associatewithhubsites"></a><span data-ttu-id="fcad6-103">contentType: associateWithHubSites</span><span class="sxs-lookup"><span data-stu-id="fcad6-103">contentType: associateWithHubSites</span></span>

<span data-ttu-id="fcad6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcad6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="fcad6-105">[Associe um tipo de][contentType] conteúdo a uma lista de sites de hub.</span><span class="sxs-lookup"><span data-stu-id="fcad6-105">Associate a [content type][contentType] with a list of hub sites.</span></span>

><span data-ttu-id="fcad6-106">**Observação:** Esse recurso é limitado a locatários que têm uma licença syntex do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fcad6-106">**Note:** This feature is limited to tenants that have a SharePoint Syntex license.</span></span>
  

## <a name="permissions"></a><span data-ttu-id="fcad6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fcad6-107">Permissions</span></span>  

<span data-ttu-id="fcad6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fcad6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="fcad6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fcad6-110">Permission type</span></span> | <span data-ttu-id="fcad6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fcad6-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------
|<span data-ttu-id="fcad6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fcad6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fcad6-113">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="fcad6-113">Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="fcad6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fcad6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fcad6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fcad6-115">Not supported.</span></span> |
|<span data-ttu-id="fcad6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fcad6-116">Application</span></span> | <span data-ttu-id="fcad6-117">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="fcad6-117">Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="fcad6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fcad6-118">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
POST /sites/id/contentTypes/id/associateWithHubSites
```

## <a name="request-headers"></a><span data-ttu-id="fcad6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fcad6-119">Request headers</span></span>
|<span data-ttu-id="fcad6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="fcad6-120">Name</span></span>|<span data-ttu-id="fcad6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcad6-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fcad6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fcad6-122">Authorization</span></span>|<span data-ttu-id="fcad6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fcad6-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fcad6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fcad6-125">Content-Type</span></span>|<span data-ttu-id="fcad6-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fcad6-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcad6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fcad6-128">Request body</span></span>
<span data-ttu-id="fcad6-129">No corpo da solicitação, fornece uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="fcad6-129">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="fcad6-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="fcad6-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fcad6-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="fcad6-131">Parameter</span></span>|<span data-ttu-id="fcad6-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="fcad6-132">Type</span></span>|<span data-ttu-id="fcad6-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcad6-133">Description</span></span>|
|-|-|-|
|<span data-ttu-id="fcad6-134">hubSiteUrls</span><span class="sxs-lookup"><span data-stu-id="fcad6-134">hubSiteUrls</span></span>| <span data-ttu-id="fcad6-135">Collection(string)</span><span class="sxs-lookup"><span data-stu-id="fcad6-135">Collection(string)</span></span> |<span data-ttu-id="fcad6-136">Lista de URLs canônicas para os sites de hub onde o tipo de conteúdo precisa ser imposto.</span><span class="sxs-lookup"><span data-stu-id="fcad6-136">List of cannonical URLs to the hub sites where the content type needs to be enforced.</span></span> <span data-ttu-id="fcad6-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fcad6-137">Required.</span></span>|
|<span data-ttu-id="fcad6-138">propagateToExistingLists</span><span class="sxs-lookup"><span data-stu-id="fcad6-138">propagateToExistingLists</span></span>| <span data-ttu-id="fcad6-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="fcad6-139">Boolean</span></span> |<span data-ttu-id="fcad6-140">Se , os tipos de conteúdo serão impostos em listas existentes nos sites de hub; caso contrário, ele será aplicado somente a listas `true` recém-criadas.</span><span class="sxs-lookup"><span data-stu-id="fcad6-140">If `true`, content types will be enforced on existing lists in the hub sites; otherwise, it will be applied only to newly created lists.</span></span> 

## <a name="response"></a><span data-ttu-id="fcad6-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcad6-141">Response</span></span>

<span data-ttu-id="fcad6-142">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fcad6-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fcad6-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fcad6-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="fcad6-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fcad6-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="fcad6-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="fcad6-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contenttype_associatewithhubsites"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/id/contentTypes/id/associateWithHubSites
Content-Type: application/json

{
   "hubSiteUrls":[
      "https://graph.microsoft.com/beta/sites/id"
   ],
   "propagateToExistingLists":false
}
```
# <a name="c"></a>[<span data-ttu-id="fcad6-146">C#</span><span class="sxs-lookup"><span data-stu-id="fcad6-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contenttype-associatewithhubsites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fcad6-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fcad6-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contenttype-associatewithhubsites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fcad6-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fcad6-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contenttype-associatewithhubsites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fcad6-149">Java</span><span class="sxs-lookup"><span data-stu-id="fcad6-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contenttype-associatewithhubsites-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




### <a name="response"></a><span data-ttu-id="fcad6-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcad6-150">Response</span></span>


<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

  

[contentType]: ../resources/contentType.md
