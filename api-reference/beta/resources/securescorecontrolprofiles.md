---
title: tipo de recurso secureScoreControlProfile
description: Representa a pontuação segura de um locatário por dados de controle. Por padrão, ele retorna todos os controles de um locatário e pode explicitamente extrair controles individuais.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5e244576cb014719d454fe37bd8395054efe2e2b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965273"
---
# <a name="securescorecontrolprofile-resource-type"></a><span data-ttu-id="413c8-104">tipo de recurso secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="413c8-104">secureScoreControlProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="413c8-105">Representa a pontuação segura de um locatário por dados de controle.</span><span class="sxs-lookup"><span data-stu-id="413c8-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="413c8-106">Por padrão, ele retorna todos os controles de um locatário e pode explicitamente extrair controles individuais.</span><span class="sxs-lookup"><span data-stu-id="413c8-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="413c8-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="413c8-107">Methods</span></span>

| <span data-ttu-id="413c8-108">Método</span><span class="sxs-lookup"><span data-stu-id="413c8-108">Method</span></span>   | <span data-ttu-id="413c8-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="413c8-109">Return Type</span></span>|<span data-ttu-id="413c8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="413c8-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="413c8-111">Lista secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="413c8-111">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | <span data-ttu-id="413c8-112">coleção [secureScoreControlProfile](securescorecontrolprofiles.md)</span><span class="sxs-lookup"><span data-stu-id="413c8-112">[secureScoreControlProfile](securescorecontrolprofiles.md) collection</span></span> |<span data-ttu-id="413c8-113">Obtenha uma coleção de objetos secureScoreControlProfile.</span><span class="sxs-lookup"><span data-stu-id="413c8-113">Get a collection of secureScoreControlProfile objects.</span></span>|


## <a name="properties"></a><span data-ttu-id="413c8-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="413c8-114">Properties</span></span>

