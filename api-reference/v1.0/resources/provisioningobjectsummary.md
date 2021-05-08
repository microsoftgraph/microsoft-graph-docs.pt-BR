---
title: Tipo de recurso provisioningObjectSummary
description: Representa uma ação executada pelo serviço de Provisionamento do Azure AD e suas propriedades associadas.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: d9852745ed14cacd47389da5031cb83af306e2d0
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241480"
---
# <a name="provisioningobjectsummary-resource-type"></a><span data-ttu-id="d50b6-103">Tipo de recurso provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="d50b6-103">provisioningObjectSummary resource type</span></span>

<span data-ttu-id="d50b6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d50b6-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="d50b6-105">Representa uma ação executada pelo serviço de Provisionamento do Azure AD e suas propriedades associadas.</span><span class="sxs-lookup"><span data-stu-id="d50b6-105">Represents an action performed by the Azure AD Provisioning service and its associated properties.</span></span> 

## <a name="methods"></a><span data-ttu-id="d50b6-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="d50b6-106">Methods</span></span>

| <span data-ttu-id="d50b6-107">Método</span><span class="sxs-lookup"><span data-stu-id="d50b6-107">Method</span></span>  | <span data-ttu-id="d50b6-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d50b6-108">Return Type</span></span> | <span data-ttu-id="d50b6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d50b6-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d50b6-110">Listar provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="d50b6-110">List provisioningObjectSummary</span></span>](../api/provisioningobjectsummary-list.md) | [<span data-ttu-id="d50b6-111">provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="d50b6-111">provisioningObjectSummary</span></span>](provisioningobjectsummary.md) | <span data-ttu-id="d50b6-112">Obter uma lista de todos os eventos de provisionamento que ocorreram em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="d50b6-112">Get a list of all provisioning events that occurred in your tenant.</span></span> |


## <a name="properties"></a><span data-ttu-id="d50b6-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d50b6-113">Properties</span></span>

