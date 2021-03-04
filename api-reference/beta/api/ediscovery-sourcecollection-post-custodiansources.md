---
title: Adicionar custodianSources
description: Adicionar objetos dataSource de custodia a uma coleção de origem.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 58088bb97f66cf0c5ac379526b641c1bf0985250
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445742"
---
# <a name="add-custodiansources"></a><span data-ttu-id="1cdea-103">Adicionar custodianSources</span><span class="sxs-lookup"><span data-stu-id="1cdea-103">Add custodianSources</span></span>

<span data-ttu-id="1cdea-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="1cdea-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cdea-105">Adicionar objetos [dataSource custodiantes](../resources/ediscovery-datasource.md) a uma coleção de origem.</span><span class="sxs-lookup"><span data-stu-id="1cdea-105">Add custodian [dataSource](../resources/ediscovery-datasource.md) objects to a source collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="1cdea-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1cdea-106">Permissions</span></span>

<span data-ttu-id="1cdea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cdea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cdea-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1cdea-109">Permission type</span></span>|<span data-ttu-id="1cdea-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1cdea-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cdea-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1cdea-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1cdea-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cdea-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="1cdea-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1cdea-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cdea-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cdea-114">Not supported.</span></span>|
|<span data-ttu-id="1cdea-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1cdea-115">Application</span></span>|<span data-ttu-id="1cdea-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cdea-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cdea-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1cdea-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/custodianSources/$ref
```

## <a name="request-headers"></a><span data-ttu-id="1cdea-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1cdea-118">Request headers</span></span>

|<span data-ttu-id="1cdea-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1cdea-119">Name</span></span>|<span data-ttu-id="1cdea-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cdea-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1cdea-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1cdea-121">Authorization</span></span>|<span data-ttu-id="1cdea-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cdea-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1cdea-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1cdea-124">Content-Type</span></span>|<span data-ttu-id="1cdea-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cdea-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cdea-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1cdea-127">Request body</span></span>

<span data-ttu-id="1cdea-128">No corpo da solicitação, fornece uma representação JSON do [objeto dataSource.](../resources/ediscovery-datasource.md)</span><span class="sxs-lookup"><span data-stu-id="1cdea-128">In the request body, supply a JSON representation of the [dataSource](../resources/ediscovery-datasource.md) object.</span></span>

<span data-ttu-id="1cdea-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o dataSource](../resources/ediscovery-datasource.md).</span><span class="sxs-lookup"><span data-stu-id="1cdea-129">The following table shows the properties that are required when you create the [dataSource](../resources/ediscovery-datasource.md).</span></span>

|<span data-ttu-id="1cdea-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1cdea-130">Property</span></span>|<span data-ttu-id="1cdea-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cdea-131">Type</span></span>|<span data-ttu-id="1cdea-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cdea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cdea-133">@odata.id</span><span class="sxs-lookup"><span data-stu-id="1cdea-133">@odata.id</span></span>|<span data-ttu-id="1cdea-134">String</span><span class="sxs-lookup"><span data-stu-id="1cdea-134">String</span></span>|<span data-ttu-id="1cdea-135">Cadeia de caracteres que define o objeto custodial.</span><span class="sxs-lookup"><span data-stu-id="1cdea-135">String that defines the custodial object.</span></span> <span data-ttu-id="1cdea-136">Vejo o exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="1cdea-136">See the example that follows.</span></span>|

## <a name="response"></a><span data-ttu-id="1cdea-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cdea-137">Response</span></span>

<span data-ttu-id="1cdea-138">Se tiver êxito, este método retornará um código de resposta e um `204 No Content` [objeto microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1cdea-138">If successful, this method returns a `204 No Content` response code and a [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1cdea-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1cdea-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1cdea-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cdea-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_datasource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourceCollections/1a9b4145d8f84e39bc45a7f68c5c5119/custodianSources/$ref
Content-Type: application/json
Content-length: 179

{
  "@odata.id":"https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/ab3a628a383045eba344b3caecba3104/userSources/31423539-3846-4333-4136-353644383531"
}
```

### <a name="response"></a><span data-ttu-id="1cdea-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cdea-141">Response</span></span>

<span data-ttu-id="1cdea-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1cdea-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.dataSource"
}
-->

``` http
HTTP/1.1 204 No Content
Content-Type: application/json
```
