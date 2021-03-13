---
title: 'tag: asHierarchy'
description: Retornar uma lista de marcas no formato hierárquico.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 34834c8ee010c8365a68b587b333bdaae6abe1fd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772531"
---
# <a name="tag-ashierarchy"></a><span data-ttu-id="d9675-103">tag: asHierarchy</span><span class="sxs-lookup"><span data-stu-id="d9675-103">tag: asHierarchy</span></span>

<span data-ttu-id="d9675-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="d9675-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9675-105">Retornar uma lista de [objetos de](../resources/ediscovery-tag.md) marca no formato hierárquico</span><span class="sxs-lookup"><span data-stu-id="d9675-105">Return a list of [tag](../resources/ediscovery-tag.md) objects in hierarchial form</span></span>

## <a name="permissions"></a><span data-ttu-id="d9675-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d9675-106">Permissions</span></span>

<span data-ttu-id="d9675-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9675-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9675-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9675-109">Permission type</span></span>|<span data-ttu-id="d9675-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9675-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9675-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9675-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d9675-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9675-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="d9675-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9675-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9675-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9675-114">Not supported.</span></span>|
|<span data-ttu-id="d9675-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9675-115">Application</span></span>|<span data-ttu-id="d9675-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9675-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9675-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9675-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/tags/asHierarchy
```

## <a name="request-headers"></a><span data-ttu-id="d9675-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9675-118">Request headers</span></span>

|<span data-ttu-id="d9675-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d9675-119">Name</span></span>|<span data-ttu-id="d9675-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9675-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d9675-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9675-121">Authorization</span></span>|<span data-ttu-id="d9675-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9675-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9675-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9675-124">Request body</span></span>

<span data-ttu-id="d9675-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9675-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9675-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9675-126">Response</span></span>

<span data-ttu-id="d9675-127">Se tiver êxito, essa função retornará um código de resposta e uma coleção `200 OK` [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9675-127">If successful, this function returns a `200 OK` response code and a [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9675-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d9675-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d9675-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9675-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d9675-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9675-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tag_ashierarchy"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/asHierarchy
```
# <a name="c"></a>[<span data-ttu-id="d9675-131">C#</span><span class="sxs-lookup"><span data-stu-id="d9675-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tag-ashierarchy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9675-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9675-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tag-ashierarchy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9675-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9675-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tag-ashierarchy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9675-134">Java</span><span class="sxs-lookup"><span data-stu-id="d9675-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tag-ashierarchy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d9675-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9675-135">Response</span></span>

<span data-ttu-id="d9675-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d9675-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.tag)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ediscovery.tag",
      "id": "String (identifier)",
      "displayName": "String",
      "description": "String",
      "childSelectability": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "String (timestamp)"
    }
  ]
}
```
