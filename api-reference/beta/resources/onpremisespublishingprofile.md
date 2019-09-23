---
title: tipo de recurso onPremisesPublishingProfile
description: tipo de recurso onPremisesPublishingProfile.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ce99713637d7607caed40451a0716cb0acde14e4
ms.sourcegitcommit: e87be8765d7f2bc90c6244d84c4719468bb3fd25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2019
ms.locfileid: "37113902"
---
# <a name="onpremisespublishingprofile-resource-type"></a><span data-ttu-id="68302-103">tipo de recurso onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="68302-103">onPremisesPublishingProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68302-104">Vários serviços do Azure (por exemplo, autenticação de passagem do Azure Active Directory Connect, WORKDAY para o provisionamento de usuários do Azure AD) permitem um acesso condicional a vários recursos locais de fora da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="68302-104">Various Azure services (for example, Azure Active Directory Connect Passthrough Authentication, Workday to Azure AD users provisioning) allow a conditional access to various on-premises resources from outside the corporate network.</span></span> <span data-ttu-id="68302-105">[Os agentes locais](onpremisesagent.md) instalados por um administrador de locatários podem ser configurados para acessar/lidar com solicitações de um [recurso publicado](publishedresource.md)específico.</span><span class="sxs-lookup"><span data-stu-id="68302-105">[On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="68302-106">Os [grupos de agentes](onpremisesagentgroup.md) permitem que um administrador de locatários atribua agentes específicos para atender recursos locais publicados específicos.</span><span class="sxs-lookup"><span data-stu-id="68302-106">[Agent groups](onpremisesagentgroup.md) enable a tenant admin to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="68302-107">Os administradores de locatários podem agrupar vários agentes e, em seguida, atribuir cada recurso publicado a um grupo.</span><span class="sxs-lookup"><span data-stu-id="68302-107">Tenant admins can group a number of agents together, and then assign each published resource to a group.</span></span> <span data-ttu-id="68302-108">Todo o conjunto de entidades do mesmo tipo de publicação local é representado pelo **onPremisesPublishingProfile**.</span><span class="sxs-lookup"><span data-stu-id="68302-108">The entire set of entities of the same on-premises publishing type is represented by **onPremisesPublishingProfile**.</span></span>

## <a name="methods"></a><span data-ttu-id="68302-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="68302-109">Methods</span></span>

| <span data-ttu-id="68302-110">Método</span><span class="sxs-lookup"><span data-stu-id="68302-110">Method</span></span>       | <span data-ttu-id="68302-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="68302-111">Return Type</span></span> | <span data-ttu-id="68302-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="68302-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="68302-113">Obter onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="68302-113">Get onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-get.md) | [<span data-ttu-id="68302-114">onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="68302-114">onPremisesPublishingProfile</span></span>](onpremisespublishingprofile.md) | <span data-ttu-id="68302-115">Leia as propriedades e os relacionamentos de um objeto **onPremisesPublishingProfile** .</span><span class="sxs-lookup"><span data-stu-id="68302-115">Read the properties and relationships of an **onPremisesPublishingProfile** object.</span></span> |
| [<span data-ttu-id="68302-116">Atualizar onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="68302-116">Update onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-update.md) | <span data-ttu-id="68302-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="68302-117">None</span></span> | <span data-ttu-id="68302-118">Atualize um objeto [onPremisesPublishingProfile](onpremisespublishingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="68302-118">Update an [onPremisesPublishingProfile](onpremisespublishingprofile.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="68302-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="68302-119">Properties</span></span>

| <span data-ttu-id="68302-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68302-120">Property</span></span>     | <span data-ttu-id="68302-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="68302-121">Type</span></span>        | <span data-ttu-id="68302-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="68302-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="68302-123">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="68302-123">hybridAgentUpdaterConfiguration</span></span>|[<span data-ttu-id="68302-124">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="68302-124">hybridAgentUpdaterConfiguration</span></span>](hybridagentupdaterconfiguration.md)| <span data-ttu-id="68302-125">Representa um objeto **hybridAgentUpdaterConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="68302-125">Represents a **hybridAgentUpdaterConfiguration** object.</span></span>|
|<span data-ttu-id="68302-126">id</span><span class="sxs-lookup"><span data-stu-id="68302-126">id</span></span>|<span data-ttu-id="68302-127">String</span><span class="sxs-lookup"><span data-stu-id="68302-127">String</span></span>| <span data-ttu-id="68302-128">Representa um tipo de publicação.</span><span class="sxs-lookup"><span data-stu-id="68302-128">Represents a publishing type.</span></span> <span data-ttu-id="68302-129">Os valores possíveis são: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="68302-129">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span> <span data-ttu-id="68302-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="68302-130">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68302-131">Relações</span><span class="sxs-lookup"><span data-stu-id="68302-131">Relationships</span></span>

| <span data-ttu-id="68302-132">Relação</span><span class="sxs-lookup"><span data-stu-id="68302-132">Relationship</span></span> | <span data-ttu-id="68302-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="68302-133">Type</span></span>        | <span data-ttu-id="68302-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="68302-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="68302-135">agentGroups</span><span class="sxs-lookup"><span data-stu-id="68302-135">agentGroups</span></span>|<span data-ttu-id="68302-136">coleção [onPremisesAgentGroup](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="68302-136">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="68302-137">Lista de objetos **onPremisesAgentGroup** existentes.</span><span class="sxs-lookup"><span data-stu-id="68302-137">List of existing **onPremisesAgentGroup** objects.</span></span> <span data-ttu-id="68302-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="68302-138">Read-only.</span></span> <span data-ttu-id="68302-139">Anulável.</span><span class="sxs-lookup"><span data-stu-id="68302-139">Nullable.</span></span>|
|<span data-ttu-id="68302-140">SNMP</span><span class="sxs-lookup"><span data-stu-id="68302-140">agents</span></span>|<span data-ttu-id="68302-141">coleção [onPremisesAgent](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="68302-141">[onPremisesAgent](onpremisesagent.md) collection</span></span>| <span data-ttu-id="68302-142">Lista de objetos **onPremisesAgent** existentes.</span><span class="sxs-lookup"><span data-stu-id="68302-142">List of existed **onPremisesAgent** objects.</span></span> <span data-ttu-id="68302-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="68302-143">Read-only.</span></span> <span data-ttu-id="68302-144">Anulável.</span><span class="sxs-lookup"><span data-stu-id="68302-144">Nullable.</span></span>|
|<span data-ttu-id="68302-145">publishedResources</span><span class="sxs-lookup"><span data-stu-id="68302-145">publishedResources</span></span>|<span data-ttu-id="68302-146">coleção [publishedResource](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="68302-146">[publishedResource](publishedresource.md) collection</span></span>| <span data-ttu-id="68302-147">Lista de objetos **publishedResource** existentes.</span><span class="sxs-lookup"><span data-stu-id="68302-147">List of existing **publishedResource** objects.</span></span> <span data-ttu-id="68302-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="68302-148">Read-only.</span></span> <span data-ttu-id="68302-149">Anulável.</span><span class="sxs-lookup"><span data-stu-id="68302-149">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="68302-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="68302-150">JSON representation</span></span>

<span data-ttu-id="68302-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="68302-151">The following is a JSON representation of the resource.</span></span>

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
