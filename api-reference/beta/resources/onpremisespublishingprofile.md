---
title: Tipo de recurso onPremisesPublishingProfile
description: Tipo de recurso onPremisesPublishingProfile.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: a7dc65f0640d2bfde9a46595b04fc24fc7512475
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156704"
---
# <a name="onpremisespublishingprofile-resource-type"></a><span data-ttu-id="9fa92-103">Tipo de recurso onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="9fa92-103">onPremisesPublishingProfile resource type</span></span>

<span data-ttu-id="9fa92-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fa92-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fa92-105">Vários serviços do Azure (por exemplo, a Autenticação de Passagem do Azure Active Directory [Connect,](/azure/active-directory/hybrid/how-to-connect-pta)o dia de trabalho para o provisionamento de usuários do [Azure AD](/azure/active-directory/saas-apps/workday-inbound-tutorial)e o [Proxy](https://aka.ms/whyappproxy) de aplicativo permitem acesso a vários recursos locais de fora da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="9fa92-105">Various Azure services (for example, Azure Active Directory Connect [Passthrough Authentication](/azure/active-directory/hybrid/how-to-connect-pta), [Workday to Azure AD users provisioning](/azure/active-directory/saas-apps/workday-inbound-tutorial), and [Application Proxy](https://aka.ms/whyappproxy) allow access to various on-premises resources from outside the corporate network.</span></span>

<span data-ttu-id="9fa92-106">[Agentes locais (ou](onpremisesagent.md) conectores para Proxy de Aplicativo) instalados por um administrador podem ser [configurados](connector.md) para encaminhar solicitações para um recurso [publicado específico.](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="9fa92-106">[On-premises agents](onpremisesagent.md) (or [connectors](connector.md) for Application Proxy) installed by an administrator can be configured to route requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="9fa92-107">[Grupos de agentes](onpremisesagentgroup.md) (ou [grupos de conectores](connectorgroup.md) para Proxy de Aplicativo) permitem que um administrador atribua agentes específicos para atender a recursos locais publicados específicos.</span><span class="sxs-lookup"><span data-stu-id="9fa92-107">[Agent groups](onpremisesagentgroup.md) (or [connector groups](connectorgroup.md) for Application Proxy) enable an administrator to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="9fa92-108">Os administradores também podem agrupar vários agentes e atribuir cada recurso publicado a um grupo de agentes.</span><span class="sxs-lookup"><span data-stu-id="9fa92-108">Administrators can also group multiple agents together, and then assign each published resource to an agent group.</span></span> <span data-ttu-id="9fa92-109">Todo o conjunto de entidades do mesmo tipo de publicação local é representado por **onPremisesPublishingProfile**.</span><span class="sxs-lookup"><span data-stu-id="9fa92-109">The entire set of entities of the same on-premises publishing type is represented by **onPremisesPublishingProfile**.</span></span>

## <a name="methods"></a><span data-ttu-id="9fa92-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="9fa92-110">Methods</span></span>

| <span data-ttu-id="9fa92-111">Método</span><span class="sxs-lookup"><span data-stu-id="9fa92-111">Method</span></span>       | <span data-ttu-id="9fa92-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9fa92-112">Return Type</span></span> | <span data-ttu-id="9fa92-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fa92-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9fa92-114">Obter onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="9fa92-114">Get onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-get.md) | [<span data-ttu-id="9fa92-115">onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="9fa92-115">onPremisesPublishingProfile</span></span>](onpremisespublishingprofile.md) | <span data-ttu-id="9fa92-116">Leia as propriedades e os relacionamentos de um **objeto onPremisesPublishingProfile.**</span><span class="sxs-lookup"><span data-stu-id="9fa92-116">Read the properties and relationships of an **onPremisesPublishingProfile** object.</span></span> |
| [<span data-ttu-id="9fa92-117">Atualizar onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="9fa92-117">Update onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-update.md) | <span data-ttu-id="9fa92-118">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="9fa92-118">None</span></span> | <span data-ttu-id="9fa92-119">Atualize [um objeto onPremisesPublishingProfile.](onpremisespublishingprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9fa92-119">Update an [onPremisesPublishingProfile](onpremisespublishingprofile.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9fa92-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9fa92-120">Properties</span></span>

| <span data-ttu-id="9fa92-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9fa92-121">Property</span></span>     | <span data-ttu-id="9fa92-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fa92-122">Type</span></span>        | <span data-ttu-id="9fa92-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fa92-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9fa92-124">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="9fa92-124">hybridAgentUpdaterConfiguration</span></span>|[<span data-ttu-id="9fa92-125">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="9fa92-125">hybridAgentUpdaterConfiguration</span></span>](hybridagentupdaterconfiguration.md)| <span data-ttu-id="9fa92-126">Representa um **objeto hybridAgentUpdaterConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="9fa92-126">Represents a **hybridAgentUpdaterConfiguration** object.</span></span>|
|<span data-ttu-id="9fa92-127">id</span><span class="sxs-lookup"><span data-stu-id="9fa92-127">id</span></span>|<span data-ttu-id="9fa92-128">String</span><span class="sxs-lookup"><span data-stu-id="9fa92-128">String</span></span>| <span data-ttu-id="9fa92-129">Representa um tipo de publicação.</span><span class="sxs-lookup"><span data-stu-id="9fa92-129">Represents a publishing type.</span></span> <span data-ttu-id="9fa92-130">Os valores possíveis são: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="9fa92-130">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span> <span data-ttu-id="9fa92-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9fa92-131">Read-only.</span></span>|
|<span data-ttu-id="9fa92-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="9fa92-132">isEnabled</span></span>|<span data-ttu-id="9fa92-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="9fa92-133">Boolean</span></span>| <span data-ttu-id="9fa92-134">Representa se o [Proxy de Aplicativo do Azure AD](https://aka.ms/whyappproxy) está habilitado para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9fa92-134">Represents if [Azure AD Application Proxy](https://aka.ms/whyappproxy) is enabled for the tenant.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9fa92-135">Relações</span><span class="sxs-lookup"><span data-stu-id="9fa92-135">Relationships</span></span>

| <span data-ttu-id="9fa92-136">Relação</span><span class="sxs-lookup"><span data-stu-id="9fa92-136">Relationship</span></span> | <span data-ttu-id="9fa92-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fa92-137">Type</span></span>        | <span data-ttu-id="9fa92-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fa92-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9fa92-139">agentGroups</span><span class="sxs-lookup"><span data-stu-id="9fa92-139">agentGroups</span></span>|<span data-ttu-id="9fa92-140">[Coleção onPremisesAgentGroup](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="9fa92-140">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="9fa92-141">Lista de objetos **onPremisesAgentGroup** existentes.</span><span class="sxs-lookup"><span data-stu-id="9fa92-141">List of existing **onPremisesAgentGroup** objects.</span></span> <span data-ttu-id="9fa92-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9fa92-142">Read-only.</span></span> <span data-ttu-id="9fa92-143">Anulável.</span><span class="sxs-lookup"><span data-stu-id="9fa92-143">Nullable.</span></span>|
|<span data-ttu-id="9fa92-144">agentes</span><span class="sxs-lookup"><span data-stu-id="9fa92-144">agents</span></span>|<span data-ttu-id="9fa92-145">[Coleção onPremisesAgent](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="9fa92-145">[onPremisesAgent](onpremisesagent.md) collection</span></span>| <span data-ttu-id="9fa92-146">Lista de objetos **onPremisesAgent** existentes.</span><span class="sxs-lookup"><span data-stu-id="9fa92-146">List of existing **onPremisesAgent** objects.</span></span> <span data-ttu-id="9fa92-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9fa92-147">Read-only.</span></span> <span data-ttu-id="9fa92-148">Anulável.</span><span class="sxs-lookup"><span data-stu-id="9fa92-148">Nullable.</span></span>|
|<span data-ttu-id="9fa92-149">connectorGroups</span><span class="sxs-lookup"><span data-stu-id="9fa92-149">connectorGroups</span></span>|<span data-ttu-id="9fa92-150">[Coleção connectorGroup](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="9fa92-150">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="9fa92-151">Lista de objetos **connectorGroup existentes** para aplicativos publicados por meio do Proxy de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9fa92-151">List of existing **connectorGroup** objects for applications published through Application Proxy.</span></span> <span data-ttu-id="9fa92-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9fa92-152">Read-only.</span></span> <span data-ttu-id="9fa92-153">Anulável.</span><span class="sxs-lookup"><span data-stu-id="9fa92-153">Nullable.</span></span>|
|<span data-ttu-id="9fa92-154">conectores</span><span class="sxs-lookup"><span data-stu-id="9fa92-154">connectors</span></span>|<span data-ttu-id="9fa92-155">[conjunto de conectores](connector.md)</span><span class="sxs-lookup"><span data-stu-id="9fa92-155">[connector](connector.md) collection</span></span>| <span data-ttu-id="9fa92-156">Lista de objetos de **conector existentes** para aplicativos publicados por meio do Proxy de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9fa92-156">List of existing **connector** objects for applications published through Application Proxy.</span></span> <span data-ttu-id="9fa92-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9fa92-157">Read-only.</span></span> <span data-ttu-id="9fa92-158">Anulável.</span><span class="sxs-lookup"><span data-stu-id="9fa92-158">Nullable.</span></span>|
|<span data-ttu-id="9fa92-159">publishedResources</span><span class="sxs-lookup"><span data-stu-id="9fa92-159">publishedResources</span></span>|<span data-ttu-id="9fa92-160">[Coleção publishedResource](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="9fa92-160">[publishedResource](publishedresource.md) collection</span></span>| <span data-ttu-id="9fa92-161">Lista de objetos **publishedResource** existentes.</span><span class="sxs-lookup"><span data-stu-id="9fa92-161">List of existing **publishedResource** objects.</span></span> <span data-ttu-id="9fa92-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9fa92-162">Read-only.</span></span> <span data-ttu-id="9fa92-163">Anulável.</span><span class="sxs-lookup"><span data-stu-id="9fa92-163">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9fa92-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9fa92-164">JSON representation</span></span>

<span data-ttu-id="9fa92-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9fa92-165">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile",
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



