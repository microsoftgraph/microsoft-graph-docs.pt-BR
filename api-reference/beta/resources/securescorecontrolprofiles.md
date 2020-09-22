---
title: tipo de recurso secureScoreControlProfile
description: Representa a pontuação segura de um locatário por dados de controle. Por padrão, ele retorna todos os controles de um locatário e pode explicitamente extrair controles individuais.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: f4bcee22036cf344fec83be8ec08bba602e08c3e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087555"
---
# <a name="securescorecontrolprofile-resource-type"></a><span data-ttu-id="8c9f9-104">tipo de recurso secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="8c9f9-104">secureScoreControlProfile resource type</span></span>

<span data-ttu-id="8c9f9-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c9f9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c9f9-106">Representa a pontuação segura de um locatário por dados de controle.</span><span class="sxs-lookup"><span data-stu-id="8c9f9-106">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="8c9f9-107">Por padrão, ele retorna todos os controles de um locatário e pode explicitamente extrair controles individuais.</span><span class="sxs-lookup"><span data-stu-id="8c9f9-107">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="8c9f9-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="8c9f9-108">Methods</span></span>

| <span data-ttu-id="8c9f9-109">Método</span><span class="sxs-lookup"><span data-stu-id="8c9f9-109">Method</span></span>   | <span data-ttu-id="8c9f9-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8c9f9-110">Return Type</span></span>|<span data-ttu-id="8c9f9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c9f9-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8c9f9-112">Listar secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="8c9f9-112">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | <span data-ttu-id="8c9f9-113">coleção [secureScoreControlProfile](securescorecontrolprofiles.md)</span><span class="sxs-lookup"><span data-stu-id="8c9f9-113">[secureScoreControlProfile](securescorecontrolprofiles.md) collection</span></span> |<span data-ttu-id="8c9f9-114">Obtenha uma coleção de objetos secureScoreControlProfile.</span><span class="sxs-lookup"><span data-stu-id="8c9f9-114">Get a collection of secureScoreControlProfile objects.</span></span>|


## <a name="properties"></a><span data-ttu-id="8c9f9-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8c9f9-115">Properties</span></span>

