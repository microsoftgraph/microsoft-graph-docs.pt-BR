---
title: tipo de recurso onPremisesAgent
description: tipo de recurso onPremisesAgent.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1bcff659cf30b946654f14190b2cf5f693d27bc4
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841259"
---
# <a name="onpremisesagent-resource-type"></a><span data-ttu-id="9269d-103">tipo de recurso onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="9269d-103">onPremisesAgent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9269d-104">Representa o agente local.</span><span class="sxs-lookup"><span data-stu-id="9269d-104">Represents on-premises agent.</span></span> <span data-ttu-id="9269d-105">Os agentes locais instalados por um administrador de locatários podem ser configurados para acessar/lidar com solicitações de um [recurso publicado](publishedresource.md)específico.</span><span class="sxs-lookup"><span data-stu-id="9269d-105">On-premises agents installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9269d-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="9269d-106">Methods</span></span>

| <span data-ttu-id="9269d-107">Método</span><span class="sxs-lookup"><span data-stu-id="9269d-107">Method</span></span>       | <span data-ttu-id="9269d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9269d-108">Return Type</span></span> | <span data-ttu-id="9269d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9269d-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9269d-110">Listar onPremisesAgents</span><span class="sxs-lookup"><span data-stu-id="9269d-110">List onPremisesAgents</span></span>](../api/onpremisesagent-list.md) | <span data-ttu-id="9269d-111">coleção [onPremisesAgent](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="9269d-111">[onPremisesAgent](onpremisesagent.md) collection</span></span> | <span data-ttu-id="9269d-112">Obtenha uma coleção de objetos **onPremisesAgents** .</span><span class="sxs-lookup"><span data-stu-id="9269d-112">Get an **onPremisesAgents** object collection.</span></span> |
| [<span data-ttu-id="9269d-113">Obter onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="9269d-113">Get onPremisesAgent</span></span>](../api/onpremisesagent-get.md) | [<span data-ttu-id="9269d-114">onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="9269d-114">onPremisesAgent</span></span>](onpremisesagent.md) | <span data-ttu-id="9269d-115">Leia as propriedades e os relacionamentos de um objeto **onPremisesAgent** .</span><span class="sxs-lookup"><span data-stu-id="9269d-115">Read the properties and relationships of an **onPremisesAgent** object.</span></span> |
| [<span data-ttu-id="9269d-116">Atribuir onPremisesAgent a onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="9269d-116">Assign onPremisesAgent to onPremisesAgentGroup</span></span>](../api/onpremisesagent-post-agentgroups.md) | <span data-ttu-id="9269d-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9269d-117">None</span></span> | <span data-ttu-id="9269d-118">Atribua um **onPremisesAgent** a um **onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="9269d-118">Assign an **onPremisesAgent** to an **onPremisesAgentGroup**.</span></span>|
| [<span data-ttu-id="9269d-119">Remover o onpremisesAgent de um onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="9269d-119">Remove onpremisesAgent from an onPremisesAgentGroup</span></span>](../api/onpremisesagent-delete-agentgroups.md) | <span data-ttu-id="9269d-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9269d-120">None</span></span> | <span data-ttu-id="9269d-121">Remover um **onPremisesAgent** de um **onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="9269d-121">Remove an **onPremisesAgent** from an **onPremisesAgentGroup**.</span></span> |

## <a name="properties"></a><span data-ttu-id="9269d-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9269d-122">Properties</span></span>

| <span data-ttu-id="9269d-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9269d-123">Property</span></span>     | <span data-ttu-id="9269d-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="9269d-124">Type</span></span>        | <span data-ttu-id="9269d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="9269d-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9269d-126">externalIp</span><span class="sxs-lookup"><span data-stu-id="9269d-126">externalIp</span></span>|<span data-ttu-id="9269d-127">String</span><span class="sxs-lookup"><span data-stu-id="9269d-127">String</span></span>|<span data-ttu-id="9269d-128">O endereço IP externo, conforme detectado pelo serviço para o computador do agente.</span><span class="sxs-lookup"><span data-stu-id="9269d-128">The external IP address as detected by the service for the agent machine.</span></span> <span data-ttu-id="9269d-129">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="9269d-129">Read-only</span></span>|
|<span data-ttu-id="9269d-130">id</span><span class="sxs-lookup"><span data-stu-id="9269d-130">id</span></span>|<span data-ttu-id="9269d-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9269d-131">String</span></span>| <span data-ttu-id="9269d-132">A ID de objeto do onPremisesAgent.</span><span class="sxs-lookup"><span data-stu-id="9269d-132">The object id of the onPremisesAgent.</span></span> <span data-ttu-id="9269d-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9269d-133">Read-only.</span></span>|
|<span data-ttu-id="9269d-134">Nomecomputador</span><span class="sxs-lookup"><span data-stu-id="9269d-134">machineName</span></span>|<span data-ttu-id="9269d-135">String</span><span class="sxs-lookup"><span data-stu-id="9269d-135">String</span></span>|<span data-ttu-id="9269d-136">O nome da máquina na qual o aggent está sendo executado.</span><span class="sxs-lookup"><span data-stu-id="9269d-136">The name of the machine that the aggent is running on.</span></span> <span data-ttu-id="9269d-137">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="9269d-137">Read-only</span></span>|
|<span data-ttu-id="9269d-138">status</span><span class="sxs-lookup"><span data-stu-id="9269d-138">status</span></span>|<span data-ttu-id="9269d-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9269d-139">string</span></span>| <span data-ttu-id="9269d-140">Os valores possíveis são: `active` e `inactive`.</span><span class="sxs-lookup"><span data-stu-id="9269d-140">Possible values are: `active`, `inactive`.</span></span>|
|<span data-ttu-id="9269d-141">publishingtype</span><span class="sxs-lookup"><span data-stu-id="9269d-141">publishingType</span></span>|<span data-ttu-id="9269d-142">string</span><span class="sxs-lookup"><span data-stu-id="9269d-142">string</span></span>| <span data-ttu-id="9269d-143">Os valores possíveis são: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="9269d-143">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9269d-144">Relações</span><span class="sxs-lookup"><span data-stu-id="9269d-144">Relationships</span></span>

| <span data-ttu-id="9269d-145">Relação</span><span class="sxs-lookup"><span data-stu-id="9269d-145">Relationship</span></span> | <span data-ttu-id="9269d-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="9269d-146">Type</span></span>        | <span data-ttu-id="9269d-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="9269d-147">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9269d-148">agentGroups</span><span class="sxs-lookup"><span data-stu-id="9269d-148">agentGroups</span></span>|<span data-ttu-id="9269d-149">coleção [onPremisesAgentGroup](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="9269d-149">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="9269d-150">Lista de **onPremisesAgentGroups** aos quais um **onPremisesAgent** é atribuído.</span><span class="sxs-lookup"><span data-stu-id="9269d-150">List of **onPremisesAgentGroups** that an **onPremisesAgent** is assigned to.</span></span> <span data-ttu-id="9269d-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9269d-151">Read-only.</span></span> <span data-ttu-id="9269d-152">Anulável.</span><span class="sxs-lookup"><span data-stu-id="9269d-152">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9269d-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9269d-153">JSON representation</span></span>

<span data-ttu-id="9269d-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9269d-154">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgent",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "externalIp": "String",
  "id": "String (identifier)",
  "machineName": "String",
  "status": "string",
  "supportedPublishingTypes": ["string"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
