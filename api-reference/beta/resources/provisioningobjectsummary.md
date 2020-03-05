---
title: tipo de recurso provisioningObjectSummary
description: Representa uma ação executada pelo serviço de provisionamento do Azure AD e suas propriedades associadas.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ed6b760af60900436d22da4ae1302f458d50c4c6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521338"
---
# <a name="provisioningobjectsummary-resource-type"></a><span data-ttu-id="4b1fa-103">tipo de recurso provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="4b1fa-103">provisioningObjectSummary resource type</span></span>

<span data-ttu-id="4b1fa-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4b1fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b1fa-105">Representa uma ação executada pelo serviço de provisionamento do Azure AD e suas propriedades associadas.</span><span class="sxs-lookup"><span data-stu-id="4b1fa-105">Represents an action performed by the Azure AD Provisioning service and its associated properties.</span></span> 

## <a name="methods"></a><span data-ttu-id="4b1fa-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="4b1fa-106">Methods</span></span>

| <span data-ttu-id="4b1fa-107">Método</span><span class="sxs-lookup"><span data-stu-id="4b1fa-107">Method</span></span>       | <span data-ttu-id="4b1fa-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4b1fa-108">Return Type</span></span> | <span data-ttu-id="4b1fa-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b1fa-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4b1fa-110">Listar provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="4b1fa-110">List provisioningObjectSummary</span></span>](../api/provisioningobjectsummary-list.md) | [<span data-ttu-id="4b1fa-111">provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="4b1fa-111">provisioningObjectSummary</span></span>](provisioningobjectsummary.md) | <span data-ttu-id="4b1fa-112">Obtenha uma lista de todos os eventos de provisionamento que ocorreram em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="4b1fa-112">Get a list of all provisioning events that occurred in your tenant.</span></span> |


## <a name="properties"></a><span data-ttu-id="4b1fa-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4b1fa-113">Properties</span></span>

