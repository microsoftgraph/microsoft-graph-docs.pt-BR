---
title: tipo de recurso de secureScores
description: 'superior = n, onde n = o número de dias de dados que você deseja recuperar. '
localization_priority: Normal
ms.openlocfilehash: 332a9656d8237bb07d5c7739b666e09539cf984f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828732"
---
# <a name="securescores-resource-type"></a><span data-ttu-id="6c785-103">tipo de recurso de secureScores</span><span class="sxs-lookup"><span data-stu-id="6c785-103">secureScores resource type</span></span>

> <span data-ttu-id="6c785-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6c785-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c785-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6c785-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6c785-106">Representa a pontuação seguro de um locatário por dia da pontuação de dados, no nível de locatário e controle.</span><span class="sxs-lookup"><span data-stu-id="6c785-106">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="6c785-107">Por padrão, 90 dias de dados é mantido.</span><span class="sxs-lookup"><span data-stu-id="6c785-107">By default, 90 days of data is held.</span></span> <span data-ttu-id="6c785-108">Esses dados são classificados pelo **createdDateTime**, do mais recente à mais antiga.</span><span class="sxs-lookup"><span data-stu-id="6c785-108">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="6c785-109">Isso permitirá que você para respostas da página usando $top = n, onde n = o número de dias de dados que você deseja recuperar.</span><span class="sxs-lookup"><span data-stu-id="6c785-109">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="6c785-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="6c785-110">Methods</span></span>

| <span data-ttu-id="6c785-111">Método</span><span class="sxs-lookup"><span data-stu-id="6c785-111">Method</span></span>   | <span data-ttu-id="6c785-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6c785-112">Return Type</span></span>|<span data-ttu-id="6c785-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c785-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6c785-114">Lista secureScores</span><span class="sxs-lookup"><span data-stu-id="6c785-114">List secureScores</span></span>](../api/securescores-list.md) | [<span data-ttu-id="6c785-115">secureScores</span><span class="sxs-lookup"><span data-stu-id="6c785-115">secureScores</span></span>](securescores.md) |<span data-ttu-id="6c785-116">Leia as propriedades e os metadados de um objeto secureScores.</span><span class="sxs-lookup"><span data-stu-id="6c785-116">Read properties and metadata of a secureScores object.</span></span>|


## <a name="properties"></a><span data-ttu-id="6c785-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6c785-117">Properties</span></span>
<span data-ttu-id="6c785-118">Propriedades que contêm de tipo de entidade de segurança locatário pontuação (dados diários de instantâneo).</span><span class="sxs-lookup"><span data-stu-id="6c785-118">Entity type containing properties of the tenant security score (daily snapshot data).</span></span>

|<span data-ttu-id="6c785-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c785-119">Property</span></span> |<span data-ttu-id="6c785-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c785-120">Type</span></span> |<span data-ttu-id="6c785-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c785-121">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="6c785-122">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="6c785-122">azureTenantId</span></span>   |   <span data-ttu-id="6c785-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c785-123">String</span></span>  |   <span data-ttu-id="6c785-124">ID de cadeia de caracteres do GUID para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="6c785-124">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="6c785-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c785-125">createdDateTime</span></span> |   <span data-ttu-id="6c785-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c785-126">DateTimeOffset</span></span>  |   <span data-ttu-id="6c785-127">A data em que a entidade é criada.</span><span class="sxs-lookup"><span data-stu-id="6c785-127">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="6c785-128">id</span><span class="sxs-lookup"><span data-stu-id="6c785-128">id</span></span>  |   <span data-ttu-id="6c785-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c785-129">String</span></span>  |   <span data-ttu-id="6c785-130">Combinação de azureTenantId_createdDateTime.</span><span class="sxs-lookup"><span data-stu-id="6c785-130">Combination of azureTenantId_createdDateTime.</span></span>   |
|   <span data-ttu-id="6c785-131">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="6c785-131">licensedUserCount</span></span>   |   <span data-ttu-id="6c785-132">Int32</span><span class="sxs-lookup"><span data-stu-id="6c785-132">Int32</span></span>   |   <span data-ttu-id="6c785-133">Licenciado contagem de usuários do determinado inquilino.</span><span class="sxs-lookup"><span data-stu-id="6c785-133">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="6c785-134">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="6c785-134">activeUserCount</span></span> |   <span data-ttu-id="6c785-135">Int32</span><span class="sxs-lookup"><span data-stu-id="6c785-135">Int32</span></span>   |   <span data-ttu-id="6c785-136">Contagem de usuário ativo do determinado inquilino.</span><span class="sxs-lookup"><span data-stu-id="6c785-136">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="6c785-137">currentScore</span><span class="sxs-lookup"><span data-stu-id="6c785-137">currentScore</span></span>    |   <span data-ttu-id="6c785-138">Duplo</span><span class="sxs-lookup"><span data-stu-id="6c785-138">Double</span></span>  |   <span data-ttu-id="6c785-139">Pontuação de locatário atual que já alcançou na data especificada.</span><span class="sxs-lookup"><span data-stu-id="6c785-139">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="6c785-140">maxScore</span><span class="sxs-lookup"><span data-stu-id="6c785-140">maxScore</span></span> |  <span data-ttu-id="6c785-141">Duplo</span><span class="sxs-lookup"><span data-stu-id="6c785-141">Double</span></span>  |   <span data-ttu-id="6c785-142">Locatário pontuação possíveis máxima na data especificada.</span><span class="sxs-lookup"><span data-stu-id="6c785-142">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="6c785-143">enabledServices</span><span class="sxs-lookup"><span data-stu-id="6c785-143">enabledServices</span></span> |   <span data-ttu-id="6c785-144">String collection</span><span class="sxs-lookup"><span data-stu-id="6c785-144">String collection</span></span>   |   <span data-ttu-id="6c785-145">Serviços fornecida pela Microsoft para o locatário (por exemplo, Exchange online, Skype, Sharepoint).</span><span class="sxs-lookup"><span data-stu-id="6c785-145">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="6c785-146">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="6c785-146">averageComparativeScores</span></span> |  <span data-ttu-id="6c785-147">coleção [averageComparativeScore](averagecomparativescore.md)</span><span class="sxs-lookup"><span data-stu-id="6c785-147">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="6c785-148">Pontuação média por escopos diferentes (por exemplo, média por setor, média por assentos) e a categoria de controle (identidade, dados, dispositivo, aplicativos, infra-estrutura) dentro do escopo.</span><span class="sxs-lookup"><span data-stu-id="6c785-148">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="6c785-149">controlScores</span><span class="sxs-lookup"><span data-stu-id="6c785-149">controlScores</span></span> | <span data-ttu-id="6c785-150">coleção [controlScore](controlscore.md)</span><span class="sxs-lookup"><span data-stu-id="6c785-150">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="6c785-151">Contém as pontuações de locatário de um conjunto de controles.</span><span class="sxs-lookup"><span data-stu-id="6c785-151">Contains tenant scores for a set of controls.</span></span>   |


## <a name="relationships"></a><span data-ttu-id="6c785-152">Relações</span><span class="sxs-lookup"><span data-stu-id="6c785-152">Relationships</span></span>

<span data-ttu-id="6c785-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6c785-153">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c785-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6c785-154">JSON representation</span></span>

<span data-ttu-id="6c785-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6c785-155">The following is a JSON representation of the resource.</span></span>

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


<!-- {
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
