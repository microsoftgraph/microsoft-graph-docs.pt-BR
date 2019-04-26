---
title: tipo de recurso secureScore
description: 'Top = n, onde n = o número de dias de dados que você deseja recuperar. '
localization_priority: Normal
ms.openlocfilehash: 1f4ee37b5e257cfb914f45a1260f3572403f00dd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343370"
---
# <a name="securescore-resource-type"></a><span data-ttu-id="d25b4-103">tipo de recurso secureScore</span><span class="sxs-lookup"><span data-stu-id="d25b4-103">secureScore resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d25b4-104">Representa a pontuação segura de um locatário por dia de dados de pontuação, no nível do locatário e do controle.</span><span class="sxs-lookup"><span data-stu-id="d25b4-104">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="d25b4-105">Por padrão, são mantidos 90 dias de dados.</span><span class="sxs-lookup"><span data-stu-id="d25b4-105">By default, 90 days of data is held.</span></span> <span data-ttu-id="d25b4-106">Esses dados são classificados por **createdDateTime**, do mais recente para o mais antigo.</span><span class="sxs-lookup"><span data-stu-id="d25b4-106">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="d25b4-107">Isso permitirá respostas de página usando $top = n, onde n = o número de dias de dados que você deseja recuperar.</span><span class="sxs-lookup"><span data-stu-id="d25b4-107">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="d25b4-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="d25b4-108">Methods</span></span>

| <span data-ttu-id="d25b4-109">Método</span><span class="sxs-lookup"><span data-stu-id="d25b4-109">Method</span></span>   | <span data-ttu-id="d25b4-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d25b4-110">Return Type</span></span>|<span data-ttu-id="d25b4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d25b4-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d25b4-112">Lista secureScores</span><span class="sxs-lookup"><span data-stu-id="d25b4-112">List secureScores</span></span>](../api/securescores-list.md) | [<span data-ttu-id="d25b4-113">secureScores</span><span class="sxs-lookup"><span data-stu-id="d25b4-113">secureScores</span></span>](securescores.md) |<span data-ttu-id="d25b4-114">Leia as propriedades e os metadados de um objeto secureScores.</span><span class="sxs-lookup"><span data-stu-id="d25b4-114">Read properties and metadata of a secureScores object.</span></span>|


## <a name="properties"></a><span data-ttu-id="d25b4-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d25b4-115">Properties</span></span>
<span data-ttu-id="d25b4-116">Tipo de entidade contendo propriedades da Pontuação de segurança do locatário (dados de instantâneos diários).</span><span class="sxs-lookup"><span data-stu-id="d25b4-116">Entity type containing properties of the tenant security score (daily snapshot data).</span></span>

|<span data-ttu-id="d25b4-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d25b4-117">Property</span></span> |<span data-ttu-id="d25b4-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="d25b4-118">Type</span></span> |<span data-ttu-id="d25b4-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d25b4-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="d25b4-120">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="d25b4-120">azureTenantId</span></span>   |   <span data-ttu-id="d25b4-121">String</span><span class="sxs-lookup"><span data-stu-id="d25b4-121">String</span></span>  |   <span data-ttu-id="d25b4-122">Cadeia de caracteres GUID para ID do locatário.</span><span class="sxs-lookup"><span data-stu-id="d25b4-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="d25b4-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d25b4-123">createdDateTime</span></span> |   <span data-ttu-id="d25b4-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d25b4-124">DateTimeOffset</span></span>  |   <span data-ttu-id="d25b4-125">A data em que a entidade é criada.</span><span class="sxs-lookup"><span data-stu-id="d25b4-125">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="d25b4-126">id</span><span class="sxs-lookup"><span data-stu-id="d25b4-126">id</span></span>  |   <span data-ttu-id="d25b4-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d25b4-127">String</span></span>  |   <span data-ttu-id="d25b4-128">Combinação de azureTenantId_createdDateTime.</span><span class="sxs-lookup"><span data-stu-id="d25b4-128">Combination of azureTenantId_createdDateTime.</span></span>   |
|   <span data-ttu-id="d25b4-129">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="d25b4-129">licensedUserCount</span></span>   |   <span data-ttu-id="d25b4-130">Int32</span><span class="sxs-lookup"><span data-stu-id="d25b4-130">Int32</span></span>   |   <span data-ttu-id="d25b4-131">Contagem de usuários licenciados de um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="d25b4-131">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="d25b4-132">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="d25b4-132">activeUserCount</span></span> |   <span data-ttu-id="d25b4-133">Int32</span><span class="sxs-lookup"><span data-stu-id="d25b4-133">Int32</span></span>   |   <span data-ttu-id="d25b4-134">Contagem de usuários ativos de um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="d25b4-134">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="d25b4-135">currentScore</span><span class="sxs-lookup"><span data-stu-id="d25b4-135">currentScore</span></span>    |   <span data-ttu-id="d25b4-136">Duplo</span><span class="sxs-lookup"><span data-stu-id="d25b4-136">Double</span></span>  |   <span data-ttu-id="d25b4-137">Pontuação Obtida de locatário atual em data especificada.</span><span class="sxs-lookup"><span data-stu-id="d25b4-137">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="d25b4-138">maxScore</span><span class="sxs-lookup"><span data-stu-id="d25b4-138">maxScore</span></span> |  <span data-ttu-id="d25b4-139">Duplo</span><span class="sxs-lookup"><span data-stu-id="d25b4-139">Double</span></span>  |   <span data-ttu-id="d25b4-140">Pontuação máxima possível de locatário na data especificada.</span><span class="sxs-lookup"><span data-stu-id="d25b4-140">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="d25b4-141">enabledservices</span><span class="sxs-lookup"><span data-stu-id="d25b4-141">enabledServices</span></span> |   <span data-ttu-id="d25b4-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="d25b4-142">String collection</span></span>   |   <span data-ttu-id="d25b4-143">Serviços fornecidos pela Microsoft para o locatário (por exemplo, Exchange Online, Skype, SharePoint).</span><span class="sxs-lookup"><span data-stu-id="d25b4-143">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="d25b4-144">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="d25b4-144">averageComparativeScores</span></span> |  <span data-ttu-id="d25b4-145">coleção [averageComparativeScore](averagecomparativescore.md)</span><span class="sxs-lookup"><span data-stu-id="d25b4-145">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="d25b4-146">Pontuação média por escopos diferentes (por exemplo, média por setor, média por meio de assentos) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura) dentro do escopo.</span><span class="sxs-lookup"><span data-stu-id="d25b4-146">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="d25b4-147">controlScores</span><span class="sxs-lookup"><span data-stu-id="d25b4-147">controlScores</span></span> | <span data-ttu-id="d25b4-148">coleção [controlScore](controlscore.md)</span><span class="sxs-lookup"><span data-stu-id="d25b4-148">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="d25b4-149">Contém pontuações de locatários para um conjunto de controles.</span><span class="sxs-lookup"><span data-stu-id="d25b4-149">Contains tenant scores for a set of controls.</span></span>   |


## <a name="relationships"></a><span data-ttu-id="d25b4-150">Relações</span><span class="sxs-lookup"><span data-stu-id="d25b4-150">Relationships</span></span>

<span data-ttu-id="d25b4-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d25b4-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d25b4-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d25b4-152">JSON representation</span></span>

<span data-ttu-id="d25b4-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d25b4-153">The following is a JSON representation of the resource.</span></span>

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
