---
title: Tipo de recurso onPremisesAgent
description: Tipo de recurso onPremisesAgent.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 74128ab48e023f066f259fea5f326d5e1642eb14
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956929"
---
# <a name="onpremisesagent-resource-type"></a><span data-ttu-id="13d78-103">Tipo de recurso onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="13d78-103">onPremisesAgent resource type</span></span>

<span data-ttu-id="13d78-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13d78-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13d78-105">Representa o agente local.</span><span class="sxs-lookup"><span data-stu-id="13d78-105">Represents on-premises agent.</span></span> <span data-ttu-id="13d78-106">Agentes locais instalados por um administrador de locatários podem ser configurados para acessar/manipular solicitações para um determinado [recurso publicado.](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="13d78-106">On-premises agents installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="13d78-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="13d78-107">Methods</span></span>

| <span data-ttu-id="13d78-108">Método</span><span class="sxs-lookup"><span data-stu-id="13d78-108">Method</span></span>       | <span data-ttu-id="13d78-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="13d78-109">Return Type</span></span> | <span data-ttu-id="13d78-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="13d78-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="13d78-111">Listar onPremisesAgents</span><span class="sxs-lookup"><span data-stu-id="13d78-111">List onPremisesAgents</span></span>](../api/onpremisesagent-list.md) | <span data-ttu-id="13d78-112">[Coleção onPremisesAgent](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="13d78-112">[onPremisesAgent](onpremisesagent.md) collection</span></span> | <span data-ttu-id="13d78-113">Obter uma **coleção de objetos onPremisesAgents.**</span><span class="sxs-lookup"><span data-stu-id="13d78-113">Get an **onPremisesAgents** object collection.</span></span> |
| [<span data-ttu-id="13d78-114">Obter onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="13d78-114">Get onPremisesAgent</span></span>](../api/onpremisesagent-get.md) | [<span data-ttu-id="13d78-115">onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="13d78-115">onPremisesAgent</span></span>](onpremisesagent.md) | <span data-ttu-id="13d78-116">Leia as propriedades e as relações de um **objeto onPremisesAgent.**</span><span class="sxs-lookup"><span data-stu-id="13d78-116">Read the properties and relationships of an **onPremisesAgent** object.</span></span> |
| [<span data-ttu-id="13d78-117">Atribuir onPremisesAgent ao onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="13d78-117">Assign onPremisesAgent to onPremisesAgentGroup</span></span>](../api/onpremisesagent-post-agentgroups.md) | <span data-ttu-id="13d78-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="13d78-118">None</span></span> | <span data-ttu-id="13d78-119">Atribua **um onPremisesAgent** a **um onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="13d78-119">Assign an **onPremisesAgent** to an **onPremisesAgentGroup**.</span></span>|
| [<span data-ttu-id="13d78-120">Remover onpremisesAgent de um onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="13d78-120">Remove onpremisesAgent from an onPremisesAgentGroup</span></span>](../api/onpremisesagent-delete-agentgroups.md) | <span data-ttu-id="13d78-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="13d78-121">None</span></span> | <span data-ttu-id="13d78-122">Remova um **onPremisesAgent** de **um onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="13d78-122">Remove an **onPremisesAgent** from an **onPremisesAgentGroup**.</span></span> |

## <a name="properties"></a><span data-ttu-id="13d78-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="13d78-123">Properties</span></span>

| <span data-ttu-id="13d78-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13d78-124">Property</span></span>     | <span data-ttu-id="13d78-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="13d78-125">Type</span></span>        | <span data-ttu-id="13d78-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="13d78-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="13d78-127">externalIp</span><span class="sxs-lookup"><span data-stu-id="13d78-127">externalIp</span></span>|<span data-ttu-id="13d78-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13d78-128">String</span></span>|<span data-ttu-id="13d78-129">O endereço IP externo, conforme detectado pelo serviço para o computador do agente.</span><span class="sxs-lookup"><span data-stu-id="13d78-129">The external IP address as detected by the service for the agent machine.</span></span> <span data-ttu-id="13d78-130">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="13d78-130">Read-only</span></span>|
|<span data-ttu-id="13d78-131">id</span><span class="sxs-lookup"><span data-stu-id="13d78-131">id</span></span>|<span data-ttu-id="13d78-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13d78-132">String</span></span>| <span data-ttu-id="13d78-133">A id do objeto do onPremisesAgent.</span><span class="sxs-lookup"><span data-stu-id="13d78-133">The object id of the onPremisesAgent.</span></span> <span data-ttu-id="13d78-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="13d78-134">Read-only.</span></span>|
|<span data-ttu-id="13d78-135">machineName</span><span class="sxs-lookup"><span data-stu-id="13d78-135">machineName</span></span>|<span data-ttu-id="13d78-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13d78-136">String</span></span>|<span data-ttu-id="13d78-137">O nome do computador em que o aggent está sendo executado.</span><span class="sxs-lookup"><span data-stu-id="13d78-137">The name of the machine that the aggent is running on.</span></span> <span data-ttu-id="13d78-138">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="13d78-138">Read-only</span></span>|
|<span data-ttu-id="13d78-139">status</span><span class="sxs-lookup"><span data-stu-id="13d78-139">status</span></span>|<span data-ttu-id="13d78-140">agentStatus</span><span class="sxs-lookup"><span data-stu-id="13d78-140">agentStatus</span></span>| <span data-ttu-id="13d78-141">Os valores possíveis são: `active` e `inactive`.</span><span class="sxs-lookup"><span data-stu-id="13d78-141">Possible values are: `active`, `inactive`.</span></span>|
|<span data-ttu-id="13d78-142">publishingType</span><span class="sxs-lookup"><span data-stu-id="13d78-142">publishingType</span></span>|<span data-ttu-id="13d78-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13d78-143">String</span></span>| <span data-ttu-id="13d78-144">Os valores possíveis são: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="13d78-144">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13d78-145">Relações</span><span class="sxs-lookup"><span data-stu-id="13d78-145">Relationships</span></span>

| <span data-ttu-id="13d78-146">Relação</span><span class="sxs-lookup"><span data-stu-id="13d78-146">Relationship</span></span> | <span data-ttu-id="13d78-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="13d78-147">Type</span></span>        | <span data-ttu-id="13d78-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="13d78-148">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="13d78-149">agentGroups</span><span class="sxs-lookup"><span data-stu-id="13d78-149">agentGroups</span></span>|<span data-ttu-id="13d78-150">[Coleção onPremisesAgentGroup](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="13d78-150">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="13d78-151">Lista de **onPremisesAgentGroups** aos que um **onPremisesAgent** é atribuído.</span><span class="sxs-lookup"><span data-stu-id="13d78-151">List of **onPremisesAgentGroups** that an **onPremisesAgent** is assigned to.</span></span> <span data-ttu-id="13d78-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="13d78-152">Read-only.</span></span> <span data-ttu-id="13d78-153">Anulável.</span><span class="sxs-lookup"><span data-stu-id="13d78-153">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13d78-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="13d78-154">JSON representation</span></span>

<span data-ttu-id="13d78-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="13d78-155">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgent",
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



