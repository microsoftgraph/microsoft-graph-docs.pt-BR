---
title: Tipos de recursos accessReviewHistoryDefinition
description: Representa uma coleção de dados de histórico de revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 96619cb95c11a77106c86cbdcc720f1a486721c7
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232898"
---
# <a name="accessreviewhistorydefinition-resource-type"></a><span data-ttu-id="71191-103">Tipo de recurso accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="71191-103">accessReviewHistoryDefinition resource type</span></span>

<span data-ttu-id="71191-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71191-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71191-105">Representa uma coleção de dados de histórico de revisão de acesso e os escopos usados para coletar esses dados.</span><span class="sxs-lookup"><span data-stu-id="71191-105">Represents a collection of access review history data and the scopes used to collect that data.</span></span> <span data-ttu-id="71191-106">As **propriedades reviewHistoryPeriodStartDateTime**, **reviewHistoryPeriodEndDateTime**, **decisions** e scopes de **um accessReviewHistoryDefinition** são usadas ao selecionar dados de histórico de revisão e podem ser **modificadas.**</span><span class="sxs-lookup"><span data-stu-id="71191-106">The **reviewHistoryPeriodStartDateTime**, **reviewHistoryPeriodEndDateTime**, **decisions**, and **scopes** properties of an **accessReviewHistoryDefinition** are used when selecting review history data, and can be modified.</span></span> <span data-ttu-id="71191-107">Cada **objeto accessReviewHistoryDefinition** está disponível apenas por 30 dias.</span><span class="sxs-lookup"><span data-stu-id="71191-107">Each **accessReviewHistoryDefinition** object is only available for 30 days.</span></span> <span data-ttu-id="71191-108">Depois que o status de uma definição de histórico é movido para um link pode ser gerado para recuperar os dados da definição chamando `done` [generateDownloadUri](../api/accessreviewhistorydefinition-generatedownloaduri.md).</span><span class="sxs-lookup"><span data-stu-id="71191-108">Once a history definition's status has moved to `done` a link can be generated to retrieve the definition's data by calling [generateDownloadUri](../api/accessreviewhistorydefinition-generatedownloaduri.md).</span></span>

