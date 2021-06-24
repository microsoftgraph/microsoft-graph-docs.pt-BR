---
title: Tipo de recurso serviceHealthIssue
description: Representa um problema de saúde do serviço em um serviço.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 2436e6d0d5e49155b936cbfb7f7fc98630b7ce57
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109065"
---
# <a name="servicehealthissue-resource-type"></a><span data-ttu-id="b3f06-103">Tipo de recurso serviceHealthIssue</span><span class="sxs-lookup"><span data-stu-id="b3f06-103">serviceHealthIssue resource type</span></span>

<span data-ttu-id="b3f06-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3f06-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3f06-105">Representa um problema de saúde do serviço em um serviço.</span><span class="sxs-lookup"><span data-stu-id="b3f06-105">Represents a service health issue in a service.</span></span>

<span data-ttu-id="b3f06-106">O problema de saúde do serviço pode ser um incidente de serviço ou uma consultoria de serviço.</span><span class="sxs-lookup"><span data-stu-id="b3f06-106">The service health issue can be a service incident or service advisory.</span></span> <span data-ttu-id="b3f06-107">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="b3f06-107">For example:</span></span>

* <span data-ttu-id="b3f06-108">Incidente de serviço: "Exchange de caixa de correio está inobada".</span><span class="sxs-lookup"><span data-stu-id="b3f06-108">Service incident: "Exchange mailbox service is down".</span></span>
* <span data-ttu-id="b3f06-109">Aviso de serviço: "Os usuários podem ter atrasos na recepção de emails".</span><span class="sxs-lookup"><span data-stu-id="b3f06-109">Service advisory: "Users may experience delays in emails reception".</span></span>

