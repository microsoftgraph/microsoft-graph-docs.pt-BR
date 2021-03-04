---
title: Obter marca
description: Leia as propriedades e as relações de um objeto tag.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 0ac2c2c1fe3e9a4d8d61980ce09850f24cac782a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445730"
---
# <a name="get-tag"></a><span data-ttu-id="46d3c-103">Obter marca</span><span class="sxs-lookup"><span data-stu-id="46d3c-103">Get tag</span></span>

<span data-ttu-id="46d3c-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="46d3c-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46d3c-105">Leia as propriedades e as relações de um [objeto tag.](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="46d3c-105">Read the properties and relationships of a [tag](../resources/ediscovery-tag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="46d3c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="46d3c-106">Permissions</span></span>

<span data-ttu-id="46d3c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46d3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46d3c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46d3c-109">Permission type</span></span>|<span data-ttu-id="46d3c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46d3c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46d3c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46d3c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="46d3c-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46d3c-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="46d3c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46d3c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46d3c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46d3c-114">Not supported.</span></span>|
|<span data-ttu-id="46d3c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46d3c-115">Application</span></span>|<span data-ttu-id="46d3c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46d3c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46d3c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46d3c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/tags/{tagId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="46d3c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="46d3c-118">Optional query parameters</span></span>

<span data-ttu-id="46d3c-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="46d3c-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="46d3c-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="46d3c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="46d3c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46d3c-121">Request headers</span></span>

|<span data-ttu-id="46d3c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="46d3c-122">Name</span></span>|<span data-ttu-id="46d3c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="46d3c-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="46d3c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="46d3c-124">Authorization</span></span>|<span data-ttu-id="46d3c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46d3c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="46d3c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46d3c-127">Request body</span></span>

<span data-ttu-id="46d3c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="46d3c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46d3c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="46d3c-129">Response</span></span>

<span data-ttu-id="46d3c-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46d3c-130">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="46d3c-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="46d3c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="46d3c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46d3c-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_tag"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/e54b3f535b434a9a8743b84e34c00504
```

### <a name="response"></a><span data-ttu-id="46d3c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="46d3c-133">Response</span></span>

<span data-ttu-id="46d3c-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="46d3c-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.tag"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('47746044-fd0b-4a30-acfc-5272b691ba5b')/tags/$entity",
    "displayName": "Responsiveness",
    "description": "Indicates the responsiveness of the document",
    "lastModifiedDateTime": "2021-01-11T19:32:23.1903658Z",
    "childSelectability": "One",
    "id": "e54b3f535b434a9a8743b84e34c00504",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "EDisco Admin",
            "userPrincipalName": "admin@contoso.com"
        }
    },
    "childTags": []
}
```
