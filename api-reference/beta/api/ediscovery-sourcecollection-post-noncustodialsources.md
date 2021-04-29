---
title: Adicionar noncustodialDataSource
description: Adicione noncustodialSources postando na coleção noncustodialSources.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 399d20f5bc046d141e8652001fe964460c2b414c
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080703"
---
# <a name="add-noncustodialdatasource"></a><span data-ttu-id="8df83-103">Adicionar noncustodialDataSource</span><span class="sxs-lookup"><span data-stu-id="8df83-103">Add noncustodialDataSource</span></span>

<span data-ttu-id="8df83-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="8df83-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8df83-105">Adicione noncustodialSources a [uma sourceCollection](../api/ediscovery-sourcecollection-get.md).</span><span class="sxs-lookup"><span data-stu-id="8df83-105">Add noncustodialSources to a [sourceCollection](../api/ediscovery-sourcecollection-get.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8df83-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8df83-106">Permissions</span></span>

<span data-ttu-id="8df83-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8df83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8df83-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8df83-109">Permission type</span></span>|<span data-ttu-id="8df83-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8df83-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8df83-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8df83-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8df83-112">eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8df83-112">eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="8df83-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8df83-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8df83-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8df83-114">Not supported.</span></span>|
|<span data-ttu-id="8df83-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8df83-115">Application</span></span>|<span data-ttu-id="8df83-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8df83-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8df83-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8df83-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/noncustodialSources/$ref
```

## <a name="request-headers"></a><span data-ttu-id="8df83-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8df83-118">Request headers</span></span>

|<span data-ttu-id="8df83-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8df83-119">Name</span></span>|<span data-ttu-id="8df83-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8df83-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8df83-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8df83-121">Authorization</span></span>|<span data-ttu-id="8df83-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8df83-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8df83-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8df83-124">Content-Type</span></span>|<span data-ttu-id="8df83-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8df83-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8df83-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8df83-127">Request body</span></span>

<span data-ttu-id="8df83-128">No corpo da solicitação, fornece uma representação JSON do [objeto noncustodialDataSource.](../resources/ediscovery-noncustodialdatasource.md)</span><span class="sxs-lookup"><span data-stu-id="8df83-128">In the request body, supply a JSON representation of the [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object.</span></span>

<span data-ttu-id="8df83-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md).</span><span class="sxs-lookup"><span data-stu-id="8df83-129">The following table shows the properties that are required when you create the [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md).</span></span>

|<span data-ttu-id="8df83-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8df83-130">Property</span></span>|<span data-ttu-id="8df83-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8df83-131">Type</span></span>|<span data-ttu-id="8df83-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8df83-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8df83-133">@odata.id</span><span class="sxs-lookup"><span data-stu-id="8df83-133">@odata.id</span></span>|<span data-ttu-id="8df83-134">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="8df83-134">String</span></span>|<span data-ttu-id="8df83-135">Cadeia de caracteres que define o objeto custodial.</span><span class="sxs-lookup"><span data-stu-id="8df83-135">String that defines the custodial object.</span></span> <span data-ttu-id="8df83-136">Vejo o exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="8df83-136">See the example that follows.</span></span>  <span data-ttu-id="8df83-137">O @odata.id pode ser recuperado do [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md).</span><span class="sxs-lookup"><span data-stu-id="8df83-137">The @odata.id can be retrieved from the [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md).</span></span>|

## <a name="response"></a><span data-ttu-id="8df83-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8df83-138">Response</span></span>

<span data-ttu-id="8df83-139">Se tiver êxito, este método retornará um código de resposta e um `204 No Content` [objeto noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8df83-139">If successful, this method returns a `204 No Content` response code and a [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8df83-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8df83-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8df83-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8df83-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_noncustodialdatasource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/06d52284-ed81-49b8-904a-b863d3164731/sourceCollections/12aab1671c834213a84ba219c06f4c5a/noncustodialSources/$ref
Content-Type: application/json
Content-length: 206

{
    "@odata.id": "https://canary.graph.microsoft.com/testprodbetancsdsaslist/compliance/ediscovery/cases/06d52284-ed81-49b8-904a-b863d3164731/noncustodialDataSources/39383530323537383742433232433246"
}
```

### <a name="response"></a><span data-ttu-id="8df83-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8df83-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.noncustodialDataSource"
}
-->

``` http
HTTP/1.1 204 No Content
```
