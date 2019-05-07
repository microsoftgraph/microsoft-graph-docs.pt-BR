---
title: tipo de recurso secureScore
description: Representa a pontuação segura de um locatário por dia de dados de pontuação, no nível do locatário e do controle.
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 89842579457365f7da10509b2b4ade31f55de4f9
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629261"
---
# <a name="securescore-resource-type"></a><span data-ttu-id="412ad-103">tipo de recurso secureScore</span><span class="sxs-lookup"><span data-stu-id="412ad-103">secureScore resource type</span></span>

<span data-ttu-id="412ad-104">Representa a pontuação segura de um locatário por dia de dados de pontuação, no nível do locatário e do controle.</span><span class="sxs-lookup"><span data-stu-id="412ad-104">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="412ad-105">Por padrão, são mantidos 90 dias de dados.</span><span class="sxs-lookup"><span data-stu-id="412ad-105">By default, 90 days of data is held.</span></span> <span data-ttu-id="412ad-106">Esses dados são classificados por **createdDateTime**, do mais recente para o mais antigo.</span><span class="sxs-lookup"><span data-stu-id="412ad-106">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="412ad-107">Isso permitirá respostas de página usando $top = n, onde n = o número de dias de dados que você deseja recuperar.</span><span class="sxs-lookup"><span data-stu-id="412ad-107">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="412ad-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="412ad-108">Methods</span></span>

| <span data-ttu-id="412ad-109">Método</span><span class="sxs-lookup"><span data-stu-id="412ad-109">Method</span></span>   | <span data-ttu-id="412ad-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="412ad-110">Return Type</span></span>|<span data-ttu-id="412ad-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="412ad-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="412ad-112">Lista secureScores</span><span class="sxs-lookup"><span data-stu-id="412ad-112">List secureScores</span></span>](../api/security-list-securescores.md) | <span data-ttu-id="412ad-113">coleção [secureScores](securescore.md)</span><span class="sxs-lookup"><span data-stu-id="412ad-113">[secureScores](securescore.md) collection</span></span> |<span data-ttu-id="412ad-114">Obtém a coleção de objetos secureScore.</span><span class="sxs-lookup"><span data-stu-id="412ad-114">Get secureScore object collection.</span></span>|
|[<span data-ttu-id="412ad-115">Obter secureScore</span><span class="sxs-lookup"><span data-stu-id="412ad-115">Get secureScore</span></span>](../api/securescore-get.md) | [<span data-ttu-id="412ad-116">secureScore</span><span class="sxs-lookup"><span data-stu-id="412ad-116">secureScore</span></span>](securescore.md) |<span data-ttu-id="412ad-117">Leia as propriedades e os metadados de um objeto secureScore.</span><span class="sxs-lookup"><span data-stu-id="412ad-117">Read properties and metadata of a secureScore object.</span></span> | 



## <a name="properties"></a><span data-ttu-id="412ad-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="412ad-118">Properties</span></span>

