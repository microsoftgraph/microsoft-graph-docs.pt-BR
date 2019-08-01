---
title: tipo de recurso secureScore
description: Representa a pontuação segura de um locatário por dia de dados de pontuação, no nível do locatário e do controle.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 395c5ed0594d1f509bb664b5aee6ea18bb42af0a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034479"
---
# <a name="securescore-resource-type"></a><span data-ttu-id="6850b-103">tipo de recurso secureScore</span><span class="sxs-lookup"><span data-stu-id="6850b-103">secureScore resource type</span></span>

<span data-ttu-id="6850b-104">Representa a pontuação segura de um locatário por dia de dados de pontuação, no nível do locatário e do controle.</span><span class="sxs-lookup"><span data-stu-id="6850b-104">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="6850b-105">Por padrão, são mantidos 90 dias de dados.</span><span class="sxs-lookup"><span data-stu-id="6850b-105">By default, 90 days of data is held.</span></span> <span data-ttu-id="6850b-106">Esses dados são classificados por **createdDateTime**, do mais recente para o mais antigo.</span><span class="sxs-lookup"><span data-stu-id="6850b-106">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="6850b-107">Isso permitirá respostas de página usando $top = n, onde n = o número de dias de dados que você deseja recuperar.</span><span class="sxs-lookup"><span data-stu-id="6850b-107">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="6850b-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="6850b-108">Methods</span></span>

| <span data-ttu-id="6850b-109">Método</span><span class="sxs-lookup"><span data-stu-id="6850b-109">Method</span></span>   | <span data-ttu-id="6850b-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6850b-110">Return Type</span></span>|<span data-ttu-id="6850b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6850b-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6850b-112">Lista secureScores</span><span class="sxs-lookup"><span data-stu-id="6850b-112">List secureScores</span></span>](../api/security-list-securescores.md) | <span data-ttu-id="6850b-113">coleção [secureScores](securescore.md)</span><span class="sxs-lookup"><span data-stu-id="6850b-113">[secureScores](securescore.md) collection</span></span> |<span data-ttu-id="6850b-114">Obtém a coleção de objetos secureScore.</span><span class="sxs-lookup"><span data-stu-id="6850b-114">Get secureScore object collection.</span></span>|
|[<span data-ttu-id="6850b-115">Obter secureScore</span><span class="sxs-lookup"><span data-stu-id="6850b-115">Get secureScore</span></span>](../api/securescore-get.md) | [<span data-ttu-id="6850b-116">secureScore</span><span class="sxs-lookup"><span data-stu-id="6850b-116">secureScore</span></span>](securescore.md) |<span data-ttu-id="6850b-117">Leia as propriedades e os metadados de um objeto secureScore.</span><span class="sxs-lookup"><span data-stu-id="6850b-117">Read properties and metadata of a secureScore object.</span></span> | 



## <a name="properties"></a><span data-ttu-id="6850b-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6850b-118">Properties</span></span>

