---
title: tipo de recurso onPremisesPublishingProfile
description: tipo de recurso onPremisesPublishingProfile.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0a4e1e40a5a8774be9498f6b89d235557ba2948e
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200023"
---
# <a name="onpremisespublishingprofile-resource-type"></a><span data-ttu-id="8d928-103">tipo de recurso onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="8d928-103">onPremisesPublishingProfile resource type</span></span>

<span data-ttu-id="8d928-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d928-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d928-105">Vários serviços do Azure (por exemplo, autenticação de passagem do Azure Active Directory Connect, WORKDAY para o provisionamento de usuários do Azure AD) permitem um acesso condicional a vários recursos locais de fora da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="8d928-105">Various Azure services (for example, Azure Active Directory Connect Passthrough Authentication, Workday to Azure AD users provisioning) allow a conditional access to various on-premises resources from outside the corporate network.</span></span> <span data-ttu-id="8d928-106">[Os agentes locais](onpremisesagent.md) instalados por um administrador de locatários podem ser configurados para acessar/lidar com solicitações de um [recurso publicado](publishedresource.md)específico.</span><span class="sxs-lookup"><span data-stu-id="8d928-106">[On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="8d928-107">Os [grupos de agentes](onpremisesagentgroup.md) permitem que um administrador de locatários atribua agentes específicos para atender recursos locais publicados específicos.</span><span class="sxs-lookup"><span data-stu-id="8d928-107">[Agent groups](onpremisesagentgroup.md) enable a tenant admin to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="8d928-108">Os administradores de locatários podem agrupar vários agentes e, em seguida, atribuir cada recurso publicado a um grupo.</span><span class="sxs-lookup"><span data-stu-id="8d928-108">Tenant admins can group a number of agents together, and then assign each published resource to a group.</span></span> <span data-ttu-id="8d928-109">Todo o conjunto de entidades do mesmo tipo de publicação local é representado pelo **onPremisesPublishingProfile**.</span><span class="sxs-lookup"><span data-stu-id="8d928-109">The entire set of entities of the same on-premises publishing type is represented by **onPremisesPublishingProfile**.</span></span>

## <a name="methods"></a><span data-ttu-id="8d928-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="8d928-110">Methods</span></span>

| <span data-ttu-id="8d928-111">Método</span><span class="sxs-lookup"><span data-stu-id="8d928-111">Method</span></span>       | <span data-ttu-id="8d928-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8d928-112">Return Type</span></span> | <span data-ttu-id="8d928-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d928-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8d928-114">Obter onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="8d928-114">Get onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-get.md) | [<span data-ttu-id="8d928-115">onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="8d928-115">onPremisesPublishingProfile</span></span>](onpremisespublishingprofile.md) | <span data-ttu-id="8d928-116">Leia as propriedades e os relacionamentos de um objeto **onPremisesPublishingProfile** .</span><span class="sxs-lookup"><span data-stu-id="8d928-116">Read the properties and relationships of an **onPremisesPublishingProfile** object.</span></span> |
| [<span data-ttu-id="8d928-117">Atualizar onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="8d928-117">Update onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-update.md) | <span data-ttu-id="8d928-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8d928-118">None</span></span> | <span data-ttu-id="8d928-119">Atualize um objeto [onPremisesPublishingProfile](onpremisespublishingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="8d928-119">Update an [onPremisesPublishingProfile](onpremisespublishingprofile.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="8d928-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8d928-120">Properties</span></span>

| <span data-ttu-id="8d928-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d928-121">Property</span></span>     | <span data-ttu-id="8d928-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d928-122">Type</span></span>        | <span data-ttu-id="8d928-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d928-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8d928-124">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d928-124">hybridAgentUpdaterConfiguration</span></span>|[<span data-ttu-id="8d928-125">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d928-125">hybridAgentUpdaterConfiguration</span></span>](hybridagentupdaterconfiguration.md)| <span data-ttu-id="8d928-126">Representa um objeto **hybridAgentUpdaterConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="8d928-126">Represents a **hybridAgentUpdaterConfiguration** object.</span></span>|
|<span data-ttu-id="8d928-127">id</span><span class="sxs-lookup"><span data-stu-id="8d928-127">id</span></span>|<span data-ttu-id="8d928-128">String</span><span class="sxs-lookup"><span data-stu-id="8d928-128">String</span></span>| <span data-ttu-id="8d928-129">Representa um tipo de publicação.</span><span class="sxs-lookup"><span data-stu-id="8d928-129">Represents a publishing type.</span></span> <span data-ttu-id="8d928-130">Os valores possíveis são: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="8d928-130">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span> <span data-ttu-id="8d928-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8d928-131">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d928-132">Relações</span><span class="sxs-lookup"><span data-stu-id="8d928-132">Relationships</span></span>

| <span data-ttu-id="8d928-133">Relação</span><span class="sxs-lookup"><span data-stu-id="8d928-133">Relationship</span></span> | <span data-ttu-id="8d928-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d928-134">Type</span></span>        | <span data-ttu-id="8d928-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d928-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8d928-136">agentGroups</span><span class="sxs-lookup"><span data-stu-id="8d928-136">agentGroups</span></span>|<span data-ttu-id="8d928-137">coleção [onPremisesAgentGroup](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="8d928-137">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="8d928-138">Lista de objetos **onPremisesAgentGroup** existentes.</span><span class="sxs-lookup"><span data-stu-id="8d928-138">List of existing **onPremisesAgentGroup** objects.</span></span> <span data-ttu-id="8d928-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8d928-139">Read-only.</span></span> <span data-ttu-id="8d928-140">Anulável.</span><span class="sxs-lookup"><span data-stu-id="8d928-140">Nullable.</span></span>|
|<span data-ttu-id="8d928-141">SNMP</span><span class="sxs-lookup"><span data-stu-id="8d928-141">agents</span></span>|<span data-ttu-id="8d928-142">coleção [onPremisesAgent](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="8d928-142">[onPremisesAgent](onpremisesagent.md) collection</span></span>| <span data-ttu-id="8d928-143">Lista de objetos **onPremisesAgent** existentes.</span><span class="sxs-lookup"><span data-stu-id="8d928-143">List of existed **onPremisesAgent** objects.</span></span> <span data-ttu-id="8d928-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8d928-144">Read-only.</span></span> <span data-ttu-id="8d928-145">Anulável.</span><span class="sxs-lookup"><span data-stu-id="8d928-145">Nullable.</span></span>|
|<span data-ttu-id="8d928-146">publishedResources</span><span class="sxs-lookup"><span data-stu-id="8d928-146">publishedResources</span></span>|<span data-ttu-id="8d928-147">coleção [publishedResource](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="8d928-147">[publishedResource](publishedresource.md) collection</span></span>| <span data-ttu-id="8d928-148">Lista de objetos **publishedResource** existentes.</span><span class="sxs-lookup"><span data-stu-id="8d928-148">List of existing **publishedResource** objects.</span></span> <span data-ttu-id="8d928-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8d928-149">Read-only.</span></span> <span data-ttu-id="8d928-150">Anulável.</span><span class="sxs-lookup"><span data-stu-id="8d928-150">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d928-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8d928-151">JSON representation</span></span>

<span data-ttu-id="8d928-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8d928-152">The following is a JSON representation of the resource.</span></span>

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
