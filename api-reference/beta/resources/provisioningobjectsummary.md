---
title: tipo de recurso provisioningObjectSummary
description: Representa uma ação executada pelo serviço de provisionamento do Azure AD e suas propriedades associadas.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c9eabbb0c0cd1cd692ad6ebc5a346c46473161b1
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394593"
---
# <a name="provisioningobjectsummary-resource-type"></a><span data-ttu-id="ae7f8-103">tipo de recurso provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="ae7f8-103">provisioningObjectSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae7f8-104">Representa uma ação executada pelo serviço de provisionamento do Azure AD e suas propriedades associadas.</span><span class="sxs-lookup"><span data-stu-id="ae7f8-104">Represents an action performed by the Azure AD Provisioning service and its associated properties.</span></span> 

## <a name="methods"></a><span data-ttu-id="ae7f8-105">Methods</span><span class="sxs-lookup"><span data-stu-id="ae7f8-105">Methods</span></span>

| <span data-ttu-id="ae7f8-106">Método</span><span class="sxs-lookup"><span data-stu-id="ae7f8-106">Method</span></span>       | <span data-ttu-id="ae7f8-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ae7f8-107">Return Type</span></span> | <span data-ttu-id="ae7f8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae7f8-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ae7f8-109">Listar provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="ae7f8-109">List provisioningObjectSummary</span></span>](../api/provisioningobjectsummary-list.md) | [<span data-ttu-id="ae7f8-110">provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="ae7f8-110">provisioningObjectSummary</span></span>](provisioningobjectsummary.md) | <span data-ttu-id="ae7f8-111">Obtenha uma lista de todos os eventos de provisionamento que ocorreram em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="ae7f8-111">Get a list of all provisioning events that occurred in your tenant.</span></span> |


## <a name="properties"></a><span data-ttu-id="ae7f8-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ae7f8-112">Properties</span></span>

