---
title: tipo de recurso onPremisesPublishingProfile
description: tipo de recurso onPremisesPublishingProfile.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 94d09955ad20af1117b156e433c95f2914df7348
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522197"
---
# <a name="onpremisespublishingprofile-resource-type"></a><span data-ttu-id="77f99-103">tipo de recurso onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="77f99-103">onPremisesPublishingProfile resource type</span></span>

<span data-ttu-id="77f99-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="77f99-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77f99-105">Vários serviços do Azure (por exemplo, autenticação de passagem do Azure Active Directory Connect, WORKDAY para o provisionamento de usuários do Azure AD) permitem um acesso condicional a vários recursos locais de fora da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="77f99-105">Various Azure services (for example, Azure Active Directory Connect Passthrough Authentication, Workday to Azure AD users provisioning) allow a conditional access to various on-premises resources from outside the corporate network.</span></span> <span data-ttu-id="77f99-106">[Os agentes locais](onpremisesagent.md) instalados por um administrador de locatários podem ser configurados para acessar/lidar com solicitações de um [recurso publicado](publishedresource.md)específico.</span><span class="sxs-lookup"><span data-stu-id="77f99-106">[On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="77f99-107">Os [grupos de agentes](onpremisesagentgroup.md) permitem que um administrador de locatários atribua agentes específicos para atender recursos locais publicados específicos.</span><span class="sxs-lookup"><span data-stu-id="77f99-107">[Agent groups](onpremisesagentgroup.md) enable a tenant admin to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="77f99-108">Os administradores de locatários podem agrupar vários agentes e, em seguida, atribuir cada recurso publicado a um grupo.</span><span class="sxs-lookup"><span data-stu-id="77f99-108">Tenant admins can group a number of agents together, and then assign each published resource to a group.</span></span> <span data-ttu-id="77f99-109">Todo o conjunto de entidades do mesmo tipo de publicação local é representado pelo **onPremisesPublishingProfile**.</span><span class="sxs-lookup"><span data-stu-id="77f99-109">The entire set of entities of the same on-premises publishing type is represented by **onPremisesPublishingProfile**.</span></span>

## <a name="methods"></a><span data-ttu-id="77f99-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="77f99-110">Methods</span></span>

| <span data-ttu-id="77f99-111">Método</span><span class="sxs-lookup"><span data-stu-id="77f99-111">Method</span></span>       | <span data-ttu-id="77f99-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="77f99-112">Return Type</span></span> | <span data-ttu-id="77f99-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="77f99-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="77f99-114">Obter onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="77f99-114">Get onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-get.md) | [<span data-ttu-id="77f99-115">onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="77f99-115">onPremisesPublishingProfile</span></span>](onpremisespublishingprofile.md) | <span data-ttu-id="77f99-116">Leia as propriedades e os relacionamentos de um objeto **onPremisesPublishingProfile** .</span><span class="sxs-lookup"><span data-stu-id="77f99-116">Read the properties and relationships of an **onPremisesPublishingProfile** object.</span></span> |
| [<span data-ttu-id="77f99-117">Atualizar onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="77f99-117">Update onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-update.md) | <span data-ttu-id="77f99-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="77f99-118">None</span></span> | <span data-ttu-id="77f99-119">Atualize um objeto [onPremisesPublishingProfile](onpremisespublishingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="77f99-119">Update an [onPremisesPublishingProfile](onpremisespublishingprofile.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="77f99-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="77f99-120">Properties</span></span>

| <span data-ttu-id="77f99-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77f99-121">Property</span></span>     | <span data-ttu-id="77f99-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="77f99-122">Type</span></span>        | <span data-ttu-id="77f99-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="77f99-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="77f99-124">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="77f99-124">hybridAgentUpdaterConfiguration</span></span>|[<span data-ttu-id="77f99-125">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="77f99-125">hybridAgentUpdaterConfiguration</span></span>](hybridagentupdaterconfiguration.md)| <span data-ttu-id="77f99-126">Representa um objeto **hybridAgentUpdaterConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="77f99-126">Represents a **hybridAgentUpdaterConfiguration** object.</span></span>|
|<span data-ttu-id="77f99-127">id</span><span class="sxs-lookup"><span data-stu-id="77f99-127">id</span></span>|<span data-ttu-id="77f99-128">String</span><span class="sxs-lookup"><span data-stu-id="77f99-128">String</span></span>| <span data-ttu-id="77f99-129">Representa um tipo de publicação.</span><span class="sxs-lookup"><span data-stu-id="77f99-129">Represents a publishing type.</span></span> <span data-ttu-id="77f99-130">Os valores possíveis são: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="77f99-130">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span> <span data-ttu-id="77f99-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="77f99-131">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77f99-132">Relações</span><span class="sxs-lookup"><span data-stu-id="77f99-132">Relationships</span></span>

| <span data-ttu-id="77f99-133">Relação</span><span class="sxs-lookup"><span data-stu-id="77f99-133">Relationship</span></span> | <span data-ttu-id="77f99-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="77f99-134">Type</span></span>        | <span data-ttu-id="77f99-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="77f99-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="77f99-136">agentGroups</span><span class="sxs-lookup"><span data-stu-id="77f99-136">agentGroups</span></span>|<span data-ttu-id="77f99-137">coleção [onPremisesAgentGroup](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="77f99-137">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="77f99-138">Lista de objetos **onPremisesAgentGroup** existentes.</span><span class="sxs-lookup"><span data-stu-id="77f99-138">List of existing **onPremisesAgentGroup** objects.</span></span> <span data-ttu-id="77f99-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="77f99-139">Read-only.</span></span> <span data-ttu-id="77f99-140">Anulável.</span><span class="sxs-lookup"><span data-stu-id="77f99-140">Nullable.</span></span>|
|<span data-ttu-id="77f99-141">SNMP</span><span class="sxs-lookup"><span data-stu-id="77f99-141">agents</span></span>|<span data-ttu-id="77f99-142">coleção [onPremisesAgent](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="77f99-142">[onPremisesAgent](onpremisesagent.md) collection</span></span>| <span data-ttu-id="77f99-143">Lista de objetos **onPremisesAgent** existentes.</span><span class="sxs-lookup"><span data-stu-id="77f99-143">List of existed **onPremisesAgent** objects.</span></span> <span data-ttu-id="77f99-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="77f99-144">Read-only.</span></span> <span data-ttu-id="77f99-145">Anulável.</span><span class="sxs-lookup"><span data-stu-id="77f99-145">Nullable.</span></span>|
|<span data-ttu-id="77f99-146">publishedResources</span><span class="sxs-lookup"><span data-stu-id="77f99-146">publishedResources</span></span>|<span data-ttu-id="77f99-147">coleção [publishedResource](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="77f99-147">[publishedResource](publishedresource.md) collection</span></span>| <span data-ttu-id="77f99-148">Lista de objetos **publishedResource** existentes.</span><span class="sxs-lookup"><span data-stu-id="77f99-148">List of existing **publishedResource** objects.</span></span> <span data-ttu-id="77f99-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="77f99-149">Read-only.</span></span> <span data-ttu-id="77f99-150">Anulável.</span><span class="sxs-lookup"><span data-stu-id="77f99-150">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="77f99-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="77f99-151">JSON representation</span></span>

<span data-ttu-id="77f99-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="77f99-152">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "hybridAgentUpdaterConfiguration": {"@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration"},
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishingProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
