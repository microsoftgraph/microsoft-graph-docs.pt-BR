---
title: 'tag: asHierarchy'
description: Retornar uma lista de marcas no formato hierárquico.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 7f4de1ad20f683286f177e90386511118bb9acb9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445740"
---
# <a name="tag-ashierarchy"></a><span data-ttu-id="ed5fa-103">tag: asHierarchy</span><span class="sxs-lookup"><span data-stu-id="ed5fa-103">tag: asHierarchy</span></span>

<span data-ttu-id="ed5fa-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="ed5fa-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed5fa-105">Retornar uma lista de [objetos de](../resources/ediscovery-tag.md) marca no formato hierárquico</span><span class="sxs-lookup"><span data-stu-id="ed5fa-105">Return a list of [tag](../resources/ediscovery-tag.md) objects in hierarchial form</span></span>

## <a name="permissions"></a><span data-ttu-id="ed5fa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ed5fa-106">Permissions</span></span>

<span data-ttu-id="ed5fa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed5fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed5fa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed5fa-109">Permission type</span></span>|<span data-ttu-id="ed5fa-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ed5fa-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed5fa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed5fa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ed5fa-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed5fa-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="ed5fa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed5fa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed5fa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed5fa-114">Not supported.</span></span>|
|<span data-ttu-id="ed5fa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed5fa-115">Application</span></span>|<span data-ttu-id="ed5fa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed5fa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed5fa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed5fa-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/tags/asHierarchy
```

## <a name="request-headers"></a><span data-ttu-id="ed5fa-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed5fa-118">Request headers</span></span>

|<span data-ttu-id="ed5fa-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ed5fa-119">Name</span></span>|<span data-ttu-id="ed5fa-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed5fa-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ed5fa-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed5fa-121">Authorization</span></span>|<span data-ttu-id="ed5fa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed5fa-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed5fa-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed5fa-124">Request body</span></span>

<span data-ttu-id="ed5fa-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ed5fa-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed5fa-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed5fa-126">Response</span></span>

<span data-ttu-id="ed5fa-127">Se tiver êxito, essa função retornará um código de resposta e uma coleção `200 OK` [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed5fa-127">If successful, this function returns a `200 OK` response code and a [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ed5fa-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ed5fa-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ed5fa-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed5fa-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "tag_ashierarchy"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/asHierarchy
```

### <a name="response"></a><span data-ttu-id="ed5fa-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed5fa-130">Response</span></span>

<span data-ttu-id="ed5fa-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ed5fa-131">**Note:** The response object shown here might be shortened for readability.</span></span>
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
