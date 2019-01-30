---
title: tipo de recurso de secureScores
description: 'superior = n, onde n = o número de dias de dados que você deseja recuperar. '
localization_priority: Normal
ms.openlocfilehash: 8b4be9822b782303efe38dbdf5bd43e1ee543421
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640179"
---
# <a name="securescores-resource-type"></a><span data-ttu-id="3b877-103">tipo de recurso de secureScores</span><span class="sxs-lookup"><span data-stu-id="3b877-103">secureScores resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b877-104">Representa a pontuação seguro de um locatário por dia da pontuação de dados, no nível de locatário e controle.</span><span class="sxs-lookup"><span data-stu-id="3b877-104">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="3b877-105">Por padrão, 90 dias de dados é mantido.</span><span class="sxs-lookup"><span data-stu-id="3b877-105">By default, 90 days of data is held.</span></span> <span data-ttu-id="3b877-106">Esses dados são classificados pelo **createdDateTime**, do mais recente à mais antiga.</span><span class="sxs-lookup"><span data-stu-id="3b877-106">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="3b877-107">Isso permitirá que você para respostas da página usando $top = n, onde n = o número de dias de dados que você deseja recuperar.</span><span class="sxs-lookup"><span data-stu-id="3b877-107">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="3b877-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="3b877-108">Methods</span></span>

| <span data-ttu-id="3b877-109">Método</span><span class="sxs-lookup"><span data-stu-id="3b877-109">Method</span></span>   | <span data-ttu-id="3b877-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3b877-110">Return Type</span></span>|<span data-ttu-id="3b877-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b877-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3b877-112">Lista secureScores</span><span class="sxs-lookup"><span data-stu-id="3b877-112">List secureScores</span></span>](../api/securescores-list.md) | [<span data-ttu-id="3b877-113">secureScores</span><span class="sxs-lookup"><span data-stu-id="3b877-113">secureScores</span></span>](securescores.md) |<span data-ttu-id="3b877-114">Leia as propriedades e os metadados de um objeto secureScores.</span><span class="sxs-lookup"><span data-stu-id="3b877-114">Read properties and metadata of a secureScores object.</span></span>|


## <a name="properties"></a><span data-ttu-id="3b877-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3b877-115">Properties</span></span>
<span data-ttu-id="3b877-116">Propriedades que contêm de tipo de entidade de segurança locatário pontuação (dados diários de instantâneo).</span><span class="sxs-lookup"><span data-stu-id="3b877-116">Entity type containing properties of the tenant security score (daily snapshot data).</span></span>

|<span data-ttu-id="3b877-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b877-117">Property</span></span> |<span data-ttu-id="3b877-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b877-118">Type</span></span> |<span data-ttu-id="3b877-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b877-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="3b877-120">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="3b877-120">azureTenantId</span></span>   |   <span data-ttu-id="3b877-121">String</span><span class="sxs-lookup"><span data-stu-id="3b877-121">String</span></span>  |   <span data-ttu-id="3b877-122">ID de cadeia de caracteres do GUID para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="3b877-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="3b877-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b877-123">createdDateTime</span></span> |   <span data-ttu-id="3b877-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b877-124">DateTimeOffset</span></span>  |   <span data-ttu-id="3b877-125">A data em que a entidade é criada.</span><span class="sxs-lookup"><span data-stu-id="3b877-125">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="3b877-126">id</span><span class="sxs-lookup"><span data-stu-id="3b877-126">id</span></span>  |   <span data-ttu-id="3b877-127">String</span><span class="sxs-lookup"><span data-stu-id="3b877-127">String</span></span>  |   <span data-ttu-id="3b877-128">Combinação de azureTenantId_createdDateTime.</span><span class="sxs-lookup"><span data-stu-id="3b877-128">Combination of azureTenantId_createdDateTime.</span></span>   |
|   <span data-ttu-id="3b877-129">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="3b877-129">licensedUserCount</span></span>   |   <span data-ttu-id="3b877-130">Int32</span><span class="sxs-lookup"><span data-stu-id="3b877-130">Int32</span></span>   |   <span data-ttu-id="3b877-131">Licenciado contagem de usuários do determinado inquilino.</span><span class="sxs-lookup"><span data-stu-id="3b877-131">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="3b877-132">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="3b877-132">activeUserCount</span></span> |   <span data-ttu-id="3b877-133">Int32</span><span class="sxs-lookup"><span data-stu-id="3b877-133">Int32</span></span>   |   <span data-ttu-id="3b877-134">Contagem de usuário ativo do determinado inquilino.</span><span class="sxs-lookup"><span data-stu-id="3b877-134">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="3b877-135">currentScore</span><span class="sxs-lookup"><span data-stu-id="3b877-135">currentScore</span></span>    |   <span data-ttu-id="3b877-136">Duplo</span><span class="sxs-lookup"><span data-stu-id="3b877-136">Double</span></span>  |   <span data-ttu-id="3b877-137">Pontuação de locatário atual que já alcançou na data especificada.</span><span class="sxs-lookup"><span data-stu-id="3b877-137">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="3b877-138">maxScore</span><span class="sxs-lookup"><span data-stu-id="3b877-138">maxScore</span></span> |  <span data-ttu-id="3b877-139">Duplo</span><span class="sxs-lookup"><span data-stu-id="3b877-139">Double</span></span>  |   <span data-ttu-id="3b877-140">Locatário pontuação possíveis máxima na data especificada.</span><span class="sxs-lookup"><span data-stu-id="3b877-140">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="3b877-141">enabledServices</span><span class="sxs-lookup"><span data-stu-id="3b877-141">enabledServices</span></span> |   <span data-ttu-id="3b877-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b877-142">String collection</span></span>   |   <span data-ttu-id="3b877-143">Serviços fornecida pela Microsoft para o locatário (por exemplo, Exchange online, Skype, Sharepoint).</span><span class="sxs-lookup"><span data-stu-id="3b877-143">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="3b877-144">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="3b877-144">averageComparativeScores</span></span> |  <span data-ttu-id="3b877-145">coleção [averageComparativeScore](averagecomparativescore.md)</span><span class="sxs-lookup"><span data-stu-id="3b877-145">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="3b877-146">Pontuação média por escopos diferentes (por exemplo, média por setor, média por assentos) e a categoria de controle (identidade, dados, dispositivo, aplicativos, infra-estrutura) dentro do escopo.</span><span class="sxs-lookup"><span data-stu-id="3b877-146">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="3b877-147">controlScores</span><span class="sxs-lookup"><span data-stu-id="3b877-147">controlScores</span></span> | <span data-ttu-id="3b877-148">coleção [controlScore](controlscore.md)</span><span class="sxs-lookup"><span data-stu-id="3b877-148">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="3b877-149">Contém as pontuações de locatário de um conjunto de controles.</span><span class="sxs-lookup"><span data-stu-id="3b877-149">Contains tenant scores for a set of controls.</span></span>   |


## <a name="relationships"></a><span data-ttu-id="3b877-150">Relações</span><span class="sxs-lookup"><span data-stu-id="3b877-150">Relationships</span></span>

<span data-ttu-id="3b877-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3b877-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b877-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3b877-152">JSON representation</span></span>

<span data-ttu-id="3b877-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3b877-153">The following is a JSON representation of the resource.</span></span>

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