|<span data-ttu-id="413c8-115">Nome</span><span class="sxs-lookup"><span data-stu-id="413c8-115">Name</span></span> |<span data-ttu-id="413c8-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="413c8-116">Type</span></span> |<span data-ttu-id="413c8-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="413c8-117">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="413c8-118">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="413c8-118">azureTenantId</span></span>   |   <span data-ttu-id="413c8-119">String</span><span class="sxs-lookup"><span data-stu-id="413c8-119">String</span></span>  |   <span data-ttu-id="413c8-120">Cadeia de caracteres GUID para ID do locatário.</span><span class="sxs-lookup"><span data-stu-id="413c8-120">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="413c8-121">controlName</span><span class="sxs-lookup"><span data-stu-id="413c8-121">controlName</span></span> |   <span data-ttu-id="413c8-122">String</span><span class="sxs-lookup"><span data-stu-id="413c8-122">String</span></span>  |   <span data-ttu-id="413c8-123">Nome do controle.</span><span class="sxs-lookup"><span data-stu-id="413c8-123">Name of the control.</span></span> |
|   <span data-ttu-id="413c8-124">title</span><span class="sxs-lookup"><span data-stu-id="413c8-124">title</span></span>   |   <span data-ttu-id="413c8-125">String</span><span class="sxs-lookup"><span data-stu-id="413c8-125">String</span></span>  |   <span data-ttu-id="413c8-126">Título do controle.</span><span class="sxs-lookup"><span data-stu-id="413c8-126">Title of the control.</span></span>   |
| <span data-ttu-id="413c8-127">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="413c8-127">complianceInformation</span></span> | <span data-ttu-id="413c8-128">coleção [complianceInformation](complianceinformation.md)</span><span class="sxs-lookup"><span data-stu-id="413c8-128">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="413c8-129">O conjunto de informações de conformidade associadas ao controle de Pontuação segura</span><span class="sxs-lookup"><span data-stu-id="413c8-129">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="413c8-130">controlCategory</span><span class="sxs-lookup"><span data-stu-id="413c8-130">controlCategory</span></span> |   <span data-ttu-id="413c8-131">String</span><span class="sxs-lookup"><span data-stu-id="413c8-131">String</span></span>  |   <span data-ttu-id="413c8-132">Categoria de ação de controle (conta, dados, dispositivo, aplicativos, infraestrutura).</span><span class="sxs-lookup"><span data-stu-id="413c8-132">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="413c8-133">actionType</span><span class="sxs-lookup"><span data-stu-id="413c8-133">actionType</span></span>  |   <span data-ttu-id="413c8-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="413c8-134">String</span></span>  |   <span data-ttu-id="413c8-135">Tipo de ação de controle (configuração, revisão, comportamento).</span><span class="sxs-lookup"><span data-stu-id="413c8-135">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="413c8-136">service</span><span class="sxs-lookup"><span data-stu-id="413c8-136">service</span></span> |   <span data-ttu-id="413c8-137">String</span><span class="sxs-lookup"><span data-stu-id="413c8-137">String</span></span>  |   <span data-ttu-id="413c8-138">Serviço que possui o controle (Exchange, SharePoint, Azure AD).</span><span class="sxs-lookup"><span data-stu-id="413c8-138">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="413c8-139">maxScore</span><span class="sxs-lookup"><span data-stu-id="413c8-139">maxScore</span></span> |  <span data-ttu-id="413c8-140">String</span><span class="sxs-lookup"><span data-stu-id="413c8-140">String</span></span>  |   <span data-ttu-id="413c8-141">A pontuação máxima obtida na data especificada.</span><span class="sxs-lookup"><span data-stu-id="413c8-141">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="413c8-142">camada</span><span class="sxs-lookup"><span data-stu-id="413c8-142">tier</span></span> |  <span data-ttu-id="413c8-143">String</span><span class="sxs-lookup"><span data-stu-id="413c8-143">String</span></span>  |   <span data-ttu-id="413c8-144">Camada de controle (Core, defesa profunda, avançada)</span><span class="sxs-lookup"><span data-stu-id="413c8-144">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="413c8-145">userimpact</span><span class="sxs-lookup"><span data-stu-id="413c8-145">userImpact</span></span> |    <span data-ttu-id="413c8-146">String</span><span class="sxs-lookup"><span data-stu-id="413c8-146">String</span></span>  | <span data-ttu-id="413c8-147">Impacto do usuário da implementação do controle (baixo, moderado, alto).</span><span class="sxs-lookup"><span data-stu-id="413c8-147">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="413c8-148">implementationCost</span><span class="sxs-lookup"><span data-stu-id="413c8-148">implementationCost</span></span> |    <span data-ttu-id="413c8-149">String</span><span class="sxs-lookup"><span data-stu-id="413c8-149">String</span></span>  |   <span data-ttu-id="413c8-150">Custo do recurso do controle implemmentating (baixo, moderado, alto).</span><span class="sxs-lookup"><span data-stu-id="413c8-150">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="413c8-151">classificação</span><span class="sxs-lookup"><span data-stu-id="413c8-151">rank</span></span> |  <span data-ttu-id="413c8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="413c8-152">Int32</span></span>   |   <span data-ttu-id="413c8-153">Classificação de pilha da Microsoft de controle.</span><span class="sxs-lookup"><span data-stu-id="413c8-153">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="413c8-154">las</span><span class="sxs-lookup"><span data-stu-id="413c8-154">threats</span></span> |   <span data-ttu-id="413c8-155">String Collection</span><span class="sxs-lookup"><span data-stu-id="413c8-155">String Collection</span></span>   |   <span data-ttu-id="413c8-156">Lista de ameaças o controle atenua (accountBreach, dataexclusão, dataExfiltration, dataderramamento, elevationOfPrivilege, maliciousInsider, passwordCracking, phishingOrWhaling, falsificação).</span><span class="sxs-lookup"><span data-stu-id="413c8-156">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="413c8-157">preterido</span><span class="sxs-lookup"><span data-stu-id="413c8-157">deprecated</span></span> |    <span data-ttu-id="413c8-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="413c8-158">Boolean</span></span> |   <span data-ttu-id="413c8-159">Sinalizador para indicar se um controle está depreciado.</span><span class="sxs-lookup"><span data-stu-id="413c8-159">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="413c8-160">correção</span><span class="sxs-lookup"><span data-stu-id="413c8-160">remediation</span></span> |   <span data-ttu-id="413c8-161">String</span><span class="sxs-lookup"><span data-stu-id="413c8-161">String</span></span>  |   <span data-ttu-id="413c8-162">Descrição do que o controle ajudará a corrigir.</span><span class="sxs-lookup"><span data-stu-id="413c8-162">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="413c8-163">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="413c8-163">remediationImpact</span></span> | <span data-ttu-id="413c8-164">String</span><span class="sxs-lookup"><span data-stu-id="413c8-164">String</span></span>  |   <span data-ttu-id="413c8-165">Descrição do impacto sobre os usuários da correção.</span><span class="sxs-lookup"><span data-stu-id="413c8-165">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="413c8-166">actionUrl</span><span class="sxs-lookup"><span data-stu-id="413c8-166">actionUrl</span></span> | <span data-ttu-id="413c8-167">String</span><span class="sxs-lookup"><span data-stu-id="413c8-167">String</span></span>  |   <span data-ttu-id="413c8-168">URL para onde o controle pode ser acionado.</span><span class="sxs-lookup"><span data-stu-id="413c8-168">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="413c8-169">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="413c8-169">controlStateUpdates</span></span> | <span data-ttu-id="413c8-170">coleção [secureScoreControlStateUpdate](securescorecontrolstateupdate.md)</span><span class="sxs-lookup"><span data-stu-id="413c8-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection</span></span> |    <span data-ttu-id="413c8-171">Sinalizador para indicar onde o locatário marcou um controle (ignore, terceiros, revisado) (suporta [atualização](../api/securescorecontrolprofiles-update.md)).</span><span class="sxs-lookup"><span data-stu-id="413c8-171">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="413c8-172">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="413c8-172">vendorInformation</span></span> | [<span data-ttu-id="413c8-173">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="413c8-173">securityVendorInformation</span></span>](securityvendorinformation.md) |

## <a name="relationships"></a><span data-ttu-id="413c8-174">Relações</span><span class="sxs-lookup"><span data-stu-id="413c8-174">Relationships</span></span>

<span data-ttu-id="413c8-175">Nenhum</span><span class="sxs-lookup"><span data-stu-id="413c8-175">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="413c8-176">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="413c8-176">JSON representation</span></span>

<span data-ttu-id="413c8-177">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="413c8-177">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
}-->

```json
{
  "title": "String",
  "azureTenantId": "String (identifier)",
  "maxScore": 1024.13,
  "actionType": "String",
  "service": "String",
  "tier": "String",
  "userImpact": "string",
  "implementationCost ": "String",
  "rank ": 100,
  "threats": ["string"],
  "deprecated ": false,
  "remediation": "String",
  "remediationImpact ": "String",
  "actionUrl": "String",
  "controlStateUpdates": [{"@odata.type": "microsoft.graph.secureScoreControlStateUpdate"}],
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
  "complianceInformation": [{"@odata.type": "microsoft.graph.complianceInformation"}],
  "controlCategory": "string",
  "lastModifiedDateTime": "String (timestamp)"
}


```


<!--
{
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
