---
title: tipo de recurso secureScore
description: Representa a pontuação segura de um locatário por dia de dados de pontuação, no nível do locatário e do controle.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1fc789a967f8fbba33e113dd55e7bfae7803940e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446930"
---
# <a name="securescore-resource-type"></a><span data-ttu-id="3c833-103">tipo de recurso secureScore</span><span class="sxs-lookup"><span data-stu-id="3c833-103">secureScore resource type</span></span>

<span data-ttu-id="3c833-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3c833-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3c833-105">Representa a pontuação segura de um locatário por dia de dados de pontuação, no nível do locatário e do controle.</span><span class="sxs-lookup"><span data-stu-id="3c833-105">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="3c833-106">Por padrão, são mantidos 90 dias de dados.</span><span class="sxs-lookup"><span data-stu-id="3c833-106">By default, 90 days of data is held.</span></span> <span data-ttu-id="3c833-107">Esses dados são classificados por **createdDateTime**, do mais recente para o mais antigo.</span><span class="sxs-lookup"><span data-stu-id="3c833-107">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="3c833-108">Isso permitirá respostas de página usando $top = n, onde n = o número de dias de dados que você deseja recuperar.</span><span class="sxs-lookup"><span data-stu-id="3c833-108">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="3c833-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="3c833-109">Methods</span></span>

| <span data-ttu-id="3c833-110">Método</span><span class="sxs-lookup"><span data-stu-id="3c833-110">Method</span></span>   | <span data-ttu-id="3c833-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3c833-111">Return Type</span></span>|<span data-ttu-id="3c833-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c833-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3c833-113">Lista secureScores</span><span class="sxs-lookup"><span data-stu-id="3c833-113">List secureScores</span></span>](../api/security-list-securescores.md) | <span data-ttu-id="3c833-114">coleção [secureScores](securescore.md)</span><span class="sxs-lookup"><span data-stu-id="3c833-114">[secureScores](securescore.md) collection</span></span> |<span data-ttu-id="3c833-115">Obtém a coleção de objetos secureScore.</span><span class="sxs-lookup"><span data-stu-id="3c833-115">Get secureScore object collection.</span></span>|
|[<span data-ttu-id="3c833-116">Obter secureScore</span><span class="sxs-lookup"><span data-stu-id="3c833-116">Get secureScore</span></span>](../api/securescore-get.md) | [<span data-ttu-id="3c833-117">secureScore</span><span class="sxs-lookup"><span data-stu-id="3c833-117">secureScore</span></span>](securescore.md) |<span data-ttu-id="3c833-118">Leia as propriedades e os metadados de um objeto secureScore.</span><span class="sxs-lookup"><span data-stu-id="3c833-118">Read properties and metadata of a secureScore object.</span></span> | 



## <a name="properties"></a><span data-ttu-id="3c833-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c833-119">Properties</span></span>

