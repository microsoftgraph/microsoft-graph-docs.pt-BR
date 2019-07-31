---
title: tipo de recurso secureScore
description: 'Top = n, onde n = o número de dias de dados que você deseja recuperar. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d1db0e97c88f4532bad2052f77a3513084c74aa7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008583"
---
# <a name="securescore-resource-type"></a><span data-ttu-id="812bd-103">tipo de recurso secureScore</span><span class="sxs-lookup"><span data-stu-id="812bd-103">secureScore resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="812bd-104">Representa a pontuação segura de um locatário por dia de dados de pontuação, no nível do locatário e do controle.</span><span class="sxs-lookup"><span data-stu-id="812bd-104">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="812bd-105">Por padrão, são mantidos 90 dias de dados.</span><span class="sxs-lookup"><span data-stu-id="812bd-105">By default, 90 days of data is held.</span></span> <span data-ttu-id="812bd-106">Esses dados são classificados por **createdDateTime**, do mais recente para o mais antigo.</span><span class="sxs-lookup"><span data-stu-id="812bd-106">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="812bd-107">Isso permitirá respostas de página usando $top = n, onde n = o número de dias de dados que você deseja recuperar.</span><span class="sxs-lookup"><span data-stu-id="812bd-107">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="812bd-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="812bd-108">Methods</span></span>

| <span data-ttu-id="812bd-109">Método</span><span class="sxs-lookup"><span data-stu-id="812bd-109">Method</span></span>   | <span data-ttu-id="812bd-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="812bd-110">Return Type</span></span>|<span data-ttu-id="812bd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="812bd-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="812bd-112">Lista secureScores</span><span class="sxs-lookup"><span data-stu-id="812bd-112">List secureScores</span></span>](../api/securescores-list.md) | [<span data-ttu-id="812bd-113">secureScores</span><span class="sxs-lookup"><span data-stu-id="812bd-113">secureScores</span></span>](securescores.md) |<span data-ttu-id="812bd-114">Leia as propriedades e os metadados de um objeto secureScores.</span><span class="sxs-lookup"><span data-stu-id="812bd-114">Read properties and metadata of a secureScores object.</span></span>|


## <a name="properties"></a><span data-ttu-id="812bd-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="812bd-115">Properties</span></span>
<span data-ttu-id="812bd-116">Tipo de entidade contendo propriedades da Pontuação de segurança do locatário (dados de instantâneos diários).</span><span class="sxs-lookup"><span data-stu-id="812bd-116">Entity type containing properties of the tenant security score (daily snapshot data).</span></span>

