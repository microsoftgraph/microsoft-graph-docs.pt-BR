---
title: Tipo de recurso onPremisesPublishingProfile
description: Tipo de recurso onPremisesPublishingProfile.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 8e74374baa397c292d323dc0520833a7318cbe79
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134894"
---
# <a name="onpremisespublishingprofile-resource-type"></a><span data-ttu-id="b9d4e-103">Tipo de recurso onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="b9d4e-103">onPremisesPublishingProfile resource type</span></span>

<span data-ttu-id="b9d4e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9d4e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9d4e-105">Vários serviços do Azure (por exemplo, a Autenticação de Passagem do Azure Active Directory [Connect,](/azure/active-directory/hybrid/how-to-connect-pta)o dia de trabalho para o provisionamento de usuários do [Azure AD](/azure/active-directory/saas-apps/workday-inbound-tutorial)e o [Proxy](https://aka.ms/whyappproxy) de aplicativo permitem acesso a vários recursos locais de fora da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-105">Various Azure services (for example, Azure Active Directory Connect [Passthrough Authentication](/azure/active-directory/hybrid/how-to-connect-pta), [Workday to Azure AD users provisioning](/azure/active-directory/saas-apps/workday-inbound-tutorial), and [Application Proxy](https://aka.ms/whyappproxy) allow access to various on-premises resources from outside the corporate network.</span></span>

<span data-ttu-id="b9d4e-106">[Agentes locais (ou](onpremisesagent.md) conectores para Proxy de Aplicativo) instalados por um administrador podem ser [configurados](connector.md) para encaminhar solicitações para um recurso [publicado específico.](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="b9d4e-106">[On-premises agents](onpremisesagent.md) (or [connectors](connector.md) for Application Proxy) installed by an administrator can be configured to route requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="b9d4e-107">[Grupos de agentes](onpremisesagentgroup.md) (ou [grupos de conectores](connectorgroup.md) para Proxy de Aplicativo) permitem que um administrador atribua agentes específicos para atender a recursos locais publicados específicos.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-107">[Agent groups](onpremisesagentgroup.md) (or [connector groups](connectorgroup.md) for Application Proxy) enable an administrator to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="b9d4e-108">Os administradores também podem agrupar vários agentes e atribuir cada recurso publicado a um grupo de agentes.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-108">Administrators can also group multiple agents together, and then assign each published resource to an agent group.</span></span> <span data-ttu-id="b9d4e-109">Todo o conjunto de entidades do mesmo tipo de publicação local é representado por **onPremisesPublishingProfile**.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-109">The entire set of entities of the same on-premises publishing type is represented by **onPremisesPublishingProfile**.</span></span>

## <a name="methods"></a><span data-ttu-id="b9d4e-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="b9d4e-110">Methods</span></span>

| <span data-ttu-id="b9d4e-111">Método</span><span class="sxs-lookup"><span data-stu-id="b9d4e-111">Method</span></span>       | <span data-ttu-id="b9d4e-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b9d4e-112">Return Type</span></span> | <span data-ttu-id="b9d4e-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9d4e-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b9d4e-114">Obter onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="b9d4e-114">Get onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-get.md) | [<span data-ttu-id="b9d4e-115">onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="b9d4e-115">onPremisesPublishingProfile</span></span>](onpremisespublishingprofile.md) | <span data-ttu-id="b9d4e-116">Leia as propriedades e os relacionamentos de um **objeto onPremisesPublishingProfile.**</span><span class="sxs-lookup"><span data-stu-id="b9d4e-116">Read the properties and relationships of an **onPremisesPublishingProfile** object.</span></span> |
| [<span data-ttu-id="b9d4e-117">Atualizar onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="b9d4e-117">Update onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-update.md) | <span data-ttu-id="b9d4e-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b9d4e-118">None</span></span> | <span data-ttu-id="b9d4e-119">Atualize [um objeto onPremisesPublishingProfile.](onpremisespublishingprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b9d4e-119">Update an [onPremisesPublishingProfile](onpremisespublishingprofile.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b9d4e-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9d4e-120">Properties</span></span>

| <span data-ttu-id="b9d4e-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9d4e-121">Property</span></span>     | <span data-ttu-id="b9d4e-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9d4e-122">Type</span></span>        | <span data-ttu-id="b9d4e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9d4e-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b9d4e-124">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="b9d4e-124">hybridAgentUpdaterConfiguration</span></span>|[<span data-ttu-id="b9d4e-125">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="b9d4e-125">hybridAgentUpdaterConfiguration</span></span>](hybridagentupdaterconfiguration.md)| <span data-ttu-id="b9d4e-126">Representa um **objeto hybridAgentUpdaterConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="b9d4e-126">Represents a **hybridAgentUpdaterConfiguration** object.</span></span>|
|<span data-ttu-id="b9d4e-127">id</span><span class="sxs-lookup"><span data-stu-id="b9d4e-127">id</span></span>|<span data-ttu-id="b9d4e-128">String</span><span class="sxs-lookup"><span data-stu-id="b9d4e-128">String</span></span>| <span data-ttu-id="b9d4e-129">Representa um tipo de publicação.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-129">Represents a publishing type.</span></span> <span data-ttu-id="b9d4e-130">Os valores possíveis são: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-130">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span> <span data-ttu-id="b9d4e-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-131">Read-only.</span></span>|
|<span data-ttu-id="b9d4e-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="b9d4e-132">isEnabled</span></span>|<span data-ttu-id="b9d4e-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="b9d4e-133">Boolean</span></span>| <span data-ttu-id="b9d4e-134">Representa se o [Proxy de Aplicativo do Azure AD](https://aka.ms/whyappproxy) está habilitado para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-134">Represents if [Azure AD Application Proxy](https://aka.ms/whyappproxy) is enabled for the tenant.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b9d4e-135">Relações</span><span class="sxs-lookup"><span data-stu-id="b9d4e-135">Relationships</span></span>

| <span data-ttu-id="b9d4e-136">Relação</span><span class="sxs-lookup"><span data-stu-id="b9d4e-136">Relationship</span></span> | <span data-ttu-id="b9d4e-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9d4e-137">Type</span></span>        | <span data-ttu-id="b9d4e-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9d4e-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b9d4e-139">agentGroups</span><span class="sxs-lookup"><span data-stu-id="b9d4e-139">agentGroups</span></span>|<span data-ttu-id="b9d4e-140">[Coleção onPremisesAgentGroup](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="b9d4e-140">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="b9d4e-141">Lista de objetos **onPremisesAgentGroup** existentes.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-141">List of existing **onPremisesAgentGroup** objects.</span></span> <span data-ttu-id="b9d4e-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-142">Read-only.</span></span> <span data-ttu-id="b9d4e-143">Anulável.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-143">Nullable.</span></span>|
|<span data-ttu-id="b9d4e-144">agentes</span><span class="sxs-lookup"><span data-stu-id="b9d4e-144">agents</span></span>|<span data-ttu-id="b9d4e-145">[Coleção onPremisesAgent](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="b9d4e-145">[onPremisesAgent](onpremisesagent.md) collection</span></span>| <span data-ttu-id="b9d4e-146">Lista de objetos **onPremisesAgent** existentes.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-146">List of existing **onPremisesAgent** objects.</span></span> <span data-ttu-id="b9d4e-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-147">Read-only.</span></span> <span data-ttu-id="b9d4e-148">Anulável.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-148">Nullable.</span></span>|
|<span data-ttu-id="b9d4e-149">connectorGroups</span><span class="sxs-lookup"><span data-stu-id="b9d4e-149">connectorGroups</span></span>|<span data-ttu-id="b9d4e-150">[Coleção connectorGroup](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="b9d4e-150">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="b9d4e-151">Lista de objetos **connectorGroup existentes** para aplicativos publicados por meio do Proxy de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-151">List of existing **connectorGroup** objects for applications published through Application Proxy.</span></span> <span data-ttu-id="b9d4e-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-152">Read-only.</span></span> <span data-ttu-id="b9d4e-153">Anulável.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-153">Nullable.</span></span>|
|<span data-ttu-id="b9d4e-154">conectores</span><span class="sxs-lookup"><span data-stu-id="b9d4e-154">connectors</span></span>|<span data-ttu-id="b9d4e-155">[conjunto de conectores](connector.md)</span><span class="sxs-lookup"><span data-stu-id="b9d4e-155">[connector](connector.md) collection</span></span>| <span data-ttu-id="b9d4e-156">Lista de objetos de **conector existentes** para aplicativos publicados por meio do Proxy de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-156">List of existing **connector** objects for applications published through Application Proxy.</span></span> <span data-ttu-id="b9d4e-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-157">Read-only.</span></span> <span data-ttu-id="b9d4e-158">Anulável.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-158">Nullable.</span></span>|
|<span data-ttu-id="b9d4e-159">publishedResources</span><span class="sxs-lookup"><span data-stu-id="b9d4e-159">publishedResources</span></span>|<span data-ttu-id="b9d4e-160">[Coleção publishedResource](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="b9d4e-160">[publishedResource](publishedresource.md) collection</span></span>| <span data-ttu-id="b9d4e-161">Lista de objetos **publishedResource** existentes.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-161">List of existing **publishedResource** objects.</span></span> <span data-ttu-id="b9d4e-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-162">Read-only.</span></span> <span data-ttu-id="b9d4e-163">Anulável.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-163">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b9d4e-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9d4e-164">JSON representation</span></span>

<span data-ttu-id="b9d4e-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-165">The following is a JSON representation of the resource.</span></span>

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