<span data-ttu-id="b3f06-110">Herda [de serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="b3f06-110">Inherits from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b3f06-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="b3f06-111">Methods</span></span>
|<span data-ttu-id="b3f06-112">Método</span><span class="sxs-lookup"><span data-stu-id="b3f06-112">Method</span></span>|<span data-ttu-id="b3f06-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b3f06-113">Return type</span></span>|<span data-ttu-id="b3f06-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3f06-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b3f06-115">Obter serviceHealthIssue</span><span class="sxs-lookup"><span data-stu-id="b3f06-115">Get serviceHealthIssue</span></span>](../api/servicehealthissue-get.md)|[<span data-ttu-id="b3f06-116">serviceHealthIssue</span><span class="sxs-lookup"><span data-stu-id="b3f06-116">serviceHealthIssue</span></span>](../resources/servicehealthissue.md)|<span data-ttu-id="b3f06-117">Recupere as propriedades e as relações de um [objeto serviceHealthIssue.](../resources/servicehealthissue.md)</span><span class="sxs-lookup"><span data-stu-id="b3f06-117">Retrieve the properties and relationships of a [serviceHealthIssue](../resources/servicehealthissue.md) object.</span></span> |
|[<span data-ttu-id="b3f06-118">Obter relatório de revisão pós-incidente</span><span class="sxs-lookup"><span data-stu-id="b3f06-118">Get post-incident review report</span></span>](../api/servicehealthissue-incidentreport.md)|<span data-ttu-id="b3f06-119">Stream</span><span class="sxs-lookup"><span data-stu-id="b3f06-119">Stream</span></span>|<span data-ttu-id="b3f06-120">Fornece o documento de relatório de incidente pós-incidente (PIR) de um problema de serviço especificado para locatário.</span><span class="sxs-lookup"><span data-stu-id="b3f06-120">Provides the post incident report (PIR) document of a specified service issue for tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="b3f06-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b3f06-121">Properties</span></span>
|<span data-ttu-id="b3f06-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3f06-122">Property</span></span>|<span data-ttu-id="b3f06-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3f06-123">Type</span></span>|<span data-ttu-id="b3f06-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3f06-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3f06-125">classificação</span><span class="sxs-lookup"><span data-stu-id="b3f06-125">classification</span></span>|<span data-ttu-id="b3f06-126">serviceHealthClassificationType</span><span class="sxs-lookup"><span data-stu-id="b3f06-126">serviceHealthClassificationType</span></span>|<span data-ttu-id="b3f06-127">O tipo de problema de saúde do serviço.</span><span class="sxs-lookup"><span data-stu-id="b3f06-127">The type of service health issue.</span></span> <span data-ttu-id="b3f06-128">Os valores possíveis são: `advisory`, `incident`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b3f06-128">Possible values are: `advisory`, `incident`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="b3f06-129">detalhes</span><span class="sxs-lookup"><span data-stu-id="b3f06-129">details</span></span>|<span data-ttu-id="b3f06-130">Coleção([keyValuePair](../resources/keyvaluepair.md))</span><span class="sxs-lookup"><span data-stu-id="b3f06-130">Collection([keyValuePair](../resources/keyvaluepair.md))</span></span>|<span data-ttu-id="b3f06-131">Detalhes adicionais sobre o problema de saúde do serviço.</span><span class="sxs-lookup"><span data-stu-id="b3f06-131">Additional details about service health issue.</span></span> <span data-ttu-id="b3f06-132">Essa propriedade não dá suporte a filtros.</span><span class="sxs-lookup"><span data-stu-id="b3f06-132">This property doesn't support filters.</span></span> <span data-ttu-id="b3f06-133">Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="b3f06-133">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="b3f06-134">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b3f06-134">endDateTime</span></span>|<span data-ttu-id="b3f06-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3f06-135">DateTimeOffset</span></span>|<span data-ttu-id="b3f06-136">A hora de término do problema do serviço.</span><span class="sxs-lookup"><span data-stu-id="b3f06-136">The end time of the service issue.</span></span> <span data-ttu-id="b3f06-137">Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="b3f06-137">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="b3f06-138">feature</span><span class="sxs-lookup"><span data-stu-id="b3f06-138">feature</span></span>|<span data-ttu-id="b3f06-139">String</span><span class="sxs-lookup"><span data-stu-id="b3f06-139">String</span></span>|<span data-ttu-id="b3f06-140">O nome do recurso do problema do serviço.</span><span class="sxs-lookup"><span data-stu-id="b3f06-140">The feature name of the service issue.</span></span>|
|<span data-ttu-id="b3f06-141">featureGroup</span><span class="sxs-lookup"><span data-stu-id="b3f06-141">featureGroup</span></span>|<span data-ttu-id="b3f06-142">String</span><span class="sxs-lookup"><span data-stu-id="b3f06-142">String</span></span>|<span data-ttu-id="b3f06-143">O nome do grupo de recursos do problema do serviço.</span><span class="sxs-lookup"><span data-stu-id="b3f06-143">The feature group name of the service issue.</span></span>|
|<span data-ttu-id="b3f06-144">id</span><span class="sxs-lookup"><span data-stu-id="b3f06-144">id</span></span>|<span data-ttu-id="b3f06-145">String</span><span class="sxs-lookup"><span data-stu-id="b3f06-145">String</span></span>|<span data-ttu-id="b3f06-146">A id do problema do serviço.</span><span class="sxs-lookup"><span data-stu-id="b3f06-146">The id of the service issue.</span></span> <span data-ttu-id="b3f06-147">Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="b3f06-147">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="b3f06-148">impactDescription</span><span class="sxs-lookup"><span data-stu-id="b3f06-148">impactDescription</span></span>|<span data-ttu-id="b3f06-149">String</span><span class="sxs-lookup"><span data-stu-id="b3f06-149">String</span></span>|<span data-ttu-id="b3f06-150">A descrição do impacto do problema do serviço.</span><span class="sxs-lookup"><span data-stu-id="b3f06-150">The description of the service issue impact.</span></span>|
|<span data-ttu-id="b3f06-151">isResolved</span><span class="sxs-lookup"><span data-stu-id="b3f06-151">isResolved</span></span>|<span data-ttu-id="b3f06-152">Booleano</span><span class="sxs-lookup"><span data-stu-id="b3f06-152">Boolean</span></span>|<span data-ttu-id="b3f06-153">Indica se o problema foi resolvido.</span><span class="sxs-lookup"><span data-stu-id="b3f06-153">Indicates whether the issue is resolved.</span></span>|
|<span data-ttu-id="b3f06-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3f06-154">lastModifiedDateTime</span></span>|<span data-ttu-id="b3f06-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3f06-155">DateTimeOffset</span></span>|<span data-ttu-id="b3f06-156">A última hora modificada do problema.</span><span class="sxs-lookup"><span data-stu-id="b3f06-156">The last modified time of the issue.</span></span> <span data-ttu-id="b3f06-157">Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="b3f06-157">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="b3f06-158">origin</span><span class="sxs-lookup"><span data-stu-id="b3f06-158">origin</span></span>|<span data-ttu-id="b3f06-159">serviceHealthOrigin</span><span class="sxs-lookup"><span data-stu-id="b3f06-159">serviceHealthOrigin</span></span>|<span data-ttu-id="b3f06-160">Indica a origem do problema do serviço.</span><span class="sxs-lookup"><span data-stu-id="b3f06-160">Indicates the origin of the service issue.</span></span> <span data-ttu-id="b3f06-161">Os valores possíveis são: `microsoft`, `thirdParty`, `customer`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b3f06-161">Possible values are: `microsoft`, `thirdParty`, `customer`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="b3f06-162">postagens</span><span class="sxs-lookup"><span data-stu-id="b3f06-162">posts</span></span>|<span data-ttu-id="b3f06-163">Collection([serviceHealthIssuePost](../resources/servicehealthissuepost.md))</span><span class="sxs-lookup"><span data-stu-id="b3f06-163">Collection([serviceHealthIssuePost](../resources/servicehealthissuepost.md))</span></span>|<span data-ttu-id="b3f06-164">Coleção de postagens históricas para o problema do serviço.</span><span class="sxs-lookup"><span data-stu-id="b3f06-164">Collection of historical posts for the service issue.</span></span>|
|<span data-ttu-id="b3f06-165">service</span><span class="sxs-lookup"><span data-stu-id="b3f06-165">service</span></span>|<span data-ttu-id="b3f06-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3f06-166">String</span></span>|<span data-ttu-id="b3f06-167">Indica o serviço afetado pelo problema.</span><span class="sxs-lookup"><span data-stu-id="b3f06-167">Indicates the service affected by the issue.</span></span>|
|<span data-ttu-id="b3f06-168">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b3f06-168">startDateTime</span></span>|<span data-ttu-id="b3f06-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3f06-169">DateTimeOffset</span></span>|<span data-ttu-id="b3f06-170">A hora de início do problema do serviço.</span><span class="sxs-lookup"><span data-stu-id="b3f06-170">The start time of the service issue.</span></span> <span data-ttu-id="b3f06-171">Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="b3f06-171">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="b3f06-172">status</span><span class="sxs-lookup"><span data-stu-id="b3f06-172">status</span></span>|<span data-ttu-id="b3f06-173">serviceHealthStatus</span><span class="sxs-lookup"><span data-stu-id="b3f06-173">serviceHealthStatus</span></span>|<span data-ttu-id="b3f06-174">O status do problema do serviço.</span><span class="sxs-lookup"><span data-stu-id="b3f06-174">The status of the service issue.</span></span> <span data-ttu-id="b3f06-175">Os valores possíveis são: `serviceOperational` , , , , , , , , `investigating` , , , `restoringService` , , `verifyingService` , , , `serviceRestored` , , `postIncidentReviewPublished` `serviceDegradation` , `serviceInterruption` `extendedRecovery` `falsePositive` `investigationSuspended` `resolved` `mitigatedExternal` `mitigated` `resolvedExternal` `confirmed` . `reported` `unknownFutureValue`</span><span class="sxs-lookup"><span data-stu-id="b3f06-175">Possible values are: `serviceOperational`, `investigating`, `restoringService`, `verifyingService`, `serviceRestored`, `postIncidentReviewPublished`, `serviceDegradation`, `serviceInterruption`, `extendedRecovery`, `falsePositive`, `investigationSuspended`, `resolved`, `mitigatedExternal`, `mitigated`, `resolvedExternal`, `confirmed`, `reported`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="b3f06-176">title</span><span class="sxs-lookup"><span data-stu-id="b3f06-176">title</span></span>|<span data-ttu-id="b3f06-177">String</span><span class="sxs-lookup"><span data-stu-id="b3f06-177">String</span></span>|<span data-ttu-id="b3f06-178">O título do problema do serviço.</span><span class="sxs-lookup"><span data-stu-id="b3f06-178">The title of the service issue.</span></span> <span data-ttu-id="b3f06-179">Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="b3f06-179">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3f06-180">Relações</span><span class="sxs-lookup"><span data-stu-id="b3f06-180">Relationships</span></span>
<span data-ttu-id="b3f06-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b3f06-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3f06-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b3f06-182">JSON representation</span></span>
<span data-ttu-id="b3f06-183">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b3f06-183">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceHealthIssue",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceHealthIssue",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "title": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "id": "String (identifier)",
  "impactDescription": "String",
  "classification": "String",
  "origin": "String",
  "posts": [
    {
      "@odata.type": "microsoft.graph.serviceHealthIssuePost"
    }
  ],
  "status": "String",
  "service": "String",
  "feature": "String",
  "featureGroup": "String",
  "isResolved": "Boolean"
}
```

