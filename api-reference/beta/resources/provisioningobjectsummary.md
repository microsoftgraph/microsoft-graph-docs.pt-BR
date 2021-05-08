---
title: Tipo de recurso provisioningObjectSummary
description: Representa uma ação executada pelo serviço de Provisionamento do Azure AD e suas propriedades associadas.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 7004a611c3fe36e2ce2d32824a5e9b78e53e61bd
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231910"
---
# <a name="provisioningobjectsummary-resource-type"></a><span data-ttu-id="9e778-103">Tipo de recurso provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="9e778-103">provisioningObjectSummary resource type</span></span>

<span data-ttu-id="9e778-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e778-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
>[!CAUTION]
><span data-ttu-id="9e778-105">As **propriedades action** e **statusInfo** são preterida.</span><span class="sxs-lookup"><span data-stu-id="9e778-105">The **action** and **statusInfo** properties are deprecated.</span></span> <span data-ttu-id="9e778-106">A **ação de** propriedade deve ser substituída pelo **provisionamentoAction**.</span><span class="sxs-lookup"><span data-stu-id="9e778-106">Property **action** should be replaced by **provisioningAction**.</span></span> <span data-ttu-id="9e778-107">Status **da propriedadeInfo** deve ser substituído por **provisioningStatusInfo**.</span><span class="sxs-lookup"><span data-stu-id="9e778-107">Property **statusInfo** should be replaced by **provisioningStatusInfo**.</span></span>

<span data-ttu-id="9e778-108">Representa uma ação executada pelo serviço de Provisionamento do Azure AD e suas propriedades associadas.</span><span class="sxs-lookup"><span data-stu-id="9e778-108">Represents an action performed by the Azure AD Provisioning service and its associated properties.</span></span> 

## <a name="methods"></a><span data-ttu-id="9e778-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="9e778-109">Methods</span></span>

| <span data-ttu-id="9e778-110">Método</span><span class="sxs-lookup"><span data-stu-id="9e778-110">Method</span></span>  | <span data-ttu-id="9e778-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9e778-111">Return Type</span></span> | <span data-ttu-id="9e778-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e778-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9e778-113">Listar provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="9e778-113">List provisioningObjectSummary</span></span>](../api/provisioningobjectsummary-list.md) | [<span data-ttu-id="9e778-114">provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="9e778-114">provisioningObjectSummary</span></span>](provisioningobjectsummary.md) | <span data-ttu-id="9e778-115">Obter uma lista de todos os eventos de provisionamento que ocorreram em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="9e778-115">Get a list of all provisioning events that occurred in your tenant.</span></span> |


## <a name="properties"></a><span data-ttu-id="9e778-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9e778-116">Properties</span></span>

