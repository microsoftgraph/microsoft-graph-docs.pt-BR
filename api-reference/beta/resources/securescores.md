---
title: tipo de recurso secureScore
description: 'Top = n, onde n = o número de dias de dados que você deseja recuperar. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 2deb3a4ab39b169778ad43f60170e51eaa32eda9
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810409"
---
# <a name="securescore-resource-type"></a><span data-ttu-id="a1420-103">tipo de recurso secureScore</span><span class="sxs-lookup"><span data-stu-id="a1420-103">secureScore resource type</span></span>

<span data-ttu-id="a1420-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1420-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1420-105">Representa a pontuação segura de um locatário por dia de dados de pontuação, no nível do locatário e do controle.</span><span class="sxs-lookup"><span data-stu-id="a1420-105">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="a1420-106">Por padrão, são mantidos 90 dias de dados.</span><span class="sxs-lookup"><span data-stu-id="a1420-106">By default, 90 days of data is held.</span></span> <span data-ttu-id="a1420-107">Esses dados são classificados por **createdDateTime**, do mais recente para o mais antigo.</span><span class="sxs-lookup"><span data-stu-id="a1420-107">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="a1420-108">Isso permitirá respostas de página usando $top = n, onde n = o número de dias de dados que você deseja recuperar.</span><span class="sxs-lookup"><span data-stu-id="a1420-108">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span>


## <a name="methods"></a><span data-ttu-id="a1420-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="a1420-109">Methods</span></span>

| <span data-ttu-id="a1420-110">Método</span><span class="sxs-lookup"><span data-stu-id="a1420-110">Method</span></span>   | <span data-ttu-id="a1420-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a1420-111">Return Type</span></span>|<span data-ttu-id="a1420-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1420-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a1420-113">Lista secureScores</span><span class="sxs-lookup"><span data-stu-id="a1420-113">List secureScores</span></span>](../api/securescores-list.md) | [<span data-ttu-id="a1420-114">secureScores</span><span class="sxs-lookup"><span data-stu-id="a1420-114">secureScores</span></span>](securescores.md) |<span data-ttu-id="a1420-115">Leia as propriedades e os metadados de um objeto secureScores.</span><span class="sxs-lookup"><span data-stu-id="a1420-115">Read properties and metadata of a secureScores object.</span></span>|


## <a name="properties"></a><span data-ttu-id="a1420-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a1420-116">Properties</span></span>
<span data-ttu-id="a1420-117">Tipo de entidade contendo propriedades da Pontuação de segurança do locatário (dados de instantâneos diários).</span><span class="sxs-lookup"><span data-stu-id="a1420-117">Entity type containing properties of the tenant security score (daily snapshot data).</span></span>

|<span data-ttu-id="a1420-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1420-118">Property</span></span> |<span data-ttu-id="a1420-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1420-119">Type</span></span> |<span data-ttu-id="a1420-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1420-120">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="a1420-121">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="a1420-121">azureTenantId</span></span>   |   <span data-ttu-id="a1420-122">String</span><span class="sxs-lookup"><span data-stu-id="a1420-122">String</span></span>  |   <span data-ttu-id="a1420-123">Cadeia de caracteres GUID para ID do locatário.</span><span class="sxs-lookup"><span data-stu-id="a1420-123">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="a1420-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1420-124">createdDateTime</span></span> |   <span data-ttu-id="a1420-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1420-125">DateTimeOffset</span></span>  |   <span data-ttu-id="a1420-126">A data em que a entidade é criada.</span><span class="sxs-lookup"><span data-stu-id="a1420-126">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="a1420-127">id</span><span class="sxs-lookup"><span data-stu-id="a1420-127">id</span></span>  |   <span data-ttu-id="a1420-128">String</span><span class="sxs-lookup"><span data-stu-id="a1420-128">String</span></span>  |   <span data-ttu-id="a1420-129">Combinação de azureTenantId_createdDateTime.</span><span class="sxs-lookup"><span data-stu-id="a1420-129">Combination of azureTenantId_createdDateTime.</span></span>   |
|   <span data-ttu-id="a1420-130">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="a1420-130">licensedUserCount</span></span>   |   <span data-ttu-id="a1420-131">Int32</span><span class="sxs-lookup"><span data-stu-id="a1420-131">Int32</span></span>   |   <span data-ttu-id="a1420-132">Contagem de usuários licenciados de um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="a1420-132">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="a1420-133">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="a1420-133">activeUserCount</span></span> |   <span data-ttu-id="a1420-134">Int32</span><span class="sxs-lookup"><span data-stu-id="a1420-134">Int32</span></span>   |   <span data-ttu-id="a1420-135">Contagem de usuários ativos de um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="a1420-135">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="a1420-136">currentScore</span><span class="sxs-lookup"><span data-stu-id="a1420-136">currentScore</span></span>    |   <span data-ttu-id="a1420-137">Duplo</span><span class="sxs-lookup"><span data-stu-id="a1420-137">Double</span></span>  |   <span data-ttu-id="a1420-138">Pontuação Obtida de locatário atual em data especificada.</span><span class="sxs-lookup"><span data-stu-id="a1420-138">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="a1420-139">maxScore</span><span class="sxs-lookup"><span data-stu-id="a1420-139">maxScore</span></span> |  <span data-ttu-id="a1420-140">Duplo</span><span class="sxs-lookup"><span data-stu-id="a1420-140">Double</span></span>  |   <span data-ttu-id="a1420-141">Pontuação máxima possível de locatário na data especificada.</span><span class="sxs-lookup"><span data-stu-id="a1420-141">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="a1420-142">enabledservices</span><span class="sxs-lookup"><span data-stu-id="a1420-142">enabledServices</span></span> |   <span data-ttu-id="a1420-143">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1420-143">String collection</span></span>   |   <span data-ttu-id="a1420-144">Serviços fornecidos pela Microsoft para o locatário (por exemplo, Exchange Online, Skype, SharePoint).</span><span class="sxs-lookup"><span data-stu-id="a1420-144">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="a1420-145">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="a1420-145">averageComparativeScores</span></span> |  <span data-ttu-id="a1420-146">coleção [averageComparativeScore](averagecomparativescore.md)</span><span class="sxs-lookup"><span data-stu-id="a1420-146">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="a1420-147">Pontuação média por escopos diferentes (por exemplo, média por setor, média por meio de assentos) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura) dentro do escopo.</span><span class="sxs-lookup"><span data-stu-id="a1420-147">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="a1420-148">controlScores</span><span class="sxs-lookup"><span data-stu-id="a1420-148">controlScores</span></span> | <span data-ttu-id="a1420-149">coleção [controlScore](controlscore.md)</span><span class="sxs-lookup"><span data-stu-id="a1420-149">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="a1420-150">Contém pontuações de locatários para um conjunto de controles.</span><span class="sxs-lookup"><span data-stu-id="a1420-150">Contains tenant scores for a set of controls.</span></span>   |


## <a name="relationships"></a><span data-ttu-id="a1420-151">Relações</span><span class="sxs-lookup"><span data-stu-id="a1420-151">Relationships</span></span>

<span data-ttu-id="a1420-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a1420-152">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1420-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a1420-153">JSON representation</span></span>

<span data-ttu-id="a1420-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a1420-154">The following is a JSON representation of the resource.</span></span>

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
