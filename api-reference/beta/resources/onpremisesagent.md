---
title: tipo de recurso onPremisesAgent
description: tipo de recurso onPremisesAgent.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ec125e52eaf9eba3423f70dd47cc7dd1562716bb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052588"
---
# <a name="onpremisesagent-resource-type"></a><span data-ttu-id="f0cdf-103">tipo de recurso onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="f0cdf-103">onPremisesAgent resource type</span></span>

<span data-ttu-id="f0cdf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0cdf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0cdf-105">Representa o agente local.</span><span class="sxs-lookup"><span data-stu-id="f0cdf-105">Represents on-premises agent.</span></span> <span data-ttu-id="f0cdf-106">Os agentes locais instalados por um administrador de locatários podem ser configurados para acessar/lidar com solicitações de um [recurso publicado](publishedresource.md)específico.</span><span class="sxs-lookup"><span data-stu-id="f0cdf-106">On-premises agents installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f0cdf-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="f0cdf-107">Methods</span></span>

| <span data-ttu-id="f0cdf-108">Método</span><span class="sxs-lookup"><span data-stu-id="f0cdf-108">Method</span></span>       | <span data-ttu-id="f0cdf-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f0cdf-109">Return Type</span></span> | <span data-ttu-id="f0cdf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0cdf-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f0cdf-111">Listar onPremisesAgents</span><span class="sxs-lookup"><span data-stu-id="f0cdf-111">List onPremisesAgents</span></span>](../api/onpremisesagent-list.md) | <span data-ttu-id="f0cdf-112">coleção [onPremisesAgent](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="f0cdf-112">[onPremisesAgent](onpremisesagent.md) collection</span></span> | <span data-ttu-id="f0cdf-113">Obtenha uma coleção de objetos **onPremisesAgents** .</span><span class="sxs-lookup"><span data-stu-id="f0cdf-113">Get an **onPremisesAgents** object collection.</span></span> |
| [<span data-ttu-id="f0cdf-114">Obter onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="f0cdf-114">Get onPremisesAgent</span></span>](../api/onpremisesagent-get.md) | [<span data-ttu-id="f0cdf-115">onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="f0cdf-115">onPremisesAgent</span></span>](onpremisesagent.md) | <span data-ttu-id="f0cdf-116">Leia as propriedades e os relacionamentos de um objeto **onPremisesAgent** .</span><span class="sxs-lookup"><span data-stu-id="f0cdf-116">Read the properties and relationships of an **onPremisesAgent** object.</span></span> |
| [<span data-ttu-id="f0cdf-117">Atribuir onPremisesAgent a onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="f0cdf-117">Assign onPremisesAgent to onPremisesAgentGroup</span></span>](../api/onpremisesagent-post-agentgroups.md) | <span data-ttu-id="f0cdf-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f0cdf-118">None</span></span> | <span data-ttu-id="f0cdf-119">Atribua um **onPremisesAgent** a um **onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="f0cdf-119">Assign an **onPremisesAgent** to an **onPremisesAgentGroup**.</span></span>|
| [<span data-ttu-id="f0cdf-120">Remover o onpremisesAgent de um onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="f0cdf-120">Remove onpremisesAgent from an onPremisesAgentGroup</span></span>](../api/onpremisesagent-delete-agentgroups.md) | <span data-ttu-id="f0cdf-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f0cdf-121">None</span></span> | <span data-ttu-id="f0cdf-122">Remover um **onPremisesAgent** de um **onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="f0cdf-122">Remove an **onPremisesAgent** from an **onPremisesAgentGroup**.</span></span> |

## <a name="properties"></a><span data-ttu-id="f0cdf-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0cdf-123">Properties</span></span>

| <span data-ttu-id="f0cdf-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0cdf-124">Property</span></span>     | <span data-ttu-id="f0cdf-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0cdf-125">Type</span></span>        | <span data-ttu-id="f0cdf-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0cdf-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f0cdf-127">externalIp</span><span class="sxs-lookup"><span data-stu-id="f0cdf-127">externalIp</span></span>|<span data-ttu-id="f0cdf-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0cdf-128">String</span></span>|<span data-ttu-id="f0cdf-129">O endereço IP externo, conforme detectado pelo serviço para o computador do agente.</span><span class="sxs-lookup"><span data-stu-id="f0cdf-129">The external IP address as detected by the service for the agent machine.</span></span> <span data-ttu-id="f0cdf-130">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="f0cdf-130">Read-only</span></span>|
|<span data-ttu-id="f0cdf-131">id</span><span class="sxs-lookup"><span data-stu-id="f0cdf-131">id</span></span>|<span data-ttu-id="f0cdf-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0cdf-132">String</span></span>| <span data-ttu-id="f0cdf-133">A ID de objeto do onPremisesAgent.</span><span class="sxs-lookup"><span data-stu-id="f0cdf-133">The object id of the onPremisesAgent.</span></span> <span data-ttu-id="f0cdf-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0cdf-134">Read-only.</span></span>|
|<span data-ttu-id="f0cdf-135">Nomecomputador</span><span class="sxs-lookup"><span data-stu-id="f0cdf-135">machineName</span></span>|<span data-ttu-id="f0cdf-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0cdf-136">String</span></span>|<span data-ttu-id="f0cdf-137">O nome da máquina na qual o aggent está sendo executado.</span><span class="sxs-lookup"><span data-stu-id="f0cdf-137">The name of the machine that the aggent is running on.</span></span> <span data-ttu-id="f0cdf-138">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="f0cdf-138">Read-only</span></span>|
|<span data-ttu-id="f0cdf-139">status</span><span class="sxs-lookup"><span data-stu-id="f0cdf-139">status</span></span>|<span data-ttu-id="f0cdf-140">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0cdf-140">string</span></span>| <span data-ttu-id="f0cdf-141">Os valores possíveis são: `active` e `inactive`.</span><span class="sxs-lookup"><span data-stu-id="f0cdf-141">Possible values are: `active`, `inactive`.</span></span>|
|<span data-ttu-id="f0cdf-142">publishingtype</span><span class="sxs-lookup"><span data-stu-id="f0cdf-142">publishingType</span></span>|<span data-ttu-id="f0cdf-143">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0cdf-143">string</span></span>| <span data-ttu-id="f0cdf-144">Os valores possíveis são: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="f0cdf-144">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0cdf-145">Relações</span><span class="sxs-lookup"><span data-stu-id="f0cdf-145">Relationships</span></span>

| <span data-ttu-id="f0cdf-146">Relação</span><span class="sxs-lookup"><span data-stu-id="f0cdf-146">Relationship</span></span> | <span data-ttu-id="f0cdf-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0cdf-147">Type</span></span>        | <span data-ttu-id="f0cdf-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0cdf-148">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f0cdf-149">agentGroups</span><span class="sxs-lookup"><span data-stu-id="f0cdf-149">agentGroups</span></span>|<span data-ttu-id="f0cdf-150">coleção [onPremisesAgentGroup](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="f0cdf-150">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="f0cdf-151">Lista de **onPremisesAgentGroups** aos quais um **onPremisesAgent** é atribuído.</span><span class="sxs-lookup"><span data-stu-id="f0cdf-151">List of **onPremisesAgentGroups** that an **onPremisesAgent** is assigned to.</span></span> <span data-ttu-id="f0cdf-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0cdf-152">Read-only.</span></span> <span data-ttu-id="f0cdf-153">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f0cdf-153">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0cdf-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0cdf-154">JSON representation</span></span>

<span data-ttu-id="f0cdf-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f0cdf-155">The following is a JSON representation of the resource.</span></span>

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


