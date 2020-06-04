---
title: tipo de recurso onPremisesPublishingProfile
description: tipo de recurso onPremisesPublishingProfile.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2b36f8307e580bc018a713822e4e9f2ea6f5586c
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556230"
---
# <a name="onpremisespublishingprofile-resource-type"></a><span data-ttu-id="eaa1d-103">tipo de recurso onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="eaa1d-103">onPremisesPublishingProfile resource type</span></span>

<span data-ttu-id="eaa1d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eaa1d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eaa1d-105">Vários serviços do Azure (por exemplo, a autenticação de [passagem](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta)do Azure Active Directory Connect, o [WORKDAY para o provisionamento de usuários do Azure ad](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)e o [proxy de aplicativo](https://aka.ms/whyappproxy) permitem o acesso a vários recursos locais de fora da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="eaa1d-105">Various Azure services (for example, Azure Active Directory Connect [Passthrough Authentication](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta), [Workday to Azure AD users provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial), and [Application Proxy](https://aka.ms/whyappproxy) allow access to various on-premises resources from outside the corporate network.</span></span>

<span data-ttu-id="eaa1d-106">[Os agentes locais](onpremisesagent.md) (ou [conectores](connector.md) para o proxy de aplicativo) instalados por um administrador podem ser configurados para encaminhar solicitações a um determinado [recurso publicado](publishedresource.md).</span><span class="sxs-lookup"><span data-stu-id="eaa1d-106">[On-premises agents](onpremisesagent.md) (or [connectors](connector.md) for Application Proxy) installed by an administrator can be configured to route requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="eaa1d-107">[Grupos de agente](onpremisesagentgroup.md) (ou [grupos de conectores](connectorgroup.md) para o proxy de aplicativo) permitem que um administrador atribua agentes específicos para atender a recursos locais publicados específicos.</span><span class="sxs-lookup"><span data-stu-id="eaa1d-107">[Agent groups](onpremisesagentgroup.md) (or [connector groups](connectorgroup.md) for Application Proxy) enable an administrator to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="eaa1d-108">Os administradores também podem agrupar vários agentes e, em seguida, atribuir cada recurso publicado a um grupo de agentes.</span><span class="sxs-lookup"><span data-stu-id="eaa1d-108">Administrators can also group multiple agents together, and then assign each published resource to an agent group.</span></span> <span data-ttu-id="eaa1d-109">Todo o conjunto de entidades do mesmo tipo de publicação local é representado pelo **onPremisesPublishingProfile**.</span><span class="sxs-lookup"><span data-stu-id="eaa1d-109">The entire set of entities of the same on-premises publishing type is represented by **onPremisesPublishingProfile**.</span></span>

## <a name="methods"></a><span data-ttu-id="eaa1d-110">Methods</span><span class="sxs-lookup"><span data-stu-id="eaa1d-110">Methods</span></span>

| <span data-ttu-id="eaa1d-111">Método</span><span class="sxs-lookup"><span data-stu-id="eaa1d-111">Method</span></span>       | <span data-ttu-id="eaa1d-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eaa1d-112">Return Type</span></span> | <span data-ttu-id="eaa1d-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaa1d-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="eaa1d-114">Obter onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="eaa1d-114">Get onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-get.md) | [<span data-ttu-id="eaa1d-115">onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="eaa1d-115">onPremisesPublishingProfile</span></span>](onpremisespublishingprofile.md) | <span data-ttu-id="eaa1d-116">Leia as propriedades e os relacionamentos de um objeto **onPremisesPublishingProfile** .</span><span class="sxs-lookup"><span data-stu-id="eaa1d-116">Read the properties and relationships of an **onPremisesPublishingProfile** object.</span></span> |
| [<span data-ttu-id="eaa1d-117">Atualizar onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="eaa1d-117">Update onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-update.md) | <span data-ttu-id="eaa1d-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="eaa1d-118">None</span></span> | <span data-ttu-id="eaa1d-119">Atualize um objeto [onPremisesPublishingProfile](onpremisespublishingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="eaa1d-119">Update an [onPremisesPublishingProfile](onpremisespublishingprofile.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="eaa1d-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eaa1d-120">Properties</span></span>

| <span data-ttu-id="eaa1d-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eaa1d-121">Property</span></span>     | <span data-ttu-id="eaa1d-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="eaa1d-122">Type</span></span>        | <span data-ttu-id="eaa1d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaa1d-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eaa1d-124">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="eaa1d-124">hybridAgentUpdaterConfiguration</span></span>|[<span data-ttu-id="eaa1d-125">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="eaa1d-125">hybridAgentUpdaterConfiguration</span></span>](hybridagentupdaterconfiguration.md)| <span data-ttu-id="eaa1d-126">Representa um objeto **hybridAgentUpdaterConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="eaa1d-126">Represents a **hybridAgentUpdaterConfiguration** object.</span></span>|
|<span data-ttu-id="eaa1d-127">id</span><span class="sxs-lookup"><span data-stu-id="eaa1d-127">id</span></span>|<span data-ttu-id="eaa1d-128">String</span><span class="sxs-lookup"><span data-stu-id="eaa1d-128">String</span></span>| <span data-ttu-id="eaa1d-129">Representa um tipo de publicação.</span><span class="sxs-lookup"><span data-stu-id="eaa1d-129">Represents a publishing type.</span></span> <span data-ttu-id="eaa1d-130">Os valores possíveis são: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="eaa1d-130">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span> <span data-ttu-id="eaa1d-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eaa1d-131">Read-only.</span></span>|
|<span data-ttu-id="eaa1d-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="eaa1d-132">isEnabled</span></span>|<span data-ttu-id="eaa1d-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="eaa1d-133">Boolean</span></span>| <span data-ttu-id="eaa1d-134">Representa se o [proxy de aplicativo do Azure ad](https://aka.ms/whyappproxy) está habilitado para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eaa1d-134">Represents if [Azure AD Application Proxy](https://aka.ms/whyappproxy) is enabled for the tenant.</span></span> |

## <a name="relationships"></a><span data-ttu-id="eaa1d-135">Relações</span><span class="sxs-lookup"><span data-stu-id="eaa1d-135">Relationships</span></span>

| <span data-ttu-id="eaa1d-136">Relação</span><span class="sxs-lookup"><span data-stu-id="eaa1d-136">Relationship</span></span> | <span data-ttu-id="eaa1d-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="eaa1d-137">Type</span></span>        | <span data-ttu-id="eaa1d-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaa1d-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eaa1d-139">agentGroups</span><span class="sxs-lookup"><span data-stu-id="eaa1d-139">agentGroups</span></span>|<span data-ttu-id="eaa1d-140">coleção [onPremisesAgentGroup](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="eaa1d-140">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="eaa1d-141">Lista de objetos **onPremisesAgentGroup** existentes.</span><span class="sxs-lookup"><span data-stu-id="eaa1d-141">List of existing **onPremisesAgentGroup** objects.</span></span> <span data-ttu-id="eaa1d-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eaa1d-142">Read-only.</span></span> <span data-ttu-id="eaa1d-143">Anulável.</span><span class="sxs-lookup"><span data-stu-id="eaa1d-143">Nullable.</span></span>|
|<span data-ttu-id="eaa1d-144">SNMP</span><span class="sxs-lookup"><span data-stu-id="eaa1d-144">agents</span></span>|<span data-ttu-id="eaa1d-145">coleção [onPremisesAgent](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="eaa1d-145">[onPremisesAgent](onpremisesagent.md) collection</span></span>| <span data-ttu-id="eaa1d-146">Lista de objetos **onPremisesAgent** existentes.</span><span class="sxs-lookup"><span data-stu-id="eaa1d-146">List of existing **onPremisesAgent** objects.</span></span> <span data-ttu-id="eaa1d-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eaa1d-147">Read-only.</span></span> <span data-ttu-id="eaa1d-148">Anulável.</span><span class="sxs-lookup"><span data-stu-id="eaa1d-148">Nullable.</span></span>|
|<span data-ttu-id="eaa1d-149">connectorGroups</span><span class="sxs-lookup"><span data-stu-id="eaa1d-149">connectorGroups</span></span>|<span data-ttu-id="eaa1d-150">coleção de [conectores](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="eaa1d-150">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="eaa1d-151">Lista de objetos de **conector** existentes para aplicativos publicados por meio do proxy de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="eaa1d-151">List of existing **connectorGroup** objects for applications published through Application Proxy.</span></span> <span data-ttu-id="eaa1d-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eaa1d-152">Read-only.</span></span> <span data-ttu-id="eaa1d-153">Anulável.</span><span class="sxs-lookup"><span data-stu-id="eaa1d-153">Nullable.</span></span>|
|<span data-ttu-id="eaa1d-154">conectores</span><span class="sxs-lookup"><span data-stu-id="eaa1d-154">connectors</span></span>|<span data-ttu-id="eaa1d-155">coleção [Connector](connector.md)</span><span class="sxs-lookup"><span data-stu-id="eaa1d-155">[connector](connector.md) collection</span></span>| <span data-ttu-id="eaa1d-156">Lista de objetos **conectores** existentes para aplicativos publicados por meio do proxy de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="eaa1d-156">List of existing **connector** objects for applications published through Application Proxy.</span></span> <span data-ttu-id="eaa1d-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eaa1d-157">Read-only.</span></span> <span data-ttu-id="eaa1d-158">Anulável.</span><span class="sxs-lookup"><span data-stu-id="eaa1d-158">Nullable.</span></span>|
|<span data-ttu-id="eaa1d-159">publishedResources</span><span class="sxs-lookup"><span data-stu-id="eaa1d-159">publishedResources</span></span>|<span data-ttu-id="eaa1d-160">coleção [publishedResource](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="eaa1d-160">[publishedResource](publishedresource.md) collection</span></span>| <span data-ttu-id="eaa1d-161">Lista de objetos **publishedResource** existentes.</span><span class="sxs-lookup"><span data-stu-id="eaa1d-161">List of existing **publishedResource** objects.</span></span> <span data-ttu-id="eaa1d-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eaa1d-162">Read-only.</span></span> <span data-ttu-id="eaa1d-163">Anulável.</span><span class="sxs-lookup"><span data-stu-id="eaa1d-163">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eaa1d-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eaa1d-164">JSON representation</span></span>

<span data-ttu-id="eaa1d-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eaa1d-165">The following is a JSON representation of the resource.</span></span>

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