|<span data-ttu-id="812bd-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="812bd-117">Property</span></span> |<span data-ttu-id="812bd-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="812bd-118">Type</span></span> |<span data-ttu-id="812bd-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="812bd-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="812bd-120">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="812bd-120">azureTenantId</span></span>   |   <span data-ttu-id="812bd-121">String</span><span class="sxs-lookup"><span data-stu-id="812bd-121">String</span></span>  |   <span data-ttu-id="812bd-122">Cadeia de caracteres GUID para ID do locatário.</span><span class="sxs-lookup"><span data-stu-id="812bd-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="812bd-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="812bd-123">createdDateTime</span></span> |   <span data-ttu-id="812bd-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="812bd-124">DateTimeOffset</span></span>  |   <span data-ttu-id="812bd-125">A data em que a entidade é criada.</span><span class="sxs-lookup"><span data-stu-id="812bd-125">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="812bd-126">id</span><span class="sxs-lookup"><span data-stu-id="812bd-126">id</span></span>  |   <span data-ttu-id="812bd-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="812bd-127">String</span></span>  |   <span data-ttu-id="812bd-128">Combinação de azureTenantId_createdDateTime.</span><span class="sxs-lookup"><span data-stu-id="812bd-128">Combination of azureTenantId_createdDateTime.</span></span>   |
|   <span data-ttu-id="812bd-129">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="812bd-129">licensedUserCount</span></span>   |   <span data-ttu-id="812bd-130">Int32</span><span class="sxs-lookup"><span data-stu-id="812bd-130">Int32</span></span>   |   <span data-ttu-id="812bd-131">Contagem de usuários licenciados de um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="812bd-131">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="812bd-132">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="812bd-132">activeUserCount</span></span> |   <span data-ttu-id="812bd-133">Int32</span><span class="sxs-lookup"><span data-stu-id="812bd-133">Int32</span></span>   |   <span data-ttu-id="812bd-134">Contagem de usuários ativos de um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="812bd-134">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="812bd-135">currentScore</span><span class="sxs-lookup"><span data-stu-id="812bd-135">currentScore</span></span>    |   <span data-ttu-id="812bd-136">Duplo</span><span class="sxs-lookup"><span data-stu-id="812bd-136">Double</span></span>  |   <span data-ttu-id="812bd-137">Pontuação Obtida de locatário atual em data especificada.</span><span class="sxs-lookup"><span data-stu-id="812bd-137">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="812bd-138">maxScore</span><span class="sxs-lookup"><span data-stu-id="812bd-138">maxScore</span></span> |  <span data-ttu-id="812bd-139">Duplo</span><span class="sxs-lookup"><span data-stu-id="812bd-139">Double</span></span>  |   <span data-ttu-id="812bd-140">Pontuação máxima possível de locatário na data especificada.</span><span class="sxs-lookup"><span data-stu-id="812bd-140">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="812bd-141">enabledservices</span><span class="sxs-lookup"><span data-stu-id="812bd-141">enabledServices</span></span> |   <span data-ttu-id="812bd-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="812bd-142">String collection</span></span>   |   <span data-ttu-id="812bd-143">Serviços fornecidos pela Microsoft para o locatário (por exemplo, Exchange Online, Skype, SharePoint).</span><span class="sxs-lookup"><span data-stu-id="812bd-143">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="812bd-144">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="812bd-144">averageComparativeScores</span></span> |  <span data-ttu-id="812bd-145">coleção [averageComparativeScore](averagecomparativescore.md)</span><span class="sxs-lookup"><span data-stu-id="812bd-145">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="812bd-146">Pontuação média por escopos diferentes (por exemplo, média por setor, média por meio de assentos) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura) dentro do escopo.</span><span class="sxs-lookup"><span data-stu-id="812bd-146">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="812bd-147">controlScores</span><span class="sxs-lookup"><span data-stu-id="812bd-147">controlScores</span></span> | <span data-ttu-id="812bd-148">coleção [controlScore](controlscore.md)</span><span class="sxs-lookup"><span data-stu-id="812bd-148">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="812bd-149">Contém pontuações de locatários para um conjunto de controles.</span><span class="sxs-lookup"><span data-stu-id="812bd-149">Contains tenant scores for a set of controls.</span></span>   |


## <a name="relationships"></a><span data-ttu-id="812bd-150">Relações</span><span class="sxs-lookup"><span data-stu-id="812bd-150">Relationships</span></span>

<span data-ttu-id="812bd-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="812bd-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="812bd-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="812bd-152">JSON representation</span></span>

<span data-ttu-id="812bd-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="812bd-153">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScore"
}-->

```json
{
  "id": "String",
  "azureTenantId": "Guid",
  "createdDate": "DateTimeOffset",
  "licensedUserCount": "Int32",
  "activeUserCount": "Int32",
  "currentScore": "Int32",
  "maxScore": "Int32",
  "averageScore": "Double",
  "enabledServices": "Collection(string)",
  "averageComparativeScores": "Collection(microsoft.graph.SecureScore.averageComparativeScores)",
  "controlScores": "Collection(microsoft.graph.SecureScore.controlScores)",
  "createdDateTime": "2019-02-07T20:33:53.156Z"
}

```


<!--
{
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
