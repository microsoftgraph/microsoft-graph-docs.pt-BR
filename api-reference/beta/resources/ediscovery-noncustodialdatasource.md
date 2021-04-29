---
title: Tipo de recurso noncustodialDataSource
description: Fontes de dados não custodiais permitem adicionar dados a um caso sem precisar associá-los a um custodiante
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 1e7dd0d656a58e65e460742158cdcc70da1f1d5a
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080751"
---
# <a name="noncustodialdatasource-resource-type"></a><span data-ttu-id="86962-103">Tipo de recurso noncustodialDataSource</span><span class="sxs-lookup"><span data-stu-id="86962-103">noncustodialDataSource resource type</span></span>

<span data-ttu-id="86962-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="86962-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86962-105">Fontes de dados não custodiais permitem adicionar dados a um caso sem precisar associá-los a um custodiante.</span><span class="sxs-lookup"><span data-stu-id="86962-105">Non-custodial data sources let you add data to a case without having to associate it to a custodian.</span></span> <span data-ttu-id="86962-106">Para saber mais, visite Adicionar fontes de dados não [custodiais a um Advanced eDiscovery caso](https://docs.microsoft.com/microsoft-365/compliance/non-custodial-data-sources)</span><span class="sxs-lookup"><span data-stu-id="86962-106">To learn more, visit [Add non-custodial data sources to an Advanced eDiscovery case ](https://docs.microsoft.com/microsoft-365/compliance/non-custodial-data-sources)</span></span>