| <span data-ttu-id="9e778-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e778-117">Property</span></span>     | <span data-ttu-id="9e778-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e778-118">Type</span></span>        | <span data-ttu-id="9e778-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e778-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9e778-120">provisioningAction</span><span class="sxs-lookup"><span data-stu-id="9e778-120">provisioningAction</span></span>|<span data-ttu-id="9e778-121">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e778-121">string</span></span>|<span data-ttu-id="9e778-122">Indica o nome da atividade ou o nome da operação.</span><span class="sxs-lookup"><span data-stu-id="9e778-122">Indicates the activity name or the operation name.</span></span> <span data-ttu-id="9e778-123">Os valores possíveis são: `create` , , , , e `update` `delete` `stageddelete` `disable` `other` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="9e778-123">Possible values are: `create`, `update`, `delete`, `stageddelete`, `disable`, `other` and `unknownFutureValue`.</span></span> <span data-ttu-id="9e778-124">Para uma lista de atividades registradas, consulte a lista de atividades do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9e778-124">For a list of activities logged, refer to Azure AD activity list.</span></span>|
|<span data-ttu-id="9e778-125">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="9e778-125">activityDateTime</span></span>|<span data-ttu-id="9e778-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e778-126">DateTimeOffset</span></span>|<span data-ttu-id="9e778-127">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="9e778-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9e778-128">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="9e778-128">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="9e778-129">changeId</span><span class="sxs-lookup"><span data-stu-id="9e778-129">changeId</span></span>|<span data-ttu-id="9e778-130">String</span><span class="sxs-lookup"><span data-stu-id="9e778-130">String</span></span>|<span data-ttu-id="9e778-131">ID exclusiva dessa alteração neste ciclo.</span><span class="sxs-lookup"><span data-stu-id="9e778-131">Unique ID of this change in this cycle.</span></span>|
|<span data-ttu-id="9e778-132">cycleId</span><span class="sxs-lookup"><span data-stu-id="9e778-132">cycleId</span></span>|<span data-ttu-id="9e778-133">String</span><span class="sxs-lookup"><span data-stu-id="9e778-133">String</span></span>|<span data-ttu-id="9e778-134">ID exclusiva por iteração de trabalho.</span><span class="sxs-lookup"><span data-stu-id="9e778-134">Unique ID per job iteration.</span></span>|
|<span data-ttu-id="9e778-135">durationInMilliseconds</span><span class="sxs-lookup"><span data-stu-id="9e778-135">durationInMilliseconds</span></span>|<span data-ttu-id="9e778-136">Int32</span><span class="sxs-lookup"><span data-stu-id="9e778-136">Int32</span></span>|<span data-ttu-id="9e778-137">Indica quanto tempo essa ação de provisionamento levou para ser final.</span><span class="sxs-lookup"><span data-stu-id="9e778-137">Indicates how long this provisioning action took to finish.</span></span> <span data-ttu-id="9e778-138">Medido em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="9e778-138">Measured in milliseconds.</span></span>|
|<span data-ttu-id="9e778-139">id</span><span class="sxs-lookup"><span data-stu-id="9e778-139">id</span></span>|<span data-ttu-id="9e778-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e778-140">String</span></span>| <span data-ttu-id="9e778-141">Indica que a ID exclusiva para a atividade.</span><span class="sxs-lookup"><span data-stu-id="9e778-141">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="9e778-142">Este é um GUID somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9e778-142">This is a read-only GUID.</span></span>|
|<span data-ttu-id="9e778-143">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="9e778-143">initiatedBy</span></span>|[<span data-ttu-id="9e778-144">Iniciador</span><span class="sxs-lookup"><span data-stu-id="9e778-144">initiator</span></span>](initiator.md)|<span data-ttu-id="9e778-145">Detalhes de quem iniciou esse provisionamento.</span><span class="sxs-lookup"><span data-stu-id="9e778-145">Details of who initiated this provisioning.</span></span>|
|<span data-ttu-id="9e778-146">jobId</span><span class="sxs-lookup"><span data-stu-id="9e778-146">jobId</span></span>|<span data-ttu-id="9e778-147">String</span><span class="sxs-lookup"><span data-stu-id="9e778-147">String</span></span>|<span data-ttu-id="9e778-148">A ID exclusiva para todo o trabalho de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="9e778-148">The unique ID for the whole provisioning job.</span></span>|
|<span data-ttu-id="9e778-149">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="9e778-149">modifiedProperties</span></span>|<span data-ttu-id="9e778-150">[Coleção modifiedProperty](modifiedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="9e778-150">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="9e778-151">Detalhes de cada propriedade que foi modificada nesta ação de provisionamento neste objeto.</span><span class="sxs-lookup"><span data-stu-id="9e778-151">Details of each property that was modified in this provisioning action on this object.</span></span>|
|<span data-ttu-id="9e778-152">provisioningSteps</span><span class="sxs-lookup"><span data-stu-id="9e778-152">provisioningSteps</span></span>|<span data-ttu-id="9e778-153">[Coleção provisioningStep](provisioningstep.md)</span><span class="sxs-lookup"><span data-stu-id="9e778-153">[provisioningStep](provisioningstep.md) collection</span></span>|<span data-ttu-id="9e778-154">Detalhes de cada etapa no provisionamento.</span><span class="sxs-lookup"><span data-stu-id="9e778-154">Details of each step in provisioning.</span></span>|
|<span data-ttu-id="9e778-155">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="9e778-155">servicePrincipal</span></span>|<span data-ttu-id="9e778-156">[servicePrincipal](serviceprincipal.md) collection</span><span class="sxs-lookup"><span data-stu-id="9e778-156">[servicePrincipal](serviceprincipal.md) collection</span></span>|<span data-ttu-id="9e778-157">Representa a entidade de serviço usada para provisionamento.</span><span class="sxs-lookup"><span data-stu-id="9e778-157">Represents the service principal used for provisioning.</span></span>|
|<span data-ttu-id="9e778-158">sourceIdentity</span><span class="sxs-lookup"><span data-stu-id="9e778-158">sourceIdentity</span></span>|[<span data-ttu-id="9e778-159">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="9e778-159">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="9e778-160">Detalhes do objeto de origem que está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="9e778-160">Details of source object being provisioned.</span></span>|
|<span data-ttu-id="9e778-161">sourceSystem</span><span class="sxs-lookup"><span data-stu-id="9e778-161">sourceSystem</span></span>|[<span data-ttu-id="9e778-162">provisioningSystem</span><span class="sxs-lookup"><span data-stu-id="9e778-162">provisioningSystem</span></span>](provisioningsystem.md)|<span data-ttu-id="9e778-163">Detalhes do sistema de origem do objeto que está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="9e778-163">Details of source system of the object being provisioned.</span></span>|
|<span data-ttu-id="9e778-164">provisioningStatusInfo</span><span class="sxs-lookup"><span data-stu-id="9e778-164">provisioningStatusInfo</span></span>|[<span data-ttu-id="9e778-165">provisioningStatusInfo</span><span class="sxs-lookup"><span data-stu-id="9e778-165">provisioningStatusInfo</span></span>](provisioningstatusinfo.md)|<span data-ttu-id="9e778-166">Detalhes do status do provisionamento.</span><span class="sxs-lookup"><span data-stu-id="9e778-166">Details of provisioning status.</span></span>|
|<span data-ttu-id="9e778-167">targetIdentity</span><span class="sxs-lookup"><span data-stu-id="9e778-167">targetIdentity</span></span>|[<span data-ttu-id="9e778-168">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="9e778-168">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="9e778-169">Detalhes do objeto de destino que está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="9e778-169">Details of target object being provisioned.</span></span>|
|<span data-ttu-id="9e778-170">targetSystem</span><span class="sxs-lookup"><span data-stu-id="9e778-170">targetSystem</span></span>|[<span data-ttu-id="9e778-171">provisioningSystem</span><span class="sxs-lookup"><span data-stu-id="9e778-171">provisioningSystem</span></span>](provisioningsystem.md)|<span data-ttu-id="9e778-172">Detalhes do sistema de destino do objeto que está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="9e778-172">Details of target system of the object being provisioned.</span></span>|
|<span data-ttu-id="9e778-173">tenantId</span><span class="sxs-lookup"><span data-stu-id="9e778-173">tenantId</span></span>|<span data-ttu-id="9e778-174">String</span><span class="sxs-lookup"><span data-stu-id="9e778-174">String</span></span>|<span data-ttu-id="9e778-175">ID exclusiva do locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9e778-175">Unique Azure AD tenant ID.</span></span>|
|<span data-ttu-id="9e778-176">action (preterido)</span><span class="sxs-lookup"><span data-stu-id="9e778-176">action (deprecated)</span></span>|<span data-ttu-id="9e778-177">String</span><span class="sxs-lookup"><span data-stu-id="9e778-177">String</span></span>|<span data-ttu-id="9e778-178">Indica o nome da atividade ou o nome da operação (por exemplo, Criar usuário, Adicionar membro ao grupo).</span><span class="sxs-lookup"><span data-stu-id="9e778-178">Indicates the activity name or the operation name (for example, Create user, Add member to group).</span></span> <span data-ttu-id="9e778-179">Para uma lista de atividades registradas, consulte a lista de atividades do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9e778-179">For a list of activities logged, refer to Azure AD activity list.</span></span> <span data-ttu-id="9e778-180">Isso é preterido.</span><span class="sxs-lookup"><span data-stu-id="9e778-180">This is deprecated.</span></span> <span data-ttu-id="9e778-181">Em vez disso, use provisioningAction.</span><span class="sxs-lookup"><span data-stu-id="9e778-181">Please use provisioningAction instead.</span></span>|
|<span data-ttu-id="9e778-182">statusInfo (preterido)</span><span class="sxs-lookup"><span data-stu-id="9e778-182">statusInfo (deprecated)</span></span>|[<span data-ttu-id="9e778-183">statusBase</span><span class="sxs-lookup"><span data-stu-id="9e778-183">statusBase</span></span>](statusbase.md)|<span data-ttu-id="9e778-184">Detalhes do status do provisionamento.</span><span class="sxs-lookup"><span data-stu-id="9e778-184">Details of provisioning status.</span></span> <span data-ttu-id="9e778-185">Isso é preterido.</span><span class="sxs-lookup"><span data-stu-id="9e778-185">This is deprecated.</span></span> <span data-ttu-id="9e778-186">Em vez disso, use provisioningStatusInfo.</span><span class="sxs-lookup"><span data-stu-id="9e778-186">Please use provisioningStatusInfo instead.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e778-187">Relações</span><span class="sxs-lookup"><span data-stu-id="9e778-187">Relationships</span></span>

<span data-ttu-id="9e778-188">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9e778-188">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e778-189">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9e778-189">JSON representation</span></span>

<span data-ttu-id="9e778-190">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9e778-190">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "keyProperty": "id"
}-->

```json
{
  "action": "String",
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
  "statusInfo": {"@odata.type": "microsoft.graph.statusBase"},
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


