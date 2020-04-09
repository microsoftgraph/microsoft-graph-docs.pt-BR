---
title: tipo de recurso onPremisesAgent
description: tipo de recurso onPremisesAgent.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fdc6355b33539899ab51a4a6881a8109cb8d87a6
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/09/2020
ms.locfileid: "43199750"
---
# <a name="onpremisesagent-resource-type"></a><span data-ttu-id="f151f-103">tipo de recurso onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="f151f-103">onPremisesAgent resource type</span></span>

<span data-ttu-id="f151f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f151f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f151f-105">Representa o agente local.</span><span class="sxs-lookup"><span data-stu-id="f151f-105">Represents on-premises agent.</span></span> <span data-ttu-id="f151f-106">Os agentes locais instalados por um administrador de locatários podem ser configurados para acessar/lidar com solicitações de um [recurso publicado](publishedresource.md)específico.</span><span class="sxs-lookup"><span data-stu-id="f151f-106">On-premises agents installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f151f-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="f151f-107">Methods</span></span>

| <span data-ttu-id="f151f-108">Método</span><span class="sxs-lookup"><span data-stu-id="f151f-108">Method</span></span>       | <span data-ttu-id="f151f-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f151f-109">Return Type</span></span> | <span data-ttu-id="f151f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f151f-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f151f-111">Listar onPremisesAgents</span><span class="sxs-lookup"><span data-stu-id="f151f-111">List onPremisesAgents</span></span>](../api/onpremisesagent-list.md) | <span data-ttu-id="f151f-112">coleção [onPremisesAgent](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="f151f-112">[onPremisesAgent](onpremisesagent.md) collection</span></span> | <span data-ttu-id="f151f-113">Obtenha uma coleção de objetos **onPremisesAgents** .</span><span class="sxs-lookup"><span data-stu-id="f151f-113">Get an **onPremisesAgents** object collection.</span></span> |
| [<span data-ttu-id="f151f-114">Obter onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="f151f-114">Get onPremisesAgent</span></span>](../api/onpremisesagent-get.md) | [<span data-ttu-id="f151f-115">onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="f151f-115">onPremisesAgent</span></span>](onpremisesagent.md) | <span data-ttu-id="f151f-116">Leia as propriedades e os relacionamentos de um objeto **onPremisesAgent** .</span><span class="sxs-lookup"><span data-stu-id="f151f-116">Read the properties and relationships of an **onPremisesAgent** object.</span></span> |
| [<span data-ttu-id="f151f-117">Atribuir onPremisesAgent a onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="f151f-117">Assign onPremisesAgent to onPremisesAgentGroup</span></span>](../api/onpremisesagent-post-agentgroups.md) | <span data-ttu-id="f151f-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f151f-118">None</span></span> | <span data-ttu-id="f151f-119">Atribua um **onPremisesAgent** a um **onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="f151f-119">Assign an **onPremisesAgent** to an **onPremisesAgentGroup**.</span></span>|
| [<span data-ttu-id="f151f-120">Remover o onpremisesAgent de um onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="f151f-120">Remove onpremisesAgent from an onPremisesAgentGroup</span></span>](../api/onpremisesagent-delete-agentgroups.md) | <span data-ttu-id="f151f-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f151f-121">None</span></span> | <span data-ttu-id="f151f-122">Remover um **onPremisesAgent** de um **onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="f151f-122">Remove an **onPremisesAgent** from an **onPremisesAgentGroup**.</span></span> |

## <a name="properties"></a><span data-ttu-id="f151f-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f151f-123">Properties</span></span>

| <span data-ttu-id="f151f-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f151f-124">Property</span></span>     | <span data-ttu-id="f151f-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="f151f-125">Type</span></span>        | <span data-ttu-id="f151f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="f151f-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f151f-127">externalIp</span><span class="sxs-lookup"><span data-stu-id="f151f-127">externalIp</span></span>|<span data-ttu-id="f151f-128">String</span><span class="sxs-lookup"><span data-stu-id="f151f-128">String</span></span>|<span data-ttu-id="f151f-129">O endereço IP externo, conforme detectado pelo serviço para o computador do agente.</span><span class="sxs-lookup"><span data-stu-id="f151f-129">The external IP address as detected by the service for the agent machine.</span></span> <span data-ttu-id="f151f-130">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="f151f-130">Read-only</span></span>|
|<span data-ttu-id="f151f-131">id</span><span class="sxs-lookup"><span data-stu-id="f151f-131">id</span></span>|<span data-ttu-id="f151f-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f151f-132">String</span></span>| <span data-ttu-id="f151f-133">A ID de objeto do onPremisesAgent.</span><span class="sxs-lookup"><span data-stu-id="f151f-133">The object id of the onPremisesAgent.</span></span> <span data-ttu-id="f151f-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f151f-134">Read-only.</span></span>|
|<span data-ttu-id="f151f-135">Nomecomputador</span><span class="sxs-lookup"><span data-stu-id="f151f-135">machineName</span></span>|<span data-ttu-id="f151f-136">String</span><span class="sxs-lookup"><span data-stu-id="f151f-136">String</span></span>|<span data-ttu-id="f151f-137">O nome da máquina na qual o aggent está sendo executado.</span><span class="sxs-lookup"><span data-stu-id="f151f-137">The name of the machine that the aggent is running on.</span></span> <span data-ttu-id="f151f-138">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="f151f-138">Read-only</span></span>|
|<span data-ttu-id="f151f-139">status</span><span class="sxs-lookup"><span data-stu-id="f151f-139">status</span></span>|<span data-ttu-id="f151f-140">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f151f-140">string</span></span>| <span data-ttu-id="f151f-141">Os valores possíveis são: `active` e `inactive`.</span><span class="sxs-lookup"><span data-stu-id="f151f-141">Possible values are: `active`, `inactive`.</span></span>|
|<span data-ttu-id="f151f-142">publishingtype</span><span class="sxs-lookup"><span data-stu-id="f151f-142">publishingType</span></span>|<span data-ttu-id="f151f-143">string</span><span class="sxs-lookup"><span data-stu-id="f151f-143">string</span></span>| <span data-ttu-id="f151f-144">Os valores possíveis são: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="f151f-144">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f151f-145">Relações</span><span class="sxs-lookup"><span data-stu-id="f151f-145">Relationships</span></span>

| <span data-ttu-id="f151f-146">Relação</span><span class="sxs-lookup"><span data-stu-id="f151f-146">Relationship</span></span> | <span data-ttu-id="f151f-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="f151f-147">Type</span></span>        | <span data-ttu-id="f151f-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="f151f-148">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f151f-149">agentGroups</span><span class="sxs-lookup"><span data-stu-id="f151f-149">agentGroups</span></span>|<span data-ttu-id="f151f-150">coleção [onPremisesAgentGroup](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="f151f-150">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="f151f-151">Lista de **onPremisesAgentGroups** aos quais um **onPremisesAgent** é atribuído.</span><span class="sxs-lookup"><span data-stu-id="f151f-151">List of **onPremisesAgentGroups** that an **onPremisesAgent** is assigned to.</span></span> <span data-ttu-id="f151f-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f151f-152">Read-only.</span></span> <span data-ttu-id="f151f-153">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f151f-153">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f151f-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f151f-154">JSON representation</span></span>

<span data-ttu-id="f151f-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f151f-155">The following is a JSON representation of the resource.</span></span>

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