|<span data-ttu-id="412ad-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="412ad-119">Property</span></span> |<span data-ttu-id="412ad-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="412ad-120">Type</span></span> |<span data-ttu-id="412ad-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="412ad-121">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="412ad-122">id</span><span class="sxs-lookup"><span data-stu-id="412ad-122">id</span></span> |<span data-ttu-id="412ad-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="412ad-123">String</span></span>|<span data-ttu-id="412ad-124">Identificador GUID/exclusivo gerado pelo provedor.</span><span class="sxs-lookup"><span data-stu-id="412ad-124">Provider-generated GUID/unique identifier.</span></span> <span data-ttu-id="412ad-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="412ad-125">Read-only.</span></span> <span data-ttu-id="412ad-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="412ad-126">Required.</span></span>|
|   <span data-ttu-id="412ad-127">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="412ad-127">azureTenantId</span></span>   |   <span data-ttu-id="412ad-128">String</span><span class="sxs-lookup"><span data-stu-id="412ad-128">String</span></span>  |   <span data-ttu-id="412ad-129">Cadeia de caracteres GUID para ID do locatário.</span><span class="sxs-lookup"><span data-stu-id="412ad-129">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="412ad-130">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="412ad-130">activeUserCount</span></span> |   <span data-ttu-id="412ad-131">Int32</span><span class="sxs-lookup"><span data-stu-id="412ad-131">Int32</span></span>   |   <span data-ttu-id="412ad-132">Contagem de usuários ativos de um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="412ad-132">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="412ad-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="412ad-133">createdDateTime</span></span> |   <span data-ttu-id="412ad-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="412ad-134">DateTimeOffset</span></span>  |   <span data-ttu-id="412ad-135">A data em que a entidade é criada.</span><span class="sxs-lookup"><span data-stu-id="412ad-135">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="412ad-136">currentScore</span><span class="sxs-lookup"><span data-stu-id="412ad-136">currentScore</span></span>    |   <span data-ttu-id="412ad-137">Duplo</span><span class="sxs-lookup"><span data-stu-id="412ad-137">Double</span></span>  |   <span data-ttu-id="412ad-138">Pontuação Obtida de locatário atual em data especificada.</span><span class="sxs-lookup"><span data-stu-id="412ad-138">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="412ad-139">enabledservices</span><span class="sxs-lookup"><span data-stu-id="412ad-139">enabledServices</span></span> |   <span data-ttu-id="412ad-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="412ad-140">String collection</span></span>   |   <span data-ttu-id="412ad-141">Serviços fornecidos pela Microsoft para o locatário (por exemplo, Exchange Online, Skype, SharePoint).</span><span class="sxs-lookup"><span data-stu-id="412ad-141">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="412ad-142">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="412ad-142">licensedUserCount</span></span>   |   <span data-ttu-id="412ad-143">Int32</span><span class="sxs-lookup"><span data-stu-id="412ad-143">Int32</span></span>   |   <span data-ttu-id="412ad-144">Contagem de usuários licenciados de um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="412ad-144">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="412ad-145">maxScore</span><span class="sxs-lookup"><span data-stu-id="412ad-145">maxScore</span></span> |  <span data-ttu-id="412ad-146">Duplo</span><span class="sxs-lookup"><span data-stu-id="412ad-146">Double</span></span>  |   <span data-ttu-id="412ad-147">Pontuação máxima possível de locatário na data especificada.</span><span class="sxs-lookup"><span data-stu-id="412ad-147">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="412ad-148">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="412ad-148">averageComparativeScores</span></span> |  <span data-ttu-id="412ad-149">coleção [averageComparativeScore](averagecomparativescore.md)</span><span class="sxs-lookup"><span data-stu-id="412ad-149">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="412ad-150">Pontuação média por escopos diferentes (por exemplo, média por setor, média por meio de assentos) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura) dentro do escopo.</span><span class="sxs-lookup"><span data-stu-id="412ad-150">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="412ad-151">controlScores</span><span class="sxs-lookup"><span data-stu-id="412ad-151">controlScores</span></span> | <span data-ttu-id="412ad-152">coleção [controlScore](controlscore.md)</span><span class="sxs-lookup"><span data-stu-id="412ad-152">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="412ad-153">Contém pontuações de locatários para um conjunto de controles.</span><span class="sxs-lookup"><span data-stu-id="412ad-153">Contains tenant scores for a set of controls.</span></span>   |
|<span data-ttu-id="412ad-154">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="412ad-154">vendorInformation</span></span> |[<span data-ttu-id="412ad-155">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="412ad-155">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="412ad-156">Tipo complexo que contém detalhes sobre o fornecedor de produtos/serviços de segurança, o provedor e o subfornecedor (por exemplo, fornecedor = Microsoft; Provider = SecureScore).</span><span class="sxs-lookup"><span data-stu-id="412ad-156">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore).</span></span> <span data-ttu-id="412ad-157">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="412ad-157">Required.</span></span>|


## <a name="relationships"></a><span data-ttu-id="412ad-158">Relações</span><span class="sxs-lookup"><span data-stu-id="412ad-158">Relationships</span></span>

<span data-ttu-id="412ad-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="412ad-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="412ad-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="412ad-160">JSON representation</span></span>

<span data-ttu-id="412ad-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="412ad-161">The following is a JSON representation of the resource.</span></span>

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