| <span data-ttu-id="ae7f8-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae7f8-113">Property</span></span>     | <span data-ttu-id="ae7f8-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae7f8-114">Type</span></span>        | <span data-ttu-id="ae7f8-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae7f8-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ae7f8-116">ação</span><span class="sxs-lookup"><span data-stu-id="ae7f8-116">action</span></span>|<span data-ttu-id="ae7f8-117">String</span><span class="sxs-lookup"><span data-stu-id="ae7f8-117">String</span></span>|<span data-ttu-id="ae7f8-118">Indica o nome da atividade ou o nome da operação (por exemplo, criar usuário, Adicionar membro ao grupo).</span><span class="sxs-lookup"><span data-stu-id="ae7f8-118">Indicates the activity name or the operation name (for example, Create user, Add member to group).</span></span> <span data-ttu-id="ae7f8-119">Para obter uma lista de atividades registradas, consulte lista de atividades do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ae7f8-119">For a list of activities logged, refer to Azure AD activity list.</span></span>|
|<span data-ttu-id="ae7f8-120">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="ae7f8-120">activityDateTime</span></span>|<span data-ttu-id="ae7f8-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae7f8-121">DateTimeOffset</span></span>|<span data-ttu-id="ae7f8-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ae7f8-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ae7f8-124">ChangeId</span><span class="sxs-lookup"><span data-stu-id="ae7f8-124">changeId</span></span>|<span data-ttu-id="ae7f8-125">String</span><span class="sxs-lookup"><span data-stu-id="ae7f8-125">String</span></span>|<span data-ttu-id="ae7f8-126">ID exclusiva dessa alteração nesse ciclo.</span><span class="sxs-lookup"><span data-stu-id="ae7f8-126">Unique ID of this change in this cycle.</span></span>|
|<span data-ttu-id="ae7f8-127">cycleid</span><span class="sxs-lookup"><span data-stu-id="ae7f8-127">cycleId</span></span>|<span data-ttu-id="ae7f8-128">String</span><span class="sxs-lookup"><span data-stu-id="ae7f8-128">String</span></span>|<span data-ttu-id="ae7f8-129">ID exclusiva por iteração de trabalho.</span><span class="sxs-lookup"><span data-stu-id="ae7f8-129">Unique ID per job iteration.</span></span>|
|<span data-ttu-id="ae7f8-130">durationInMilliseconds</span><span class="sxs-lookup"><span data-stu-id="ae7f8-130">durationInMilliseconds</span></span>|<span data-ttu-id="ae7f8-131">Int32</span><span class="sxs-lookup"><span data-stu-id="ae7f8-131">Int32</span></span>|<span data-ttu-id="ae7f8-132">Indica quanto tempo esta ação de provisionamento levou para ser concluída.</span><span class="sxs-lookup"><span data-stu-id="ae7f8-132">Indicates how long this provisioning action took to finish.</span></span> <span data-ttu-id="ae7f8-133">Medido em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="ae7f8-133">Measured in milliseconds.</span></span>|
|<span data-ttu-id="ae7f8-134">id</span><span class="sxs-lookup"><span data-stu-id="ae7f8-134">id</span></span>|<span data-ttu-id="ae7f8-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae7f8-135">String</span></span>| <span data-ttu-id="ae7f8-136">Indica que a ID exclusiva para a atividade.</span><span class="sxs-lookup"><span data-stu-id="ae7f8-136">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="ae7f8-137">Este é um GUID somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ae7f8-137">This is a read-only GUID.</span></span>|
|<span data-ttu-id="ae7f8-138">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="ae7f8-138">initiatedBy</span></span>|[<span data-ttu-id="ae7f8-139">Iniciador</span><span class="sxs-lookup"><span data-stu-id="ae7f8-139">initiator</span></span>](initiator.md)|<span data-ttu-id="ae7f8-140">Detalhes sobre quem iniciou este provisionamento.</span><span class="sxs-lookup"><span data-stu-id="ae7f8-140">Details of who initiated this provisioning.</span></span>|
|<span data-ttu-id="ae7f8-141">ID</span><span class="sxs-lookup"><span data-stu-id="ae7f8-141">jobId</span></span>|<span data-ttu-id="ae7f8-142">String</span><span class="sxs-lookup"><span data-stu-id="ae7f8-142">String</span></span>|<span data-ttu-id="ae7f8-143">A identificação exclusiva de todo o trabalho de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="ae7f8-143">The unique ID for the whole provisioning job.</span></span>|
|<span data-ttu-id="ae7f8-144">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="ae7f8-144">modifiedProperties</span></span>|<span data-ttu-id="ae7f8-145">coleção [modifiedproperty](modifiedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="ae7f8-145">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="ae7f8-146">Os detalhes de cada propriedade que foi modificada nesta ação de provisionamento neste objeto.</span><span class="sxs-lookup"><span data-stu-id="ae7f8-146">Details of each property that was modified in this provisioning action on this object.</span></span>|
|<span data-ttu-id="ae7f8-147">provisioningSteps</span><span class="sxs-lookup"><span data-stu-id="ae7f8-147">provisioningSteps</span></span>|<span data-ttu-id="ae7f8-148">coleção [provisioningStep](provisioningstep.md)</span><span class="sxs-lookup"><span data-stu-id="ae7f8-148">[provisioningStep](provisioningstep.md) collection</span></span>|<span data-ttu-id="ae7f8-149">Detalhes de cada etapa no provisionamento.</span><span class="sxs-lookup"><span data-stu-id="ae7f8-149">Details of each step in provisioning.</span></span>|
|<span data-ttu-id="ae7f8-150">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="ae7f8-150">servicePrincipal</span></span>|<span data-ttu-id="ae7f8-151">[servicePrincipal](serviceprincipal.md) collection</span><span class="sxs-lookup"><span data-stu-id="ae7f8-151">[servicePrincipal](serviceprincipal.md) collection</span></span>|<span data-ttu-id="ae7f8-152">Representa a entidade de serviço usada para provisionamento.</span><span class="sxs-lookup"><span data-stu-id="ae7f8-152">Represents the service principal used for provisioning.</span></span>|
|<span data-ttu-id="ae7f8-153">sourceIdentity</span><span class="sxs-lookup"><span data-stu-id="ae7f8-153">sourceIdentity</span></span>|[<span data-ttu-id="ae7f8-154">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="ae7f8-154">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="ae7f8-155">Detalhes do objeto de origem que está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="ae7f8-155">Details of source object being provisioned.</span></span>|
|<span data-ttu-id="ae7f8-156">sourceSystem</span><span class="sxs-lookup"><span data-stu-id="ae7f8-156">sourceSystem</span></span>|[<span data-ttu-id="ae7f8-157">provisioningSystemDetails</span><span class="sxs-lookup"><span data-stu-id="ae7f8-157">provisioningSystemDetails</span></span>](provisioningsystemdetails.md)|<span data-ttu-id="ae7f8-158">Detalhes do sistema de origem do objeto que está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="ae7f8-158">Details of source system of the object being provisioned.</span></span>|
|<span data-ttu-id="ae7f8-159">statusInfo</span><span class="sxs-lookup"><span data-stu-id="ae7f8-159">statusInfo</span></span>|[<span data-ttu-id="ae7f8-160">statusBase</span><span class="sxs-lookup"><span data-stu-id="ae7f8-160">statusBase</span></span>](statusbase.md)|<span data-ttu-id="ae7f8-161">Detalhes do status de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="ae7f8-161">Details of provisioning status.</span></span>|
|<span data-ttu-id="ae7f8-162">targetIdentity</span><span class="sxs-lookup"><span data-stu-id="ae7f8-162">targetIdentity</span></span>|[<span data-ttu-id="ae7f8-163">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="ae7f8-163">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="ae7f8-164">Detalhes do objeto de destino que está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="ae7f8-164">Details of target object being provisioned.</span></span>|
|<span data-ttu-id="ae7f8-165">targetSystem</span><span class="sxs-lookup"><span data-stu-id="ae7f8-165">targetSystem</span></span>|[<span data-ttu-id="ae7f8-166">provisioningSystemDetails</span><span class="sxs-lookup"><span data-stu-id="ae7f8-166">provisioningSystemDetails</span></span>](provisioningsystemdetails.md)|<span data-ttu-id="ae7f8-167">Detalhes do sistema de destino do objeto que está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="ae7f8-167">Details of target system of the object being provisioned.</span></span>|
|<span data-ttu-id="ae7f8-168">tenantId</span><span class="sxs-lookup"><span data-stu-id="ae7f8-168">tenantId</span></span>|<span data-ttu-id="ae7f8-169">String</span><span class="sxs-lookup"><span data-stu-id="ae7f8-169">String</span></span>|<span data-ttu-id="ae7f8-170">ID exclusiva do locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ae7f8-170">Unique Azure AD tenant ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae7f8-171">Relações</span><span class="sxs-lookup"><span data-stu-id="ae7f8-171">Relationships</span></span>

<span data-ttu-id="ae7f8-172">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ae7f8-172">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae7f8-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ae7f8-173">JSON representation</span></span>

<span data-ttu-id="ae7f8-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ae7f8-174">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "action": "String",
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
  "sourceSystem": {"@odata.type": "microsoft.graph.provisioningSystemDetails"},
  "statusInfo": {"@odata.type": "microsoft.graph.statusBase"},
  "targetIdentity": {"@odata.type": "microsoft.graph.provisionedIdentity"},
  "targetSystem": {"@odata.type": "microsoft.graph.provisioningSystemDetails"},
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