## <a name="methods"></a><span data-ttu-id="71191-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="71191-109">Methods</span></span>
|<span data-ttu-id="71191-110">Método</span><span class="sxs-lookup"><span data-stu-id="71191-110">Method</span></span>|<span data-ttu-id="71191-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="71191-111">Return type</span></span>|<span data-ttu-id="71191-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="71191-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="71191-113">Listar accessReviewHistoryDefinitions</span><span class="sxs-lookup"><span data-stu-id="71191-113">List accessReviewHistoryDefinitions</span></span>](../api/accessreviewhistorydefinition-list.md)|<span data-ttu-id="71191-114">[Coleção accessReviewHistoryDefinition](accessreviewhistorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="71191-114">[accessReviewHistoryDefinition](accessreviewhistorydefinition.md) collection</span></span>|<span data-ttu-id="71191-115">Obter uma lista dos [objetos accessReviewHistoryDefinition](accessreviewhistorydefinition.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="71191-115">Get a list of the [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) objects and their properties.</span></span>|
|[<span data-ttu-id="71191-116">Criar accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="71191-116">Create accessReviewHistoryDefinition</span></span>](../api/accessreviewhistorydefinition-post.md)|[<span data-ttu-id="71191-117">accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="71191-117">accessReviewHistoryDefinition</span></span>](accessreviewhistorydefinition.md)|<span data-ttu-id="71191-118">Crie um novo [objeto accessReviewHistoryDefinition.](accessreviewhistorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="71191-118">Create a new [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) object.</span></span>|
|[<span data-ttu-id="71191-119">Obter accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="71191-119">Get accessReviewHistoryDefinition</span></span>](../api/accessreviewhistorydefinition-get.md)|[<span data-ttu-id="71191-120">accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="71191-120">accessReviewHistoryDefinition</span></span>](accessreviewhistorydefinition.md)|<span data-ttu-id="71191-121">Leia as propriedades e as relações de [um objeto accessReviewHistoryDefinition.](accessreviewhistorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="71191-121">Read the properties and relationships of an [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) object.</span></span>|
|[<span data-ttu-id="71191-122">generateDownloadUri</span><span class="sxs-lookup"><span data-stu-id="71191-122">generateDownloadUri</span></span>](../api/accessreviewhistorydefinition-generatedownloaduri.md)|[<span data-ttu-id="71191-123">accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="71191-123">accessReviewHistoryDefinition</span></span>](accessreviewhistorydefinition.md)|<span data-ttu-id="71191-124">Gere um URI que pode ser usado para recuperar dados de histórico de revisão.</span><span class="sxs-lookup"><span data-stu-id="71191-124">Generate a URI that can be used to retrieve review history data.</span></span>|

## <a name="properties"></a><span data-ttu-id="71191-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71191-125">Properties</span></span>
|<span data-ttu-id="71191-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71191-126">Property</span></span>|<span data-ttu-id="71191-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="71191-127">Type</span></span>|<span data-ttu-id="71191-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="71191-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71191-129">createdBy</span><span class="sxs-lookup"><span data-stu-id="71191-129">createdBy</span></span>|[<span data-ttu-id="71191-130">userIdentity</span><span class="sxs-lookup"><span data-stu-id="71191-130">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="71191-131">Usuário que criou essa definição de histórico de revisão.</span><span class="sxs-lookup"><span data-stu-id="71191-131">User who created this review history definition.</span></span> |
|<span data-ttu-id="71191-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71191-132">createdDateTime</span></span>|<span data-ttu-id="71191-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71191-133">DateTimeOffset</span></span>|<span data-ttu-id="71191-134">Timestamp quando a definição de revisão de acesso foi criada.</span><span class="sxs-lookup"><span data-stu-id="71191-134">Timestamp when the access review definition was created.</span></span>|
|<span data-ttu-id="71191-135">decisions</span><span class="sxs-lookup"><span data-stu-id="71191-135">decisions</span></span>|<span data-ttu-id="71191-136">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="71191-136">String collection</span></span>|<span data-ttu-id="71191-137">Determina quais decisões de revisão serão incluídas nos dados de histórico de revisão buscados, se especificado.</span><span class="sxs-lookup"><span data-stu-id="71191-137">Determines which review decisions will be included in the fetched review history data if specified.</span></span> <span data-ttu-id="71191-138">Opcional ao criar.</span><span class="sxs-lookup"><span data-stu-id="71191-138">Optional on create.</span></span> <span data-ttu-id="71191-139">Todas as decisões serão incluídas por padrão se nenhuma decisão for fornecida na criação.</span><span class="sxs-lookup"><span data-stu-id="71191-139">All decisions will be included by default if no decisions are provided on create.</span></span> <span data-ttu-id="71191-140">Os valores possíveis são: `approve` , , , e `deny` `dontKnow` `notReviewed` `notNotified` .</span><span class="sxs-lookup"><span data-stu-id="71191-140">Possible values are: `approve`, `deny`, `dontKnow`, `notReviewed`, and `notNotified`.</span></span>|
|<span data-ttu-id="71191-141">displayName</span><span class="sxs-lookup"><span data-stu-id="71191-141">displayName</span></span>|<span data-ttu-id="71191-142">String</span><span class="sxs-lookup"><span data-stu-id="71191-142">String</span></span>|<span data-ttu-id="71191-143">Nome da coleção de dados do histórico de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="71191-143">Name for the access review history data collection.</span></span> <span data-ttu-id="71191-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71191-144">Required.</span></span>|
|<span data-ttu-id="71191-145">downloadUri</span><span class="sxs-lookup"><span data-stu-id="71191-145">downloadUri</span></span>|<span data-ttu-id="71191-146">String</span><span class="sxs-lookup"><span data-stu-id="71191-146">String</span></span>|<span data-ttu-id="71191-147">Uri que pode ser usado para recuperar dados de histórico de revisão.</span><span class="sxs-lookup"><span data-stu-id="71191-147">Uri which can be used to retrieve review history data.</span></span> <span data-ttu-id="71191-148">Esse URI ficará ativo por 24 horas após ser gerado.</span><span class="sxs-lookup"><span data-stu-id="71191-148">This URI will be active for 24 hours after being generated.</span></span>|
|<span data-ttu-id="71191-149">fulfilledDateTime</span><span class="sxs-lookup"><span data-stu-id="71191-149">fulfilledDateTime</span></span>|<span data-ttu-id="71191-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71191-150">DateTimeOffset</span></span>|<span data-ttu-id="71191-151">Timestamp quando todos os dados disponíveis para essa definição foram coletados.</span><span class="sxs-lookup"><span data-stu-id="71191-151">Timestamp when all of the available data for this definition was collected.</span></span> <span data-ttu-id="71191-152">Isso será definido depois que o status dessa definição for definido como `done` .</span><span class="sxs-lookup"><span data-stu-id="71191-152">This will be set after this definition's status is set to `done`.</span></span>|
|<span data-ttu-id="71191-153">id</span><span class="sxs-lookup"><span data-stu-id="71191-153">id</span></span>|<span data-ttu-id="71191-154">String</span><span class="sxs-lookup"><span data-stu-id="71191-154">String</span></span>|<span data-ttu-id="71191-155">O identificador exclusivo atribuído de uma definição de histórico de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="71191-155">The assigned unique identifier of an access review history definition.</span></span>|
|<span data-ttu-id="71191-156">reviewHistoryPeriodEndDateTime</span><span class="sxs-lookup"><span data-stu-id="71191-156">reviewHistoryPeriodEndDateTime</span></span>|<span data-ttu-id="71191-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71191-157">DateTimeOffset</span></span>|<span data-ttu-id="71191-158">Timestamp, as avaliações que começam em ou após essa data serão incluídas nos dados de histórico buscados.</span><span class="sxs-lookup"><span data-stu-id="71191-158">Timestamp, reviews starting on or after this date will be included in the fetched history data.</span></span> <span data-ttu-id="71191-159">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71191-159">Required.</span></span>|
|<span data-ttu-id="71191-160">reviewHistoryPeriodStartDateTime</span><span class="sxs-lookup"><span data-stu-id="71191-160">reviewHistoryPeriodStartDateTime</span></span>|<span data-ttu-id="71191-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71191-161">DateTimeOffset</span></span>|<span data-ttu-id="71191-162">Timestamp, as avaliações que começam em ou antes dessa data serão incluídas nos dados de histórico buscados.</span><span class="sxs-lookup"><span data-stu-id="71191-162">Timestamp, reviews starting on or before this date will be included in the fetched history data.</span></span> <span data-ttu-id="71191-163">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71191-163">Required.</span></span>|
|<span data-ttu-id="71191-164">escopos</span><span class="sxs-lookup"><span data-stu-id="71191-164">scopes</span></span>|<span data-ttu-id="71191-165">coleção microsoft.graph.accessReviewQueryScope</span><span class="sxs-lookup"><span data-stu-id="71191-165">microsoft.graph.accessReviewQueryScope collection</span></span>|<span data-ttu-id="71191-166">Usado para analisar quais avaliações são incluídas nos dados de histórico buscados.</span><span class="sxs-lookup"><span data-stu-id="71191-166">Used to scope what reviews are included in the fetched history data.</span></span> <span data-ttu-id="71191-167">Busca avaliações cujo escopo corresponde a esse escopo fornecido.</span><span class="sxs-lookup"><span data-stu-id="71191-167">Fetches reviews whose scope matches with this provided scope.</span></span> <span data-ttu-id="71191-168">Consulte [accessreviewqueryscope](accessreviewqueryscope.md).</span><span class="sxs-lookup"><span data-stu-id="71191-168">See [accessreviewqueryscope](accessreviewqueryscope.md).</span></span> <span data-ttu-id="71191-169">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71191-169">Required.</span></span>|
|<span data-ttu-id="71191-170">status</span><span class="sxs-lookup"><span data-stu-id="71191-170">status</span></span>|<span data-ttu-id="71191-171">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="71191-171">String collection</span></span>|<span data-ttu-id="71191-172">Representa o status da coleção de dados do histórico de revisão.</span><span class="sxs-lookup"><span data-stu-id="71191-172">Represents the status of the review history data collection.</span></span> <span data-ttu-id="71191-173">Os valores possíveis são: `done`, `inprogress`, `error`, `requested`.</span><span class="sxs-lookup"><span data-stu-id="71191-173">Possible values are: `done`, `inprogress`, `error`, `requested`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71191-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71191-174">JSON representation</span></span>
<span data-ttu-id="71191-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71191-175">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewHistoryDefinition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewHistoryDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "reviewHistoryPeriodStartDateTime": "String (timestamp)",
  "reviewHistoryPeriodEndDateTime": "String (timestamp)",
  "decisions": [
    {
      "@odata.type": "String"
    }
  ],
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "fulfilledDateTime": "String (timestamp)",
  "downloadUri": "String",
  "createdBy": {
    "@odata.type": "#microsoft.graph.userIdentity"
  },
  "scopes": [
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    }
  ]
}
```
