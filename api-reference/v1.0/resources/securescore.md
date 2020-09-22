---
title: tipo de recurso secureScore
description: Representa a pontuação segura de um locatário por dia de dados de pontuação, no nível do locatário e do controle.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e4f798ae64b881c95ed4330901c0a34ba4073f0e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984093"
---
# <a name="securescore-resource-type"></a><span data-ttu-id="23ee3-103">tipo de recurso secureScore</span><span class="sxs-lookup"><span data-stu-id="23ee3-103">secureScore resource type</span></span>

<span data-ttu-id="23ee3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23ee3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="23ee3-105">Representa a pontuação segura de um locatário por dia de dados de pontuação, no nível do locatário e do controle.</span><span class="sxs-lookup"><span data-stu-id="23ee3-105">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="23ee3-106">Por padrão, são mantidos 90 dias de dados.</span><span class="sxs-lookup"><span data-stu-id="23ee3-106">By default, 90 days of data is held.</span></span> <span data-ttu-id="23ee3-107">Esses dados são classificados por **createdDateTime**, do mais recente para o mais antigo.</span><span class="sxs-lookup"><span data-stu-id="23ee3-107">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="23ee3-108">Isso permitirá respostas de página usando $top = n, onde n = o número de dias de dados que você deseja recuperar.</span><span class="sxs-lookup"><span data-stu-id="23ee3-108">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="23ee3-109">Methods</span><span class="sxs-lookup"><span data-stu-id="23ee3-109">Methods</span></span>

| <span data-ttu-id="23ee3-110">Método</span><span class="sxs-lookup"><span data-stu-id="23ee3-110">Method</span></span>   | <span data-ttu-id="23ee3-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="23ee3-111">Return Type</span></span>|<span data-ttu-id="23ee3-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="23ee3-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="23ee3-113">Lista secureScores</span><span class="sxs-lookup"><span data-stu-id="23ee3-113">List secureScores</span></span>](../api/security-list-securescores.md) | <span data-ttu-id="23ee3-114">coleção [secureScores](securescore.md)</span><span class="sxs-lookup"><span data-stu-id="23ee3-114">[secureScores](securescore.md) collection</span></span> |<span data-ttu-id="23ee3-115">Obtém a coleção de objetos secureScore.</span><span class="sxs-lookup"><span data-stu-id="23ee3-115">Get secureScore object collection.</span></span>|
|[<span data-ttu-id="23ee3-116">Obter secureScore</span><span class="sxs-lookup"><span data-stu-id="23ee3-116">Get secureScore</span></span>](../api/securescore-get.md) | [<span data-ttu-id="23ee3-117">secureScore</span><span class="sxs-lookup"><span data-stu-id="23ee3-117">secureScore</span></span>](securescore.md) |<span data-ttu-id="23ee3-118">Leia as propriedades e os metadados de um objeto secureScore.</span><span class="sxs-lookup"><span data-stu-id="23ee3-118">Read properties and metadata of a secureScore object.</span></span> | 



## <a name="properties"></a><span data-ttu-id="23ee3-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23ee3-119">Properties</span></span>