|<span data-ttu-id="6850b-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6850b-119">Property</span></span> |<span data-ttu-id="6850b-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="6850b-120">Type</span></span> |<span data-ttu-id="6850b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6850b-121">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="6850b-122">id</span><span class="sxs-lookup"><span data-stu-id="6850b-122">id</span></span> |<span data-ttu-id="6850b-123">String</span><span class="sxs-lookup"><span data-stu-id="6850b-123">String</span></span>|<span data-ttu-id="6850b-124">Identificador GUID/exclusivo gerado pelo provedor.</span><span class="sxs-lookup"><span data-stu-id="6850b-124">Provider-generated GUID/unique identifier.</span></span> <span data-ttu-id="6850b-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6850b-125">Read-only.</span></span> <span data-ttu-id="6850b-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6850b-126">Required.</span></span>|
|   <span data-ttu-id="6850b-127">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="6850b-127">azureTenantId</span></span>   |   <span data-ttu-id="6850b-128">String</span><span class="sxs-lookup"><span data-stu-id="6850b-128">String</span></span>  |   <span data-ttu-id="6850b-129">Cadeia de caracteres GUID para ID do locatário.</span><span class="sxs-lookup"><span data-stu-id="6850b-129">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="6850b-130">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="6850b-130">activeUserCount</span></span> |   <span data-ttu-id="6850b-131">Int32</span><span class="sxs-lookup"><span data-stu-id="6850b-131">Int32</span></span>   |   <span data-ttu-id="6850b-132">Contagem de usuários ativos de um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="6850b-132">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="6850b-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6850b-133">createdDateTime</span></span> |   <span data-ttu-id="6850b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6850b-134">DateTimeOffset</span></span>  |   <span data-ttu-id="6850b-135">A data em que a entidade é criada.</span><span class="sxs-lookup"><span data-stu-id="6850b-135">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="6850b-136">currentScore</span><span class="sxs-lookup"><span data-stu-id="6850b-136">currentScore</span></span>    |   <span data-ttu-id="6850b-137">Duplo</span><span class="sxs-lookup"><span data-stu-id="6850b-137">Double</span></span>  |   <span data-ttu-id="6850b-138">Pontuação Obtida de locatário atual em data especificada.</span><span class="sxs-lookup"><span data-stu-id="6850b-138">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="6850b-139">enabledservices</span><span class="sxs-lookup"><span data-stu-id="6850b-139">enabledServices</span></span> |   <span data-ttu-id="6850b-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6850b-140">String collection</span></span>   |   <span data-ttu-id="6850b-141">Serviços fornecidos pela Microsoft para o locatário (por exemplo, Exchange Online, Skype, SharePoint).</span><span class="sxs-lookup"><span data-stu-id="6850b-141">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="6850b-142">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="6850b-142">licensedUserCount</span></span>   |   <span data-ttu-id="6850b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="6850b-143">Int32</span></span>   |   <span data-ttu-id="6850b-144">Contagem de usuários licenciados de um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="6850b-144">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="6850b-145">maxScore</span><span class="sxs-lookup"><span data-stu-id="6850b-145">maxScore</span></span> |  <span data-ttu-id="6850b-146">Duplo</span><span class="sxs-lookup"><span data-stu-id="6850b-146">Double</span></span>  |   <span data-ttu-id="6850b-147">Pontuação máxima possível de locatário na data especificada.</span><span class="sxs-lookup"><span data-stu-id="6850b-147">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="6850b-148">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="6850b-148">averageComparativeScores</span></span> |  <span data-ttu-id="6850b-149">coleção [averageComparativeScore](averagecomparativescore.md)</span><span class="sxs-lookup"><span data-stu-id="6850b-149">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="6850b-150">Pontuação média por escopos diferentes (por exemplo, média por setor, média por meio de assentos) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura) dentro do escopo.</span><span class="sxs-lookup"><span data-stu-id="6850b-150">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="6850b-151">controlScores</span><span class="sxs-lookup"><span data-stu-id="6850b-151">controlScores</span></span> | <span data-ttu-id="6850b-152">coleção [controlScore](controlscore.md)</span><span class="sxs-lookup"><span data-stu-id="6850b-152">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="6850b-153">Contém pontuações de locatários para um conjunto de controles.</span><span class="sxs-lookup"><span data-stu-id="6850b-153">Contains tenant scores for a set of controls.</span></span>   |
|<span data-ttu-id="6850b-154">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="6850b-154">vendorInformation</span></span> |[<span data-ttu-id="6850b-155">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="6850b-155">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="6850b-156">Tipo complexo que contém detalhes sobre o fornecedor de produtos/serviços de segurança, o provedor e o subfornecedor (por exemplo, fornecedor = Microsoft; Provider = SecureScore).</span><span class="sxs-lookup"><span data-stu-id="6850b-156">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore).</span></span> <span data-ttu-id="6850b-157">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6850b-157">Required.</span></span>|


## <a name="relationships"></a><span data-ttu-id="6850b-158">Relações</span><span class="sxs-lookup"><span data-stu-id="6850b-158">Relationships</span></span>

<span data-ttu-id="6850b-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6850b-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6850b-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6850b-160">JSON representation</span></span>

<span data-ttu-id="6850b-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6850b-161">The following is a JSON representation of the resource.</span></span>

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