| <span data-ttu-id="4b1fa-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b1fa-114">Property</span></span>     | <span data-ttu-id="4b1fa-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b1fa-115">Type</span></span>        | <span data-ttu-id="4b1fa-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b1fa-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4b1fa-117">ação</span><span class="sxs-lookup"><span data-stu-id="4b1fa-117">action</span></span>|<span data-ttu-id="4b1fa-118">String</span><span class="sxs-lookup"><span data-stu-id="4b1fa-118">String</span></span>|<span data-ttu-id="4b1fa-119">Indica o nome da atividade ou o nome da operação (por exemplo, criar usuário, Adicionar membro ao grupo).</span><span class="sxs-lookup"><span data-stu-id="4b1fa-119">Indicates the activity name or the operation name (for example, Create user, Add member to group).</span></span> <span data-ttu-id="4b1fa-120">Para obter uma lista de atividades registradas, consulte lista de atividades do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4b1fa-120">For a list of activities logged, refer to Azure AD activity list.</span></span>|
|<span data-ttu-id="4b1fa-121">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="4b1fa-121">activityDateTime</span></span>|<span data-ttu-id="4b1fa-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b1fa-122">DateTimeOffset</span></span>|<span data-ttu-id="4b1fa-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4b1fa-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4b1fa-125">ChangeId</span><span class="sxs-lookup"><span data-stu-id="4b1fa-125">changeId</span></span>|<span data-ttu-id="4b1fa-126">String</span><span class="sxs-lookup"><span data-stu-id="4b1fa-126">String</span></span>|<span data-ttu-id="4b1fa-127">ID exclusiva dessa alteração nesse ciclo.</span><span class="sxs-lookup"><span data-stu-id="4b1fa-127">Unique ID of this change in this cycle.</span></span>|
|<span data-ttu-id="4b1fa-128">cycleid</span><span class="sxs-lookup"><span data-stu-id="4b1fa-128">cycleId</span></span>|<span data-ttu-id="4b1fa-129">String</span><span class="sxs-lookup"><span data-stu-id="4b1fa-129">String</span></span>|<span data-ttu-id="4b1fa-130">ID exclusiva por iteração de trabalho.</span><span class="sxs-lookup"><span data-stu-id="4b1fa-130">Unique ID per job iteration.</span></span>|
|<span data-ttu-id="4b1fa-131">durationInMilliseconds</span><span class="sxs-lookup"><span data-stu-id="4b1fa-131">durationInMilliseconds</span></span>|<span data-ttu-id="4b1fa-132">Int32</span><span class="sxs-lookup"><span data-stu-id="4b1fa-132">Int32</span></span>|<span data-ttu-id="4b1fa-133">Indica quanto tempo esta ação de provisionamento levou para ser concluída.</span><span class="sxs-lookup"><span data-stu-id="4b1fa-133">Indicates how long this provisioning action took to finish.</span></span> <span data-ttu-id="4b1fa-134">Medido em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="4b1fa-134">Measured in milliseconds.</span></span>|
|<span data-ttu-id="4b1fa-135">id</span><span class="sxs-lookup"><span data-stu-id="4b1fa-135">id</span></span>|<span data-ttu-id="4b1fa-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b1fa-136">String</span></span>| <span data-ttu-id="4b1fa-137">Indica que a ID exclusiva para a atividade.</span><span class="sxs-lookup"><span data-stu-id="4b1fa-137">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="4b1fa-138">Este é um GUID somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4b1fa-138">This is a read-only GUID.</span></span>|
|<span data-ttu-id="4b1fa-139">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="4b1fa-139">initiatedBy</span></span>|[<span data-ttu-id="4b1fa-140">Iniciador</span><span class="sxs-lookup"><span data-stu-id="4b1fa-140">initiator</span></span>](initiator.md)|<span data-ttu-id="4b1fa-141">Detalhes sobre quem iniciou este provisionamento.</span><span class="sxs-lookup"><span data-stu-id="4b1fa-141">Details of who initiated this provisioning.</span></span>|
|<span data-ttu-id="4b1fa-142">ID</span><span class="sxs-lookup"><span data-stu-id="4b1fa-142">jobId</span></span>|<span data-ttu-id="4b1fa-143">String</span><span class="sxs-lookup"><span data-stu-id="4b1fa-143">String</span></span>|<span data-ttu-id="4b1fa-144">A identificação exclusiva de todo o trabalho de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="4b1fa-144">The unique ID for the whole provisioning job.</span></span>|
|<span data-ttu-id="4b1fa-145">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="4b1fa-145">modifiedProperties</span></span>|<span data-ttu-id="4b1fa-146">coleção [modifiedproperty](modifiedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="4b1fa-146">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="4b1fa-147">Os detalhes de cada propriedade que foi modificada nesta ação de provisionamento neste objeto.</span><span class="sxs-lookup"><span data-stu-id="4b1fa-147">Details of each property that was modified in this provisioning action on this object.</span></span>|
|<span data-ttu-id="4b1fa-148">provisioningSteps</span><span class="sxs-lookup"><span data-stu-id="4b1fa-148">provisioningSteps</span></span>|<span data-ttu-id="4b1fa-149">coleção [provisioningStep](provisioningstep.md)</span><span class="sxs-lookup"><span data-stu-id="4b1fa-149">[provisioningStep](provisioningstep.md) collection</span></span>|<span data-ttu-id="4b1fa-150">Detalhes de cada etapa no provisionamento.</span><span class="sxs-lookup"><span data-stu-id="4b1fa-150">Details of each step in provisioning.</span></span>|
|<span data-ttu-id="4b1fa-151">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="4b1fa-151">servicePrincipal</span></span>|<span data-ttu-id="4b1fa-152">[servicePrincipal](serviceprincipal.md) collection</span><span class="sxs-lookup"><span data-stu-id="4b1fa-152">[servicePrincipal](serviceprincipal.md) collection</span></span>|<span data-ttu-id="4b1fa-153">Representa a entidade de serviço usada para provisionamento.</span><span class="sxs-lookup"><span data-stu-id="4b1fa-153">Represents the service principal used for provisioning.</span></span>|
|<span data-ttu-id="4b1fa-154">sourceIdentity</span><span class="sxs-lookup"><span data-stu-id="4b1fa-154">sourceIdentity</span></span>|[<span data-ttu-id="4b1fa-155">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="4b1fa-155">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="4b1fa-156">Detalhes do objeto de origem que está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="4b1fa-156">Details of source object being provisioned.</span></span>|
|<span data-ttu-id="4b1fa-157">sourceSystem</span><span class="sxs-lookup"><span data-stu-id="4b1fa-157">sourceSystem</span></span>|[<span data-ttu-id="4b1fa-158">provisioningSystemDetails</span><span class="sxs-lookup"><span data-stu-id="4b1fa-158">provisioningSystemDetails</span></span>](provisioningsystemdetails.md)|<span data-ttu-id="4b1fa-159">Detalhes do sistema de origem do objeto que está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="4b1fa-159">Details of source system of the object being provisioned.</span></span>|
|<span data-ttu-id="4b1fa-160">statusInfo</span><span class="sxs-lookup"><span data-stu-id="4b1fa-160">statusInfo</span></span>|[<span data-ttu-id="4b1fa-161">statusBase</span><span class="sxs-lookup"><span data-stu-id="4b1fa-161">statusBase</span></span>](statusbase.md)|<span data-ttu-id="4b1fa-162">Detalhes do status de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="4b1fa-162">Details of provisioning status.</span></span>|
|<span data-ttu-id="4b1fa-163">targetIdentity</span><span class="sxs-lookup"><span data-stu-id="4b1fa-163">targetIdentity</span></span>|[<span data-ttu-id="4b1fa-164">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="4b1fa-164">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="4b1fa-165">Detalhes do objeto de destino que está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="4b1fa-165">Details of target object being provisioned.</span></span>|
|<span data-ttu-id="4b1fa-166">targetSystem</span><span class="sxs-lookup"><span data-stu-id="4b1fa-166">targetSystem</span></span>|[<span data-ttu-id="4b1fa-167">provisioningSystemDetails</span><span class="sxs-lookup"><span data-stu-id="4b1fa-167">provisioningSystemDetails</span></span>](provisioningsystemdetails.md)|<span data-ttu-id="4b1fa-168">Detalhes do sistema de destino do objeto que está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="4b1fa-168">Details of target system of the object being provisioned.</span></span>|
|<span data-ttu-id="4b1fa-169">tenantId</span><span class="sxs-lookup"><span data-stu-id="4b1fa-169">tenantId</span></span>|<span data-ttu-id="4b1fa-170">String</span><span class="sxs-lookup"><span data-stu-id="4b1fa-170">String</span></span>|<span data-ttu-id="4b1fa-171">ID exclusiva do locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4b1fa-171">Unique Azure AD tenant ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b1fa-172">Relações</span><span class="sxs-lookup"><span data-stu-id="4b1fa-172">Relationships</span></span>

<span data-ttu-id="4b1fa-173">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4b1fa-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b1fa-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4b1fa-174">JSON representation</span></span>

<span data-ttu-id="4b1fa-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4b1fa-175">The following is a JSON representation of the resource.</span></span>

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