|<span data-ttu-id="23ee3-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23ee3-120">Property</span></span> |<span data-ttu-id="23ee3-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="23ee3-121">Type</span></span> |<span data-ttu-id="23ee3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="23ee3-122">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="23ee3-123">id</span><span class="sxs-lookup"><span data-stu-id="23ee3-123">id</span></span> |<span data-ttu-id="23ee3-124">String</span><span class="sxs-lookup"><span data-stu-id="23ee3-124">String</span></span>|<span data-ttu-id="23ee3-125">Identificador GUID/exclusivo gerado pelo provedor.</span><span class="sxs-lookup"><span data-stu-id="23ee3-125">Provider-generated GUID/unique identifier.</span></span> <span data-ttu-id="23ee3-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23ee3-126">Read-only.</span></span> <span data-ttu-id="23ee3-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23ee3-127">Required.</span></span>|
|   <span data-ttu-id="23ee3-128">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="23ee3-128">azureTenantId</span></span>   |   <span data-ttu-id="23ee3-129">String</span><span class="sxs-lookup"><span data-stu-id="23ee3-129">String</span></span>  |   <span data-ttu-id="23ee3-130">Cadeia de caracteres GUID para ID do locatário.</span><span class="sxs-lookup"><span data-stu-id="23ee3-130">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="23ee3-131">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="23ee3-131">activeUserCount</span></span> |   <span data-ttu-id="23ee3-132">Int32</span><span class="sxs-lookup"><span data-stu-id="23ee3-132">Int32</span></span>   |   <span data-ttu-id="23ee3-133">Contagem de usuários ativos de um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="23ee3-133">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="23ee3-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23ee3-134">createdDateTime</span></span> |   <span data-ttu-id="23ee3-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23ee3-135">DateTimeOffset</span></span>  |   <span data-ttu-id="23ee3-136">A data em que a entidade é criada.</span><span class="sxs-lookup"><span data-stu-id="23ee3-136">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="23ee3-137">currentScore</span><span class="sxs-lookup"><span data-stu-id="23ee3-137">currentScore</span></span>    |   <span data-ttu-id="23ee3-138">Duplo</span><span class="sxs-lookup"><span data-stu-id="23ee3-138">Double</span></span>  |   <span data-ttu-id="23ee3-139">Pontuação Obtida de locatário atual em data especificada.</span><span class="sxs-lookup"><span data-stu-id="23ee3-139">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="23ee3-140">enabledservices</span><span class="sxs-lookup"><span data-stu-id="23ee3-140">enabledServices</span></span> |   <span data-ttu-id="23ee3-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="23ee3-141">String collection</span></span>   |   <span data-ttu-id="23ee3-142">Serviços fornecidos pela Microsoft para o locatário (por exemplo, Exchange Online, Skype, SharePoint).</span><span class="sxs-lookup"><span data-stu-id="23ee3-142">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="23ee3-143">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="23ee3-143">licensedUserCount</span></span>   |   <span data-ttu-id="23ee3-144">Int32</span><span class="sxs-lookup"><span data-stu-id="23ee3-144">Int32</span></span>   |   <span data-ttu-id="23ee3-145">Contagem de usuários licenciados de um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="23ee3-145">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="23ee3-146">maxScore</span><span class="sxs-lookup"><span data-stu-id="23ee3-146">maxScore</span></span> |  <span data-ttu-id="23ee3-147">Duplo</span><span class="sxs-lookup"><span data-stu-id="23ee3-147">Double</span></span>  |   <span data-ttu-id="23ee3-148">Pontuação máxima possível de locatário na data especificada.</span><span class="sxs-lookup"><span data-stu-id="23ee3-148">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="23ee3-149">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="23ee3-149">averageComparativeScores</span></span> |  <span data-ttu-id="23ee3-150">coleção [averageComparativeScore](averagecomparativescore.md)</span><span class="sxs-lookup"><span data-stu-id="23ee3-150">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="23ee3-151">Pontuação média por escopos diferentes (por exemplo, média por setor, média por meio de assentos) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura) dentro do escopo.</span><span class="sxs-lookup"><span data-stu-id="23ee3-151">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="23ee3-152">controlScores</span><span class="sxs-lookup"><span data-stu-id="23ee3-152">controlScores</span></span> | <span data-ttu-id="23ee3-153">coleção [controlScore](controlscore.md)</span><span class="sxs-lookup"><span data-stu-id="23ee3-153">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="23ee3-154">Contém pontuações de locatários para um conjunto de controles.</span><span class="sxs-lookup"><span data-stu-id="23ee3-154">Contains tenant scores for a set of controls.</span></span>   |
|<span data-ttu-id="23ee3-155">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="23ee3-155">vendorInformation</span></span> |[<span data-ttu-id="23ee3-156">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="23ee3-156">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="23ee3-157">Tipo complexo que contém detalhes sobre o fornecedor de produtos/serviços de segurança, o provedor e o subfornecedor (por exemplo, fornecedor = Microsoft; Provider = SecureScore).</span><span class="sxs-lookup"><span data-stu-id="23ee3-157">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore).</span></span> <span data-ttu-id="23ee3-158">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23ee3-158">Required.</span></span>|


## <a name="relationships"></a><span data-ttu-id="23ee3-159">Relações</span><span class="sxs-lookup"><span data-stu-id="23ee3-159">Relationships</span></span>

<span data-ttu-id="23ee3-160">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23ee3-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="23ee3-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23ee3-161">JSON representation</span></span>

<span data-ttu-id="23ee3-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23ee3-162">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScore"
}-->

```json
{
"id": "String (identifier)",
"azureTenantId": "String",
"activeUserCount": "Int32",
"createdDateTime": "String (timestamp)",
"currentScore": "Double",
"enabledServices": ["String"],
"licensedUserCount": "Int32",
"maxScore": "Double",
"averageComparativeScores": [{"@odata.type": "microsoft.graph.averageComparativeScore"}],
"controlScores": [{"@odata.type": "microsoft.graph.controlScore"}],
"vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "secureScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

