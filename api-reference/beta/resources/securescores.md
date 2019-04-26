---
title: tipo de recurso secureScores
description: 'Top = n, onde n = o número de dias de dados que você deseja recuperar. '
localization_priority: Normal
ms.openlocfilehash: 8b4be9822b782303efe38dbdf5bd43e1ee543421
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549188"
---
# <a name="securescores-resource-type"></a><span data-ttu-id="67b96-103">tipo de recurso secureScores</span><span class="sxs-lookup"><span data-stu-id="67b96-103">secureScores resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67b96-104">Representa a pontuação segura de um locatário por dia de dados de pontuação, no nível do locatário e do controle.</span><span class="sxs-lookup"><span data-stu-id="67b96-104">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="67b96-105">Por padrão, são mantidos 90 dias de dados.</span><span class="sxs-lookup"><span data-stu-id="67b96-105">By default, 90 days of data is held.</span></span> <span data-ttu-id="67b96-106">Esses dados são classificados por **createdDateTime**, do mais recente para o mais antigo.</span><span class="sxs-lookup"><span data-stu-id="67b96-106">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="67b96-107">Isso permitirá respostas de página usando $top = n, onde n = o número de dias de dados que você deseja recuperar.</span><span class="sxs-lookup"><span data-stu-id="67b96-107">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="67b96-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="67b96-108">Methods</span></span>

| <span data-ttu-id="67b96-109">Método</span><span class="sxs-lookup"><span data-stu-id="67b96-109">Method</span></span>   | <span data-ttu-id="67b96-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="67b96-110">Return Type</span></span>|<span data-ttu-id="67b96-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="67b96-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="67b96-112">Lista secureScores</span><span class="sxs-lookup"><span data-stu-id="67b96-112">List secureScores</span></span>](../api/securescores-list.md) | [<span data-ttu-id="67b96-113">secureScores</span><span class="sxs-lookup"><span data-stu-id="67b96-113">secureScores</span></span>](securescores.md) |<span data-ttu-id="67b96-114">Leia as propriedades e os metadados de um objeto secureScores.</span><span class="sxs-lookup"><span data-stu-id="67b96-114">Read properties and metadata of a secureScores object.</span></span>|


## <a name="properties"></a><span data-ttu-id="67b96-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="67b96-115">Properties</span></span>
<span data-ttu-id="67b96-116">Tipo de entidade contendo propriedades da Pontuação de segurança do locatário (dados de instantâneos diários).</span><span class="sxs-lookup"><span data-stu-id="67b96-116">Entity type containing properties of the tenant security score (daily snapshot data).</span></span>

|<span data-ttu-id="67b96-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67b96-117">Property</span></span> |<span data-ttu-id="67b96-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="67b96-118">Type</span></span> |<span data-ttu-id="67b96-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="67b96-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="67b96-120">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="67b96-120">azureTenantId</span></span>   |   <span data-ttu-id="67b96-121">String</span><span class="sxs-lookup"><span data-stu-id="67b96-121">String</span></span>  |   <span data-ttu-id="67b96-122">Cadeia de caracteres GUID para ID do locatário.</span><span class="sxs-lookup"><span data-stu-id="67b96-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="67b96-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67b96-123">createdDateTime</span></span> |   <span data-ttu-id="67b96-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67b96-124">DateTimeOffset</span></span>  |   <span data-ttu-id="67b96-125">A data em que a entidade é criada.</span><span class="sxs-lookup"><span data-stu-id="67b96-125">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="67b96-126">id</span><span class="sxs-lookup"><span data-stu-id="67b96-126">id</span></span>  |   <span data-ttu-id="67b96-127">String</span><span class="sxs-lookup"><span data-stu-id="67b96-127">String</span></span>  |   <span data-ttu-id="67b96-128">Combinação de azureTenantId_createdDateTime.</span><span class="sxs-lookup"><span data-stu-id="67b96-128">Combination of azureTenantId_createdDateTime.</span></span>   |
|   <span data-ttu-id="67b96-129">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="67b96-129">licensedUserCount</span></span>   |   <span data-ttu-id="67b96-130">Int32</span><span class="sxs-lookup"><span data-stu-id="67b96-130">Int32</span></span>   |   <span data-ttu-id="67b96-131">Contagem de usuários licenciados de um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="67b96-131">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="67b96-132">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="67b96-132">activeUserCount</span></span> |   <span data-ttu-id="67b96-133">Int32</span><span class="sxs-lookup"><span data-stu-id="67b96-133">Int32</span></span>   |   <span data-ttu-id="67b96-134">Contagem de usuários ativos de um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="67b96-134">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="67b96-135">currentScore</span><span class="sxs-lookup"><span data-stu-id="67b96-135">currentScore</span></span>    |   <span data-ttu-id="67b96-136">Duplo</span><span class="sxs-lookup"><span data-stu-id="67b96-136">Double</span></span>  |   <span data-ttu-id="67b96-137">Pontuação Obtida de locatário atual em data especificada.</span><span class="sxs-lookup"><span data-stu-id="67b96-137">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="67b96-138">maxScore</span><span class="sxs-lookup"><span data-stu-id="67b96-138">maxScore</span></span> |  <span data-ttu-id="67b96-139">Duplo</span><span class="sxs-lookup"><span data-stu-id="67b96-139">Double</span></span>  |   <span data-ttu-id="67b96-140">Pontuação máxima possível de locatário na data especificada.</span><span class="sxs-lookup"><span data-stu-id="67b96-140">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="67b96-141">enabledservices</span><span class="sxs-lookup"><span data-stu-id="67b96-141">enabledServices</span></span> |   <span data-ttu-id="67b96-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="67b96-142">String collection</span></span>   |   <span data-ttu-id="67b96-143">Serviços fornecidos pela Microsoft para o locatário (por exemplo, Exchange Online, Skype, SharePoint).</span><span class="sxs-lookup"><span data-stu-id="67b96-143">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="67b96-144">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="67b96-144">averageComparativeScores</span></span> |  <span data-ttu-id="67b96-145">coleção [averageComparativeScore](averagecomparativescore.md)</span><span class="sxs-lookup"><span data-stu-id="67b96-145">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="67b96-146">Pontuação média por escopos diferentes (por exemplo, média por setor, média por meio de assentos) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura) dentro do escopo.</span><span class="sxs-lookup"><span data-stu-id="67b96-146">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="67b96-147">controlScores</span><span class="sxs-lookup"><span data-stu-id="67b96-147">controlScores</span></span> | <span data-ttu-id="67b96-148">coleção [controlScore](controlscore.md)</span><span class="sxs-lookup"><span data-stu-id="67b96-148">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="67b96-149">Contém pontuações de locatários para um conjunto de controles.</span><span class="sxs-lookup"><span data-stu-id="67b96-149">Contains tenant scores for a set of controls.</span></span>   |


## <a name="relationships"></a><span data-ttu-id="67b96-150">Relações</span><span class="sxs-lookup"><span data-stu-id="67b96-150">Relationships</span></span>

<span data-ttu-id="67b96-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="67b96-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="67b96-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="67b96-152">JSON representation</span></span>

<span data-ttu-id="67b96-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="67b96-153">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScores"
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
}

```


<!--
{
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securescores.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
