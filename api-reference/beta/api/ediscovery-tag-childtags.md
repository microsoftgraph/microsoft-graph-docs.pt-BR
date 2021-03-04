---
title: Listar childTags
description: Obter uma lista de objetos filho [tag] associados a uma marca.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 2e59fa0d54d9b8bf2793ee61759f6c675722fed5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445734"
---
# <a name="list-childtags"></a><span data-ttu-id="f17c9-103">Listar childTags</span><span class="sxs-lookup"><span data-stu-id="f17c9-103">List childTags</span></span>

<span data-ttu-id="f17c9-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="f17c9-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f17c9-105">Obter uma lista de objetos [de marca](../resources/ediscovery-tag.md) filho associados a uma marca.</span><span class="sxs-lookup"><span data-stu-id="f17c9-105">Get a list of child [tag](../resources/ediscovery-tag.md) objects associated with a tag.</span></span>

## <a name="permissions"></a><span data-ttu-id="f17c9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f17c9-106">Permissions</span></span>

<span data-ttu-id="f17c9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f17c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f17c9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f17c9-109">Permission type</span></span>|<span data-ttu-id="f17c9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f17c9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f17c9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f17c9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f17c9-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f17c9-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="f17c9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f17c9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f17c9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f17c9-114">Not supported.</span></span>|
|<span data-ttu-id="f17c9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f17c9-115">Application</span></span>|<span data-ttu-id="f17c9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f17c9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f17c9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f17c9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/tags/{tagId}/childTags
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f17c9-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f17c9-118">Optional query parameters</span></span>

<span data-ttu-id="f17c9-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f17c9-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f17c9-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f17c9-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f17c9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f17c9-121">Request headers</span></span>

|<span data-ttu-id="f17c9-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f17c9-122">Name</span></span>|<span data-ttu-id="f17c9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f17c9-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f17c9-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f17c9-124">Authorization</span></span>|<span data-ttu-id="f17c9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f17c9-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f17c9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f17c9-127">Request body</span></span>

<span data-ttu-id="f17c9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f17c9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f17c9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f17c9-129">Response</span></span>

<span data-ttu-id="f17c9-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f17c9-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f17c9-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f17c9-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f17c9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f17c9-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_tag"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/e54b3f535b434a9a8743b84e34c00504/childTags
```

### <a name="response"></a><span data-ttu-id="f17c9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f17c9-133">Response</span></span>

<span data-ttu-id="f17c9-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f17c9-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