|<span data-ttu-id="8c9f9-116">Nome</span><span class="sxs-lookup"><span data-stu-id="8c9f9-116">Name</span></span> |<span data-ttu-id="8c9f9-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c9f9-117">Type</span></span> |<span data-ttu-id="8c9f9-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c9f9-118">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="8c9f9-119">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="8c9f9-119">azureTenantId</span></span>   |   <span data-ttu-id="8c9f9-120">String</span><span class="sxs-lookup"><span data-stu-id="8c9f9-120">String</span></span>  |   <span data-ttu-id="8c9f9-121">Cadeia de caracteres GUID para ID do locatário.</span><span class="sxs-lookup"><span data-stu-id="8c9f9-121">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="8c9f9-122">controlName</span><span class="sxs-lookup"><span data-stu-id="8c9f9-122">controlName</span></span> |   <span data-ttu-id="8c9f9-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c9f9-123">String</span></span>  |   <span data-ttu-id="8c9f9-124">Nome do controle.</span><span class="sxs-lookup"><span data-stu-id="8c9f9-124">Name of the control.</span></span> |
|   <span data-ttu-id="8c9f9-125">title</span><span class="sxs-lookup"><span data-stu-id="8c9f9-125">title</span></span>   |   <span data-ttu-id="8c9f9-126">String</span><span class="sxs-lookup"><span data-stu-id="8c9f9-126">String</span></span>  |   <span data-ttu-id="8c9f9-127">Título do controle.</span><span class="sxs-lookup"><span data-stu-id="8c9f9-127">Title of the control.</span></span>   |
| <span data-ttu-id="8c9f9-128">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="8c9f9-128">complianceInformation</span></span> | <span data-ttu-id="8c9f9-129">coleção [complianceInformation](complianceinformation.md)</span><span class="sxs-lookup"><span data-stu-id="8c9f9-129">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="8c9f9-130">O conjunto de informações de conformidade associadas ao controle de Pontuação segura</span><span class="sxs-lookup"><span data-stu-id="8c9f9-130">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="8c9f9-131">controlCategory</span><span class="sxs-lookup"><span data-stu-id="8c9f9-131">controlCategory</span></span> |   <span data-ttu-id="8c9f9-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c9f9-132">String</span></span>  |   <span data-ttu-id="8c9f9-133">Categoria de ação de controle (conta, dados, dispositivo, aplicativos, infraestrutura).</span><span class="sxs-lookup"><span data-stu-id="8c9f9-133">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="8c9f9-134">actionType</span><span class="sxs-lookup"><span data-stu-id="8c9f9-134">actionType</span></span>  |   <span data-ttu-id="8c9f9-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c9f9-135">String</span></span>  |   <span data-ttu-id="8c9f9-136">Tipo de ação de controle (configuração, revisão, comportamento).</span><span class="sxs-lookup"><span data-stu-id="8c9f9-136">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="8c9f9-137">service</span><span class="sxs-lookup"><span data-stu-id="8c9f9-137">service</span></span> |   <span data-ttu-id="8c9f9-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c9f9-138">String</span></span>  |   <span data-ttu-id="8c9f9-139">Serviço que possui o controle (Exchange, SharePoint, Azure AD).</span><span class="sxs-lookup"><span data-stu-id="8c9f9-139">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="8c9f9-140">maxScore</span><span class="sxs-lookup"><span data-stu-id="8c9f9-140">maxScore</span></span> |  <span data-ttu-id="8c9f9-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c9f9-141">String</span></span>  |   <span data-ttu-id="8c9f9-142">A pontuação máxima obtida na data especificada.</span><span class="sxs-lookup"><span data-stu-id="8c9f9-142">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="8c9f9-143">camada</span><span class="sxs-lookup"><span data-stu-id="8c9f9-143">tier</span></span> |  <span data-ttu-id="8c9f9-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c9f9-144">String</span></span>  |   <span data-ttu-id="8c9f9-145">Camada de controle (Core, defesa profunda, avançada)</span><span class="sxs-lookup"><span data-stu-id="8c9f9-145">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="8c9f9-146">userimpact</span><span class="sxs-lookup"><span data-stu-id="8c9f9-146">userImpact</span></span> |    <span data-ttu-id="8c9f9-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c9f9-147">String</span></span>  | <span data-ttu-id="8c9f9-148">Impacto do usuário da implementação do controle (baixo, moderado, alto).</span><span class="sxs-lookup"><span data-stu-id="8c9f9-148">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="8c9f9-149">implementationCost</span><span class="sxs-lookup"><span data-stu-id="8c9f9-149">implementationCost</span></span> |    <span data-ttu-id="8c9f9-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c9f9-150">String</span></span>  |   <span data-ttu-id="8c9f9-151">Custo do recurso do controle implemmentating (baixo, moderado, alto).</span><span class="sxs-lookup"><span data-stu-id="8c9f9-151">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="8c9f9-152">classificação</span><span class="sxs-lookup"><span data-stu-id="8c9f9-152">rank</span></span> |  <span data-ttu-id="8c9f9-153">Int32</span><span class="sxs-lookup"><span data-stu-id="8c9f9-153">Int32</span></span>   |   <span data-ttu-id="8c9f9-154">Classificação de pilha da Microsoft de controle.</span><span class="sxs-lookup"><span data-stu-id="8c9f9-154">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="8c9f9-155">las</span><span class="sxs-lookup"><span data-stu-id="8c9f9-155">threats</span></span> |   <span data-ttu-id="8c9f9-156">String Collection</span><span class="sxs-lookup"><span data-stu-id="8c9f9-156">String Collection</span></span>   |   <span data-ttu-id="8c9f9-157">Lista de ameaças o controle atenua (accountBreach, dataexclusão, dataExfiltration, dataderramamento, elevationOfPrivilege, maliciousInsider, passwordCracking, phishingOrWhaling, falsificação).</span><span class="sxs-lookup"><span data-stu-id="8c9f9-157">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="8c9f9-158">preterido</span><span class="sxs-lookup"><span data-stu-id="8c9f9-158">deprecated</span></span> |    <span data-ttu-id="8c9f9-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c9f9-159">Boolean</span></span> |   <span data-ttu-id="8c9f9-160">Sinalizador para indicar se um controle está depreciado.</span><span class="sxs-lookup"><span data-stu-id="8c9f9-160">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="8c9f9-161">correção</span><span class="sxs-lookup"><span data-stu-id="8c9f9-161">remediation</span></span> |   <span data-ttu-id="8c9f9-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c9f9-162">String</span></span>  |   <span data-ttu-id="8c9f9-163">Descrição do que o controle ajudará a corrigir.</span><span class="sxs-lookup"><span data-stu-id="8c9f9-163">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="8c9f9-164">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="8c9f9-164">remediationImpact</span></span> | <span data-ttu-id="8c9f9-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c9f9-165">String</span></span>  |   <span data-ttu-id="8c9f9-166">Descrição do impacto sobre os usuários da correção.</span><span class="sxs-lookup"><span data-stu-id="8c9f9-166">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="8c9f9-167">actionUrl</span><span class="sxs-lookup"><span data-stu-id="8c9f9-167">actionUrl</span></span> | <span data-ttu-id="8c9f9-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c9f9-168">String</span></span>  |   <span data-ttu-id="8c9f9-169">URL para onde o controle pode ser acionado.</span><span class="sxs-lookup"><span data-stu-id="8c9f9-169">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="8c9f9-170">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="8c9f9-170">controlStateUpdates</span></span> | <span data-ttu-id="8c9f9-171">coleção [secureScoreControlStateUpdate](securescorecontrolstateupdate.md)</span><span class="sxs-lookup"><span data-stu-id="8c9f9-171">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection</span></span> |    <span data-ttu-id="8c9f9-172">Sinalizador para indicar onde o locatário marcou um controle (ignore, terceiros, revisado) (suporta [atualização](../api/securescorecontrolprofiles-update.md)).</span><span class="sxs-lookup"><span data-stu-id="8c9f9-172">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="8c9f9-173">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="8c9f9-173">vendorInformation</span></span> | [<span data-ttu-id="8c9f9-174">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="8c9f9-174">securityVendorInformation</span></span>](securityvendorinformation.md) |

## <a name="relationships"></a><span data-ttu-id="8c9f9-175">Relações</span><span class="sxs-lookup"><span data-stu-id="8c9f9-175">Relationships</span></span>

<span data-ttu-id="8c9f9-176">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8c9f9-176">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c9f9-177">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8c9f9-177">JSON representation</span></span>

<span data-ttu-id="8c9f9-178">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8c9f9-178">The following is a JSON representation of the resource.</span></span>

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


