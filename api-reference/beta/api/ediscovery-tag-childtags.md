---
title: Listar childTags
description: Obter uma lista de objetos filho [tag] associados a uma marca.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: b9683b2b38420d0e535cc0b87bf54d55a663f3f3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951997"
---
# <a name="list-childtags"></a><span data-ttu-id="aa261-103">Listar childTags</span><span class="sxs-lookup"><span data-stu-id="aa261-103">List childTags</span></span>

<span data-ttu-id="aa261-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="aa261-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa261-105">Obter uma lista de objetos [de marca](../resources/ediscovery-tag.md) filho associados a uma marca.</span><span class="sxs-lookup"><span data-stu-id="aa261-105">Get a list of child [tag](../resources/ediscovery-tag.md) objects associated with a tag.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa261-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="aa261-106">Permissions</span></span>

<span data-ttu-id="aa261-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa261-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa261-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa261-109">Permission type</span></span>|<span data-ttu-id="aa261-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aa261-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa261-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa261-111">Delegated (work or school account)</span></span>|<span data-ttu-id="aa261-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa261-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="aa261-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa261-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa261-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa261-114">Not supported.</span></span>|
|<span data-ttu-id="aa261-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa261-115">Application</span></span>|<span data-ttu-id="aa261-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa261-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa261-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa261-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/tags/{tagId}/childTags
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aa261-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="aa261-118">Optional query parameters</span></span>

<span data-ttu-id="aa261-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="aa261-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="aa261-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="aa261-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa261-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa261-121">Request headers</span></span>

|<span data-ttu-id="aa261-122">Nome</span><span class="sxs-lookup"><span data-stu-id="aa261-122">Name</span></span>|<span data-ttu-id="aa261-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa261-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="aa261-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa261-124">Authorization</span></span>|<span data-ttu-id="aa261-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa261-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa261-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa261-127">Request body</span></span>

<span data-ttu-id="aa261-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aa261-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa261-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa261-129">Response</span></span>

<span data-ttu-id="aa261-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa261-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aa261-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="aa261-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aa261-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa261-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="aa261-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa261-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tag_2"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/e54b3f535b434a9a8743b84e34c00504/childTags
```
# <a name="c"></a>[<span data-ttu-id="aa261-134">C#</span><span class="sxs-lookup"><span data-stu-id="aa261-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tag-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa261-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa261-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tag-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa261-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa261-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tag-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aa261-137">Java</span><span class="sxs-lookup"><span data-stu-id="aa261-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tag-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="aa261-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa261-138">Response</span></span>

<span data-ttu-id="aa261-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="aa261-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.ediscovery.tag)",
    "value": [
        {
            "displayName": "Yes",
            "description": "The document is responsive",
            "lastModifiedDateTime": "2021-01-11T19:32:22.4091161Z",
            "childSelectability": "One",
            "id": "081ff31e7324423186e01b549efe7033",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": "EDisco Admin",
                    "userPrincipalName": "admin@contoso.com"
                }
            },
            "childTags": []
        },
        {
            "displayName": "No",
            "description": "The document is not responsive",
            "lastModifiedDateTime": "2021-01-11T19:32:21.5693878Z",
            "childSelectability": "One",
            "id": "61624e6c96a64ccea40e0d2c48e23e16",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": "EDisco Admin",
                    "userPrincipalName": "admin@contoso.com"
                }
            },
            "childTags": []
        }
    ]
}
```