|<span data-ttu-id="3c833-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c833-120">Property</span></span> |<span data-ttu-id="3c833-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c833-121">Type</span></span> |<span data-ttu-id="3c833-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c833-122">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="3c833-123">id</span><span class="sxs-lookup"><span data-stu-id="3c833-123">id</span></span> |<span data-ttu-id="3c833-124">String</span><span class="sxs-lookup"><span data-stu-id="3c833-124">String</span></span>|<span data-ttu-id="3c833-125">Identificador GUID/exclusivo gerado pelo provedor.</span><span class="sxs-lookup"><span data-stu-id="3c833-125">Provider-generated GUID/unique identifier.</span></span> <span data-ttu-id="3c833-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3c833-126">Read-only.</span></span> <span data-ttu-id="3c833-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c833-127">Required.</span></span>|
|   <span data-ttu-id="3c833-128">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="3c833-128">azureTenantId</span></span>   |   <span data-ttu-id="3c833-129">String</span><span class="sxs-lookup"><span data-stu-id="3c833-129">String</span></span>  |   <span data-ttu-id="3c833-130">Cadeia de caracteres GUID para ID do locatário.</span><span class="sxs-lookup"><span data-stu-id="3c833-130">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="3c833-131">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="3c833-131">activeUserCount</span></span> |   <span data-ttu-id="3c833-132">Int32</span><span class="sxs-lookup"><span data-stu-id="3c833-132">Int32</span></span>   |   <span data-ttu-id="3c833-133">Contagem de usuários ativos de um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="3c833-133">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="3c833-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c833-134">createdDateTime</span></span> |   <span data-ttu-id="3c833-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c833-135">DateTimeOffset</span></span>  |   <span data-ttu-id="3c833-136">A data em que a entidade é criada.</span><span class="sxs-lookup"><span data-stu-id="3c833-136">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="3c833-137">currentScore</span><span class="sxs-lookup"><span data-stu-id="3c833-137">currentScore</span></span>    |   <span data-ttu-id="3c833-138">Duplo</span><span class="sxs-lookup"><span data-stu-id="3c833-138">Double</span></span>  |   <span data-ttu-id="3c833-139">Pontuação Obtida de locatário atual em data especificada.</span><span class="sxs-lookup"><span data-stu-id="3c833-139">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="3c833-140">enabledservices</span><span class="sxs-lookup"><span data-stu-id="3c833-140">enabledServices</span></span> |   <span data-ttu-id="3c833-141">String collection</span><span class="sxs-lookup"><span data-stu-id="3c833-141">String collection</span></span>   |   <span data-ttu-id="3c833-142">Serviços fornecidos pela Microsoft para o locatário (por exemplo, Exchange Online, Skype, SharePoint).</span><span class="sxs-lookup"><span data-stu-id="3c833-142">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="3c833-143">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="3c833-143">licensedUserCount</span></span>   |   <span data-ttu-id="3c833-144">Int32</span><span class="sxs-lookup"><span data-stu-id="3c833-144">Int32</span></span>   |   <span data-ttu-id="3c833-145">Contagem de usuários licenciados de um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="3c833-145">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="3c833-146">maxScore</span><span class="sxs-lookup"><span data-stu-id="3c833-146">maxScore</span></span> |  <span data-ttu-id="3c833-147">Duplo</span><span class="sxs-lookup"><span data-stu-id="3c833-147">Double</span></span>  |   <span data-ttu-id="3c833-148">Pontuação máxima possível de locatário na data especificada.</span><span class="sxs-lookup"><span data-stu-id="3c833-148">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="3c833-149">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="3c833-149">averageComparativeScores</span></span> |  <span data-ttu-id="3c833-150">coleção [averageComparativeScore](averagecomparativescore.md)</span><span class="sxs-lookup"><span data-stu-id="3c833-150">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="3c833-151">Pontuação média por escopos diferentes (por exemplo, média por setor, média por meio de assentos) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura) dentro do escopo.</span><span class="sxs-lookup"><span data-stu-id="3c833-151">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="3c833-152">controlScores</span><span class="sxs-lookup"><span data-stu-id="3c833-152">controlScores</span></span> | <span data-ttu-id="3c833-153">coleção [controlScore](controlscore.md)</span><span class="sxs-lookup"><span data-stu-id="3c833-153">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="3c833-154">Contém pontuações de locatários para um conjunto de controles.</span><span class="sxs-lookup"><span data-stu-id="3c833-154">Contains tenant scores for a set of controls.</span></span>   |
|<span data-ttu-id="3c833-155">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="3c833-155">vendorInformation</span></span> |[<span data-ttu-id="3c833-156">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="3c833-156">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="3c833-157">Tipo complexo que contém detalhes sobre o fornecedor de produtos/serviços de segurança, o provedor e o subfornecedor (por exemplo, fornecedor = Microsoft; Provider = SecureScore).</span><span class="sxs-lookup"><span data-stu-id="3c833-157">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore).</span></span> <span data-ttu-id="3c833-158">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c833-158">Required.</span></span>|


## <a name="relationships"></a><span data-ttu-id="3c833-159">Relações</span><span class="sxs-lookup"><span data-stu-id="3c833-159">Relationships</span></span>

<span data-ttu-id="3c833-160">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3c833-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c833-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c833-161">JSON representation</span></span>

<span data-ttu-id="3c833-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c833-162">The following is a JSON representation of the resource.</span></span>

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
