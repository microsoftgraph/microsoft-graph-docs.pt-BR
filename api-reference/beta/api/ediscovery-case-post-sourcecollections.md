---
title: Criar sourceCollection
description: Crie um novo objeto sourceCollection.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 69476c91acffc6d0a1edc8a18cc4208c5239fa26
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445826"
---
# <a name="create-sourcecollection"></a><span data-ttu-id="d53db-103">Criar sourceCollection</span><span class="sxs-lookup"><span data-stu-id="d53db-103">Create sourceCollection</span></span>

<span data-ttu-id="d53db-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="d53db-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d53db-105">Crie um novo [objeto sourceCollection.](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d53db-105">Create a new [sourceCollection](../resources/ediscovery-sourcecollection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d53db-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d53db-106">Permissions</span></span>

<span data-ttu-id="d53db-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d53db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d53db-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d53db-109">Permission type</span></span>|<span data-ttu-id="d53db-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d53db-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d53db-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d53db-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d53db-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d53db-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="d53db-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d53db-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d53db-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d53db-114">Not supported.</span></span>|
|<span data-ttu-id="d53db-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d53db-115">Application</span></span>|<span data-ttu-id="d53db-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d53db-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d53db-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d53db-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections
```

## <a name="request-headers"></a><span data-ttu-id="d53db-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d53db-118">Request headers</span></span>

|<span data-ttu-id="d53db-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d53db-119">Name</span></span>|<span data-ttu-id="d53db-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d53db-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d53db-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d53db-121">Authorization</span></span>|<span data-ttu-id="d53db-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d53db-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d53db-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d53db-124">Content-Type</span></span>|<span data-ttu-id="d53db-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d53db-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d53db-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d53db-127">Request body</span></span>

<span data-ttu-id="d53db-128">No corpo da solicitação, fornece uma representação JSON do [objeto sourceCollection.](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d53db-128">In the request body, supply a JSON representation of the [sourceCollection](../resources/ediscovery-sourcecollection.md) object.</span></span>

<span data-ttu-id="d53db-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [sourceCollection](../resources/ediscovery-sourcecollection.md).</span><span class="sxs-lookup"><span data-stu-id="d53db-129">The following table shows the properties that are required when you create the [sourceCollection](../resources/ediscovery-sourcecollection.md).</span></span>

|<span data-ttu-id="d53db-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d53db-130">Property</span></span>|<span data-ttu-id="d53db-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d53db-131">Type</span></span>|<span data-ttu-id="d53db-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d53db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d53db-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d53db-133">displayName</span></span>|<span data-ttu-id="d53db-134">String</span><span class="sxs-lookup"><span data-stu-id="d53db-134">String</span></span>|<span data-ttu-id="d53db-135">O nome de exibição da **sourceCollection**</span><span class="sxs-lookup"><span data-stu-id="d53db-135">The display name of the **sourceCollection**</span></span>|
|<span data-ttu-id="d53db-136">custodianSources</span><span class="sxs-lookup"><span data-stu-id="d53db-136">custodianSources</span></span>|<span data-ttu-id="d53db-137">[coleção microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)</span><span class="sxs-lookup"><span data-stu-id="d53db-137">[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) collection</span></span>|<span data-ttu-id="d53db-138">As fontes custodiadas a incluir nesta pesquisa.</span><span class="sxs-lookup"><span data-stu-id="d53db-138">The custodian sources to include in this search.</span></span> <span data-ttu-id="d53db-139">Você pode obter a URL do [site custodianteSources,](../api/ediscovery-custodian-list-sitesources.md) [unifiedGroupSources](../api/ediscovery-custodian-list-unifiedgroupsources.md)ou [userSources](../api/ediscovery-custodian-list-usersources.md) mais a ID da origem.</span><span class="sxs-lookup"><span data-stu-id="d53db-139">You can get the URL from from custodian [siteSources](../api/ediscovery-custodian-list-sitesources.md), [unifiedGroupSources](../api/ediscovery-custodian-list-unifiedgroupsources.md), or [userSources](../api/ediscovery-custodian-list-usersources.md) plus the ID of the source.</span></span> <span data-ttu-id="d53db-140">**Observação:** Um custodiante ou a especificação da origem do locatário é necessário ao criar uma coleção de origem.</span><span class="sxs-lookup"><span data-stu-id="d53db-140">**Note:** Either one custodian or specifying tenant source is required when creating a source collection.</span></span> |
|<span data-ttu-id="d53db-141">tenantSources</span><span class="sxs-lookup"><span data-stu-id="d53db-141">tenantSources</span></span>|<span data-ttu-id="d53db-142">microsoft.graph.ediscovery.tenantSources</span><span class="sxs-lookup"><span data-stu-id="d53db-142">microsoft.graph.ediscovery.tenantSources</span></span>|<span data-ttu-id="d53db-143">Quando especificado, a coleção se estenderá por um serviço para uma carga de trabalho inteira.</span><span class="sxs-lookup"><span data-stu-id="d53db-143">When specified, the collection will span across a service for an entire workload.</span></span> <span data-ttu-id="d53db-144">Os valores possíveis são: `allMailboxes` e `allSites`.</span><span class="sxs-lookup"><span data-stu-id="d53db-144">Possible values are: `allMailboxes`, `allSites`.</span></span> <span data-ttu-id="d53db-145">**Observação:** Um custodiante ou a especificação da origem do locatário é necessário ao criar uma coleção de origem.</span><span class="sxs-lookup"><span data-stu-id="d53db-145">**Note:** Either one custodian or specifying tenant source is required when creating a source collection.</span></span>|

## <a name="response"></a><span data-ttu-id="d53db-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="d53db-146">Response</span></span>

<span data-ttu-id="d53db-147">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d53db-147">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d53db-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d53db-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d53db-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d53db-149">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_sourcecollection_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourceCollections
Content-Type: application/json
Content-length: 272

{
    "displayName": "Quarterly Financials search",
    "contentQuery": "subject:'Quarterly Financials'",
    "custodianSources@odata.bind": [
        "https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735"
    ]
}
```

### <a name="response"></a><span data-ttu-id="d53db-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="d53db-150">Response</span></span>

<span data-ttu-id="d53db-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d53db-151">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.sourceCollection"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourceCollections/$entity",
    "description": null,
    "lastModifiedDateTime": "2021-01-12T18:09:03.7378679Z",
    "contentQuery": "subject:'Quarterly Financials'",
    "tenantSources": "none",
    "id": "1a9b4145d8f84e39bc45a7f68c5c5119",
    "displayName": "Quarterly Financials search",
    "createdDateTime": "2021-01-12T18:09:03.417009Z",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "EDisco Admin",
            "userPrincipalname": "admin@contoso.com"
        }
    },
    "lastModifiedBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "EDisco Admin",
            "userPrincipalname": "admin@contoso.com"
        }
    }
}
```