| <span data-ttu-id="d50b6-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d50b6-114">Property</span></span>     | <span data-ttu-id="d50b6-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="d50b6-115">Type</span></span>        | <span data-ttu-id="d50b6-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="d50b6-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d50b6-117">provisioningAction</span><span class="sxs-lookup"><span data-stu-id="d50b6-117">provisioningAction</span></span>|<span data-ttu-id="d50b6-118">provisioningAction</span><span class="sxs-lookup"><span data-stu-id="d50b6-118">provisioningAction</span></span>|<span data-ttu-id="d50b6-119">Indica o nome da atividade ou o nome da operação.</span><span class="sxs-lookup"><span data-stu-id="d50b6-119">Indicates the activity name or the operation name.</span></span> <span data-ttu-id="d50b6-120">Os valores possíveis são: `create` , , , , e `update` `delete` `stageddelete` `disable` `other` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="d50b6-120">Possible values are: `create`, `update`, `delete`, `stageddelete`, `disable`, `other` and `unknownFutureValue`.</span></span> <span data-ttu-id="d50b6-121">Para uma lista de atividades registradas, consulte a lista de atividades do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d50b6-121">For a list of activities logged, refer to Azure AD activity list.</span></span>|
|<span data-ttu-id="d50b6-122">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="d50b6-122">activityDateTime</span></span>|<span data-ttu-id="d50b6-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d50b6-123">DateTimeOffset</span></span>|<span data-ttu-id="d50b6-124">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d50b6-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d50b6-125">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="d50b6-125">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="d50b6-126">changeId</span><span class="sxs-lookup"><span data-stu-id="d50b6-126">changeId</span></span>|<span data-ttu-id="d50b6-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d50b6-127">String</span></span>|<span data-ttu-id="d50b6-128">ID exclusiva dessa alteração neste ciclo.</span><span class="sxs-lookup"><span data-stu-id="d50b6-128">Unique ID of this change in this cycle.</span></span>|
|<span data-ttu-id="d50b6-129">cycleId</span><span class="sxs-lookup"><span data-stu-id="d50b6-129">cycleId</span></span>|<span data-ttu-id="d50b6-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d50b6-130">String</span></span>|<span data-ttu-id="d50b6-131">ID exclusiva por iteração de trabalho.</span><span class="sxs-lookup"><span data-stu-id="d50b6-131">Unique ID per job iteration.</span></span>|
|<span data-ttu-id="d50b6-132">durationInMilliseconds</span><span class="sxs-lookup"><span data-stu-id="d50b6-132">durationInMilliseconds</span></span>|<span data-ttu-id="d50b6-133">Int32</span><span class="sxs-lookup"><span data-stu-id="d50b6-133">Int32</span></span>|<span data-ttu-id="d50b6-134">Indica quanto tempo essa ação de provisionamento levou para ser final.</span><span class="sxs-lookup"><span data-stu-id="d50b6-134">Indicates how long this provisioning action took to finish.</span></span> <span data-ttu-id="d50b6-135">Medido em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="d50b6-135">Measured in milliseconds.</span></span>|
|<span data-ttu-id="d50b6-136">id</span><span class="sxs-lookup"><span data-stu-id="d50b6-136">id</span></span>|<span data-ttu-id="d50b6-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d50b6-137">String</span></span>| <span data-ttu-id="d50b6-138">Indica que a ID exclusiva para a atividade.</span><span class="sxs-lookup"><span data-stu-id="d50b6-138">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="d50b6-139">Este é um GUID somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d50b6-139">This is a read-only GUID.</span></span>|
|<span data-ttu-id="d50b6-140">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="d50b6-140">initiatedBy</span></span>|[<span data-ttu-id="d50b6-141">Iniciador</span><span class="sxs-lookup"><span data-stu-id="d50b6-141">initiator</span></span>](initiator.md)|<span data-ttu-id="d50b6-142">Detalhes de quem iniciou esse provisionamento.</span><span class="sxs-lookup"><span data-stu-id="d50b6-142">Details of who initiated this provisioning.</span></span>|
|<span data-ttu-id="d50b6-143">jobId</span><span class="sxs-lookup"><span data-stu-id="d50b6-143">jobId</span></span>|<span data-ttu-id="d50b6-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d50b6-144">String</span></span>|<span data-ttu-id="d50b6-145">A ID exclusiva para todo o trabalho de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="d50b6-145">The unique ID for the whole provisioning job.</span></span>|
|<span data-ttu-id="d50b6-146">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="d50b6-146">modifiedProperties</span></span>|<span data-ttu-id="d50b6-147">[Coleção modifiedProperty](modifiedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="d50b6-147">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="d50b6-148">Detalhes de cada propriedade que foi modificada nesta ação de provisionamento neste objeto.</span><span class="sxs-lookup"><span data-stu-id="d50b6-148">Details of each property that was modified in this provisioning action on this object.</span></span>|
|<span data-ttu-id="d50b6-149">provisioningSteps</span><span class="sxs-lookup"><span data-stu-id="d50b6-149">provisioningSteps</span></span>|<span data-ttu-id="d50b6-150">[Coleção provisioningStep](provisioningstep.md)</span><span class="sxs-lookup"><span data-stu-id="d50b6-150">[provisioningStep](provisioningstep.md) collection</span></span>|<span data-ttu-id="d50b6-151">Detalhes de cada etapa no provisionamento.</span><span class="sxs-lookup"><span data-stu-id="d50b6-151">Details of each step in provisioning.</span></span>|
|<span data-ttu-id="d50b6-152">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="d50b6-152">servicePrincipal</span></span>|<span data-ttu-id="d50b6-153">[servicePrincipal](provisioningserviceprincipal.md) collection</span><span class="sxs-lookup"><span data-stu-id="d50b6-153">[servicePrincipal](provisioningserviceprincipal.md) collection</span></span>|<span data-ttu-id="d50b6-154">Representa a entidade de serviço usada para provisionamento.</span><span class="sxs-lookup"><span data-stu-id="d50b6-154">Represents the service principal used for provisioning.</span></span>|
|<span data-ttu-id="d50b6-155">sourceIdentity</span><span class="sxs-lookup"><span data-stu-id="d50b6-155">sourceIdentity</span></span>|[<span data-ttu-id="d50b6-156">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="d50b6-156">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="d50b6-157">Detalhes do objeto de origem que está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="d50b6-157">Details of source object being provisioned.</span></span>|
|<span data-ttu-id="d50b6-158">sourceSystem</span><span class="sxs-lookup"><span data-stu-id="d50b6-158">sourceSystem</span></span>|[<span data-ttu-id="d50b6-159">provisioningSystem</span><span class="sxs-lookup"><span data-stu-id="d50b6-159">provisioningSystem</span></span>](provisioningsystem.md)|<span data-ttu-id="d50b6-160">Detalhes do sistema de origem do objeto que está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="d50b6-160">Details of source system of the object being provisioned.</span></span>|
|<span data-ttu-id="d50b6-161">provisioningStatusInfo</span><span class="sxs-lookup"><span data-stu-id="d50b6-161">provisioningStatusInfo</span></span>|[<span data-ttu-id="d50b6-162">provisioningStatusInfo</span><span class="sxs-lookup"><span data-stu-id="d50b6-162">provisioningStatusInfo</span></span>](provisioningstatusinfo.md)|<span data-ttu-id="d50b6-163">Detalhes do status do provisionamento.</span><span class="sxs-lookup"><span data-stu-id="d50b6-163">Details of provisioning status.</span></span>|
|<span data-ttu-id="d50b6-164">targetIdentity</span><span class="sxs-lookup"><span data-stu-id="d50b6-164">targetIdentity</span></span>|[<span data-ttu-id="d50b6-165">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="d50b6-165">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="d50b6-166">Detalhes do objeto de destino que está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="d50b6-166">Details of target object being provisioned.</span></span>|
|<span data-ttu-id="d50b6-167">targetSystem</span><span class="sxs-lookup"><span data-stu-id="d50b6-167">targetSystem</span></span>|[<span data-ttu-id="d50b6-168">provisioningSystem</span><span class="sxs-lookup"><span data-stu-id="d50b6-168">provisioningSystem</span></span>](provisioningsystem.md)|<span data-ttu-id="d50b6-169">Detalhes do sistema de destino do objeto que está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="d50b6-169">Details of target system of the object being provisioned.</span></span>|
|<span data-ttu-id="d50b6-170">tenantId</span><span class="sxs-lookup"><span data-stu-id="d50b6-170">tenantId</span></span>|<span data-ttu-id="d50b6-171">String</span><span class="sxs-lookup"><span data-stu-id="d50b6-171">String</span></span>|<span data-ttu-id="d50b6-172">ID exclusiva do locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d50b6-172">Unique Azure AD tenant ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d50b6-173">Relações</span><span class="sxs-lookup"><span data-stu-id="d50b6-173">Relationships</span></span>

<span data-ttu-id="d50b6-174">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d50b6-174">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d50b6-175">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d50b6-175">JSON representation</span></span>

<span data-ttu-id="d50b6-176">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d50b6-176">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "keyProperty": "id"
}-->

```json
{
  "provisioningAction":  "String",
  "activityDateTime": "String (timestamp)",
  "changeId": "String",
  "cycleId": "String",
  "durationInMilliseconds": 1024,
  "id": "String (identifier)",
  "initiatedBy": {"@odata.type": "microsoft.graph.initiator"},
  "jobId": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}],
  "provisioningSteps": [{"@odata.type": "microsoft.graph.provisioningStep"}],
  "servicePrincipal": [{"@odata.type": "microsoft.graph.provisioningServicePrincipal"}],
  "sourceIdentity": {"@odata.type": "microsoft.graph.provisionedIdentity"},
  "sourceSystem": {"@odata.type": "microsoft.graph.provisioningSystem"},
  "provisioningStatusInfo": {"@odata.type": "microsoft.graph.provisioningStatusInfo"},
  "targetIdentity": {"@odata.type": "microsoft.graph.provisionedIdentity"},
  "targetSystem": {"@odata.type": "microsoft.graph.provisioningSystem"},
  "tenantId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningObjectSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