<span data-ttu-id="86962-107">Herda de [dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span><span class="sxs-lookup"><span data-stu-id="86962-107">Inherits from [dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span></span>

## <a name="methods"></a><span data-ttu-id="86962-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="86962-108">Methods</span></span>

|<span data-ttu-id="86962-109">Método</span><span class="sxs-lookup"><span data-stu-id="86962-109">Method</span></span>|<span data-ttu-id="86962-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="86962-110">Return type</span></span>|<span data-ttu-id="86962-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="86962-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="86962-112">Listar noncustodialDataSources</span><span class="sxs-lookup"><span data-stu-id="86962-112">List noncustodialDataSources</span></span>](../api/ediscovery-noncustodialdatasource-list.md)|<span data-ttu-id="86962-113">[coleção microsoft.graph.ediscovery.noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md)</span><span class="sxs-lookup"><span data-stu-id="86962-113">[microsoft.graph.ediscovery.noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) collection</span></span>|<span data-ttu-id="86962-114">Obter uma lista dos [objetos noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="86962-114">Get a list of the [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) objects and their properties.</span></span>|
|[<span data-ttu-id="86962-115">Obter noncustodialDataSource</span><span class="sxs-lookup"><span data-stu-id="86962-115">Get noncustodialDataSource</span></span>](../api/ediscovery-noncustodialdatasource-get.md)|[<span data-ttu-id="86962-116">microsoft.graph.ediscovery.noncustodialDataSource</span><span class="sxs-lookup"><span data-stu-id="86962-116">microsoft.graph.ediscovery.noncustodialDataSource</span></span>](../resources/ediscovery-noncustodialdatasource.md)|<span data-ttu-id="86962-117">Leia as propriedades e as relações de [um objeto noncustodialDataSource.](../resources/ediscovery-noncustodialdatasource.md)</span><span class="sxs-lookup"><span data-stu-id="86962-117">Read the properties and relationships of a [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object.</span></span>|
|[<span data-ttu-id="86962-118">Liberar dadosSource</span><span class="sxs-lookup"><span data-stu-id="86962-118">Release dataSource</span></span>](../api/ediscovery-noncustodialdatasource-release.md)|<span data-ttu-id="86962-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="86962-119">None</span></span>|<span data-ttu-id="86962-120">Libera uma fonte de dados não custodiada.</span><span class="sxs-lookup"><span data-stu-id="86962-120">Releases a non-custodial data source.</span></span>|
|[<span data-ttu-id="86962-121">Listar dadosSource</span><span class="sxs-lookup"><span data-stu-id="86962-121">List dataSource</span></span>](../api/ediscovery-noncustodialdatasource-list-datasource.md)|<span data-ttu-id="86962-122">[coleção microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)</span><span class="sxs-lookup"><span data-stu-id="86962-122">[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) collection</span></span>|<span data-ttu-id="86962-123">Obter os recursos dataSource da propriedade de navegação dataSource.</span><span class="sxs-lookup"><span data-stu-id="86962-123">Get the dataSource resources from the dataSource navigation property.</span></span>|
|[<span data-ttu-id="86962-124">Criar dataSource</span><span class="sxs-lookup"><span data-stu-id="86962-124">Create dataSource</span></span>](../api/ediscovery-noncustodialdatasource-post.md)|[<span data-ttu-id="86962-125">microsoft.graph.ediscovery.dataSource</span><span class="sxs-lookup"><span data-stu-id="86962-125">microsoft.graph.ediscovery.dataSource</span></span>](../resources/ediscovery-datasource.md)|<span data-ttu-id="86962-126">Crie um novo objeto dataSource.</span><span class="sxs-lookup"><span data-stu-id="86962-126">Create a new dataSource object.</span></span>|

## <a name="properties"></a><span data-ttu-id="86962-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="86962-127">Properties</span></span>

|<span data-ttu-id="86962-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86962-128">Property</span></span>|<span data-ttu-id="86962-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="86962-129">Type</span></span>|<span data-ttu-id="86962-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="86962-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86962-131">applyHoldToSource</span><span class="sxs-lookup"><span data-stu-id="86962-131">applyHoldToSource</span></span>|<span data-ttu-id="86962-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="86962-132">Boolean</span></span>|<span data-ttu-id="86962-133">Indica se a espera é aplicada à fonte de dados não custodial (como caixa de correio ou site).</span><span class="sxs-lookup"><span data-stu-id="86962-133">Indicates if hold is applied to non-custodial data source (such as mailbox or site).</span></span>|
|<span data-ttu-id="86962-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86962-134">createdDateTime</span></span>|<span data-ttu-id="86962-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86962-135">DateTimeOffset</span></span>|<span data-ttu-id="86962-136">Data e hora criadas do nonCustodialDataSource.</span><span class="sxs-lookup"><span data-stu-id="86962-136">Created date and time of the nonCustodialDataSource.</span></span> <span data-ttu-id="86962-137">Herdado [de microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span><span class="sxs-lookup"><span data-stu-id="86962-137">Inherited from [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span></span>|
|<span data-ttu-id="86962-138">displayName</span><span class="sxs-lookup"><span data-stu-id="86962-138">displayName</span></span>|<span data-ttu-id="86962-139">String</span><span class="sxs-lookup"><span data-stu-id="86962-139">String</span></span>|<span data-ttu-id="86962-140">Nome de exibição do noncustodialDataSource.</span><span class="sxs-lookup"><span data-stu-id="86962-140">Display name of the noncustodialDataSource.</span></span> <span data-ttu-id="86962-141">Herdado [de microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span><span class="sxs-lookup"><span data-stu-id="86962-141">Inherited from [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span></span>|
|<span data-ttu-id="86962-142">id</span><span class="sxs-lookup"><span data-stu-id="86962-142">id</span></span>|<span data-ttu-id="86962-143">String</span><span class="sxs-lookup"><span data-stu-id="86962-143">String</span></span>|<span data-ttu-id="86962-144">Identificador exclusivo do nonCustodialDataSource.</span><span class="sxs-lookup"><span data-stu-id="86962-144">Unique identifier of the nonCustodialDataSource.</span></span> <span data-ttu-id="86962-145">Herdado da [entidade](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="86962-145">Inherited from [entity](../resources/entity.md).</span></span>|
|<span data-ttu-id="86962-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86962-146">lastModifiedDateTime</span></span>|<span data-ttu-id="86962-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86962-147">DateTimeOffset</span></span>|<span data-ttu-id="86962-148">Data e hora da última modificação do nonCustodialDataSource.</span><span class="sxs-lookup"><span data-stu-id="86962-148">Last modified date and time of the nonCustodialDataSource.</span></span> <span data-ttu-id="86962-149">Herdado [de microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span><span class="sxs-lookup"><span data-stu-id="86962-149">Inherited from [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span></span>|
|<span data-ttu-id="86962-150">releasedDateTime</span><span class="sxs-lookup"><span data-stu-id="86962-150">releasedDateTime</span></span>|<span data-ttu-id="86962-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86962-151">DateTimeOffset</span></span>|<span data-ttu-id="86962-152">Data e hora em que o nonCustodialDataSource foi liberado do caso.</span><span class="sxs-lookup"><span data-stu-id="86962-152">Date and time that the nonCustodialDataSource was released from the case.</span></span> <span data-ttu-id="86962-153">Herdado [de microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span><span class="sxs-lookup"><span data-stu-id="86962-153">Inherited from [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span></span>|
|<span data-ttu-id="86962-154">status</span><span class="sxs-lookup"><span data-stu-id="86962-154">status</span></span>|<span data-ttu-id="86962-155">microsoft.graph.ediscovery.dataSourceContainerStatus</span><span class="sxs-lookup"><span data-stu-id="86962-155">microsoft.graph.ediscovery.dataSourceContainerStatus</span></span>|<span data-ttu-id="86962-156">Status mais recente do nonCustodialDataSource.</span><span class="sxs-lookup"><span data-stu-id="86962-156">Latest status of the nonCustodialDataSource.</span></span> <span data-ttu-id="86962-157">Herdado [de microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span><span class="sxs-lookup"><span data-stu-id="86962-157">Inherited from [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span></span> <span data-ttu-id="86962-158">Os valores possíveis são: `Active`, `Released`.</span><span class="sxs-lookup"><span data-stu-id="86962-158">Possible values are: `Active`, `Released`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86962-159">Relações</span><span class="sxs-lookup"><span data-stu-id="86962-159">Relationships</span></span>

|<span data-ttu-id="86962-160">Relação</span><span class="sxs-lookup"><span data-stu-id="86962-160">Relationship</span></span>|<span data-ttu-id="86962-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="86962-161">Type</span></span>|<span data-ttu-id="86962-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="86962-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86962-163">dataSource</span><span class="sxs-lookup"><span data-stu-id="86962-163">dataSource</span></span>|[<span data-ttu-id="86962-164">microsoft.graph.ediscovery.dataSource</span><span class="sxs-lookup"><span data-stu-id="86962-164">microsoft.graph.ediscovery.dataSource</span></span>](../resources/ediscovery-datasource.md)|<span data-ttu-id="86962-165">Fonte de usuário ou SharePoint de dados do site como fonte de dados não custodiada.</span><span class="sxs-lookup"><span data-stu-id="86962-165">User source or SharePoint site data source as non-custodial data source.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="86962-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="86962-166">JSON representation</span></span>

<span data-ttu-id="86962-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="86962-167">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.noncustodialDataSource",
  "baseType": "microsoft.graph.ediscovery.dataSourceContainer",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.noncustodialDataSource",
  "id": "String (identifier)",
  "status": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "applyHoldToSource": "Boolean"
}
```
