---
title: Tipo de recurso onPremisesAgent
description: Tipo de recurso onPremisesAgent.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 59ee11bb952c85695b8c20daa1e040c8899740b9
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158349"
---
# <a name="onpremisesagent-resource-type"></a><span data-ttu-id="8d9d5-103">Tipo de recurso onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="8d9d5-103">onPremisesAgent resource type</span></span>

<span data-ttu-id="8d9d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d9d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d9d5-105">Representa o agente local.</span><span class="sxs-lookup"><span data-stu-id="8d9d5-105">Represents on-premises agent.</span></span> <span data-ttu-id="8d9d5-106">Agentes locais instalados por um administrador de locatários podem ser configurados para acessar/manipular solicitações para um determinado [recurso publicado.](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="8d9d5-106">On-premises agents installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8d9d5-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="8d9d5-107">Methods</span></span>

| <span data-ttu-id="8d9d5-108">Método</span><span class="sxs-lookup"><span data-stu-id="8d9d5-108">Method</span></span>       | <span data-ttu-id="8d9d5-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8d9d5-109">Return Type</span></span> | <span data-ttu-id="8d9d5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d9d5-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8d9d5-111">Listar onPremisesAgents</span><span class="sxs-lookup"><span data-stu-id="8d9d5-111">List onPremisesAgents</span></span>](../api/onpremisesagent-list.md) | <span data-ttu-id="8d9d5-112">[Coleção onPremisesAgent](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="8d9d5-112">[onPremisesAgent](onpremisesagent.md) collection</span></span> | <span data-ttu-id="8d9d5-113">Obter uma **coleção de objetos onPremisesAgents.**</span><span class="sxs-lookup"><span data-stu-id="8d9d5-113">Get an **onPremisesAgents** object collection.</span></span> |
| [<span data-ttu-id="8d9d5-114">Obter onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="8d9d5-114">Get onPremisesAgent</span></span>](../api/onpremisesagent-get.md) | [<span data-ttu-id="8d9d5-115">onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="8d9d5-115">onPremisesAgent</span></span>](onpremisesagent.md) | <span data-ttu-id="8d9d5-116">Leia as propriedades e os relacionamentos de um **objeto onPremisesAgent.**</span><span class="sxs-lookup"><span data-stu-id="8d9d5-116">Read the properties and relationships of an **onPremisesAgent** object.</span></span> |
| [<span data-ttu-id="8d9d5-117">Atribuir onPremisesAgent a onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="8d9d5-117">Assign onPremisesAgent to onPremisesAgentGroup</span></span>](../api/onpremisesagent-post-agentgroups.md) | <span data-ttu-id="8d9d5-118">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="8d9d5-118">None</span></span> | <span data-ttu-id="8d9d5-119">Atribua **um onPremisesAgent** a **um onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="8d9d5-119">Assign an **onPremisesAgent** to an **onPremisesAgentGroup**.</span></span>|
| [<span data-ttu-id="8d9d5-120">Remover onpremisesAgent de um onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="8d9d5-120">Remove onpremisesAgent from an onPremisesAgentGroup</span></span>](../api/onpremisesagent-delete-agentgroups.md) | <span data-ttu-id="8d9d5-121">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="8d9d5-121">None</span></span> | <span data-ttu-id="8d9d5-122">Remover um **onPremisesAgent** de **um onPremisesAgentGroup**.</span><span class="sxs-lookup"><span data-stu-id="8d9d5-122">Remove an **onPremisesAgent** from an **onPremisesAgentGroup**.</span></span> |

## <a name="properties"></a><span data-ttu-id="8d9d5-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8d9d5-123">Properties</span></span>

| <span data-ttu-id="8d9d5-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d9d5-124">Property</span></span>     | <span data-ttu-id="8d9d5-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d9d5-125">Type</span></span>        | <span data-ttu-id="8d9d5-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d9d5-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8d9d5-127">externalIp</span><span class="sxs-lookup"><span data-stu-id="8d9d5-127">externalIp</span></span>|<span data-ttu-id="8d9d5-128">String</span><span class="sxs-lookup"><span data-stu-id="8d9d5-128">String</span></span>|<span data-ttu-id="8d9d5-129">O endereço IP externo conforme detectado pelo serviço para o computador do agente.</span><span class="sxs-lookup"><span data-stu-id="8d9d5-129">The external IP address as detected by the service for the agent machine.</span></span> <span data-ttu-id="8d9d5-130">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="8d9d5-130">Read-only</span></span>|
|<span data-ttu-id="8d9d5-131">id</span><span class="sxs-lookup"><span data-stu-id="8d9d5-131">id</span></span>|<span data-ttu-id="8d9d5-132">String</span><span class="sxs-lookup"><span data-stu-id="8d9d5-132">String</span></span>| <span data-ttu-id="8d9d5-133">A ID do objeto do onPremisesAgent.</span><span class="sxs-lookup"><span data-stu-id="8d9d5-133">The object id of the onPremisesAgent.</span></span> <span data-ttu-id="8d9d5-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8d9d5-134">Read-only.</span></span>|
|<span data-ttu-id="8d9d5-135">machineName</span><span class="sxs-lookup"><span data-stu-id="8d9d5-135">machineName</span></span>|<span data-ttu-id="8d9d5-136">String</span><span class="sxs-lookup"><span data-stu-id="8d9d5-136">String</span></span>|<span data-ttu-id="8d9d5-137">O nome do computador em que o agregação está sendo executado.</span><span class="sxs-lookup"><span data-stu-id="8d9d5-137">The name of the machine that the aggent is running on.</span></span> <span data-ttu-id="8d9d5-138">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="8d9d5-138">Read-only</span></span>|
|<span data-ttu-id="8d9d5-139">status</span><span class="sxs-lookup"><span data-stu-id="8d9d5-139">status</span></span>|<span data-ttu-id="8d9d5-140">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d9d5-140">string</span></span>| <span data-ttu-id="8d9d5-141">Os valores possíveis são: `active` e `inactive`.</span><span class="sxs-lookup"><span data-stu-id="8d9d5-141">Possible values are: `active`, `inactive`.</span></span>|
|<span data-ttu-id="8d9d5-142">publishingType</span><span class="sxs-lookup"><span data-stu-id="8d9d5-142">publishingType</span></span>|<span data-ttu-id="8d9d5-143">string</span><span class="sxs-lookup"><span data-stu-id="8d9d5-143">string</span></span>| <span data-ttu-id="8d9d5-144">Os valores possíveis são: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="8d9d5-144">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d9d5-145">Relações</span><span class="sxs-lookup"><span data-stu-id="8d9d5-145">Relationships</span></span>

| <span data-ttu-id="8d9d5-146">Relação</span><span class="sxs-lookup"><span data-stu-id="8d9d5-146">Relationship</span></span> | <span data-ttu-id="8d9d5-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d9d5-147">Type</span></span>        | <span data-ttu-id="8d9d5-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d9d5-148">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8d9d5-149">agentGroups</span><span class="sxs-lookup"><span data-stu-id="8d9d5-149">agentGroups</span></span>|<span data-ttu-id="8d9d5-150">[Coleção onPremisesAgentGroup](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="8d9d5-150">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="8d9d5-151">Lista de **onPremisesAgentGroups** aos que um **onPremisesAgent** está atribuído.</span><span class="sxs-lookup"><span data-stu-id="8d9d5-151">List of **onPremisesAgentGroups** that an **onPremisesAgent** is assigned to.</span></span> <span data-ttu-id="8d9d5-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8d9d5-152">Read-only.</span></span> <span data-ttu-id="8d9d5-153">Anulável.</span><span class="sxs-lookup"><span data-stu-id="8d9d5-153">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d9d5-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8d9d5-154">JSON representation</span></span>

<span data-ttu-id="8d9d5-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8d9d5-155">The following is a JSON representation of the resource.</span></span>

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



