---
title: Tipo de recurso onPremisesAgent
description: Tipo de recurso onPremisesAgent.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 8269c2d2273df385c4815e2276f320a7e4f5b813
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135867"
---
# <a name="onpremisesagent-resource-type"></a><span data-ttu-id="cf51d-103">Tipo de recurso onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="cf51d-103">onPremisesAgent resource type</span></span>

<span data-ttu-id="cf51d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf51d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf51d-105">Representa o agente local.</span><span class="sxs-lookup"><span data-stu-id="cf51d-105">Represents on-premises agent.</span></span> <span data-ttu-id="cf51d-106">Agentes locais instalados por um administrador de locatários podem ser configurados para acessar/manipular solicitações para um determinado [recurso publicado.](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="cf51d-106">On-premises agents installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="cf51d-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="cf51d-107">Methods</span></span>

| <span data-ttu-id="cf51d-108">Método</span><span class="sxs-lookup"><span data-stu-id="cf51d-108">Method</span></span>       | <span data-ttu-id="cf51d-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cf51d-109">Return Type</span></span> | <span data-ttu-id="cf51d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf51d-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="cf51d-111">Listar onPremisesAgents</span><span class="sxs-lookup"><span data-stu-id="cf51d-111">List onPremisesAgents</span></span>](../api/onpremisesagent-list.md) | <span data-ttu-id="cf51d-112">[Coleção onPremisesAgent](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="cf51d-112">[onPremisesAgent](onpremisesagent.md) collection</span></span> | <span data-ttu-id="cf51d-113">Obter uma **coleção de objetos onPremisesAgents.**</span><span class="sxs-lookup"><span data-stu-id="cf51d-113">Get an **onPremisesAgents** object collection.</span></span> |
| [<span data-ttu-id="cf51d-114">Obter onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="cf51d-114">Get onPremisesAgent</span></span>](../api/onpremisesagent-get.md) | [<span data-ttu-id="cf51d-115">onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="cf51d-115">onPremisesAgent</span></span>](onpremisesagent.md) | <span data-ttu-id="cf51d-116">Leia as propriedades e os relacionamentos de um **objeto onPremisesAgent.**</span><span class="sxs-lookup"><span data-stu-id="cf51d-116">Read the properties and relationships of an **onPremisesAgent** object.</span></span> |
| [<span data-ttu-id="cf51d-117">Atribuir onPremisesAgent a onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="cf51d-117">Assign onPremisesAgent to onPremisesAgentGroup</span></span>](../api/onpremisesagent-post-agentgroups.md) | <span data-ttu-id="cf51d-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="cf51d-118">None</span></span> | <span data-ttu-id="cf51d-119">Atribua **um onPremisesAgent** a **um onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="cf51d-119">Assign an **onPremisesAgent** to an **onPremisesAgentGroup**.</span></span>|
| [<span data-ttu-id="cf51d-120">Remover onpremisesAgent de um onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="cf51d-120">Remove onpremisesAgent from an onPremisesAgentGroup</span></span>](../api/onpremisesagent-delete-agentgroups.md) | <span data-ttu-id="cf51d-121">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="cf51d-121">None</span></span> | <span data-ttu-id="cf51d-122">Remover um **onPremisesAgent** de **um onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="cf51d-122">Remove an **onPremisesAgent** from an **onPremisesAgentGroup**.</span></span> |

## <a name="properties"></a><span data-ttu-id="cf51d-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf51d-123">Properties</span></span>

| <span data-ttu-id="cf51d-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf51d-124">Property</span></span>     | <span data-ttu-id="cf51d-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf51d-125">Type</span></span>        | <span data-ttu-id="cf51d-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf51d-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cf51d-127">externalIp</span><span class="sxs-lookup"><span data-stu-id="cf51d-127">externalIp</span></span>|<span data-ttu-id="cf51d-128">String</span><span class="sxs-lookup"><span data-stu-id="cf51d-128">String</span></span>|<span data-ttu-id="cf51d-129">O endereço IP externo conforme detectado pelo serviço para o computador do agente.</span><span class="sxs-lookup"><span data-stu-id="cf51d-129">The external IP address as detected by the service for the agent machine.</span></span> <span data-ttu-id="cf51d-130">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="cf51d-130">Read-only</span></span>|
|<span data-ttu-id="cf51d-131">id</span><span class="sxs-lookup"><span data-stu-id="cf51d-131">id</span></span>|<span data-ttu-id="cf51d-132">String</span><span class="sxs-lookup"><span data-stu-id="cf51d-132">String</span></span>| <span data-ttu-id="cf51d-133">A ID do objeto do onPremisesAgent.</span><span class="sxs-lookup"><span data-stu-id="cf51d-133">The object id of the onPremisesAgent.</span></span> <span data-ttu-id="cf51d-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cf51d-134">Read-only.</span></span>|
|<span data-ttu-id="cf51d-135">machineName</span><span class="sxs-lookup"><span data-stu-id="cf51d-135">machineName</span></span>|<span data-ttu-id="cf51d-136">String</span><span class="sxs-lookup"><span data-stu-id="cf51d-136">String</span></span>|<span data-ttu-id="cf51d-137">O nome do computador em que o agregação está sendo executado.</span><span class="sxs-lookup"><span data-stu-id="cf51d-137">The name of the machine that the aggent is running on.</span></span> <span data-ttu-id="cf51d-138">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="cf51d-138">Read-only</span></span>|
|<span data-ttu-id="cf51d-139">status</span><span class="sxs-lookup"><span data-stu-id="cf51d-139">status</span></span>|<span data-ttu-id="cf51d-140">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf51d-140">string</span></span>| <span data-ttu-id="cf51d-141">Os valores possíveis são: `active` e `inactive`.</span><span class="sxs-lookup"><span data-stu-id="cf51d-141">Possible values are: `active`, `inactive`.</span></span>|
|<span data-ttu-id="cf51d-142">publishingType</span><span class="sxs-lookup"><span data-stu-id="cf51d-142">publishingType</span></span>|<span data-ttu-id="cf51d-143">string</span><span class="sxs-lookup"><span data-stu-id="cf51d-143">string</span></span>| <span data-ttu-id="cf51d-144">Os valores possíveis são: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="cf51d-144">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf51d-145">Relações</span><span class="sxs-lookup"><span data-stu-id="cf51d-145">Relationships</span></span>

| <span data-ttu-id="cf51d-146">Relação</span><span class="sxs-lookup"><span data-stu-id="cf51d-146">Relationship</span></span> | <span data-ttu-id="cf51d-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf51d-147">Type</span></span>        | <span data-ttu-id="cf51d-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf51d-148">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cf51d-149">agentGroups</span><span class="sxs-lookup"><span data-stu-id="cf51d-149">agentGroups</span></span>|<span data-ttu-id="cf51d-150">[Coleção onPremisesAgentGroup](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="cf51d-150">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="cf51d-151">Lista de **onPremisesAgentGroups** aos que um **onPremisesAgent** está atribuído.</span><span class="sxs-lookup"><span data-stu-id="cf51d-151">List of **onPremisesAgentGroups** that an **onPremisesAgent** is assigned to.</span></span> <span data-ttu-id="cf51d-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cf51d-152">Read-only.</span></span> <span data-ttu-id="cf51d-153">Anulável.</span><span class="sxs-lookup"><span data-stu-id="cf51d-153">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cf51d-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf51d-154">JSON representation</span></span>

<span data-ttu-id="cf51d-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cf51d-155">The following is a JSON representation of the resource.</span></span>

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



