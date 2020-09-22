---
title: tipo de recurso secureScoreControlProfile
description: Representa a pontuação segura de um locatário por dados de controle. Por padrão, ele retorna todos os controles de um locatário e pode explicitamente extrair controles individuais.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c7af5b2ab614dae57ef7c18aee80133cd7a2096a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984065"
---
# <a name="securescorecontrolprofile-resource-type"></a><span data-ttu-id="625c3-104">tipo de recurso secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="625c3-104">secureScoreControlProfile resource type</span></span>

<span data-ttu-id="625c3-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="625c3-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="625c3-106">Representa a pontuação segura de um locatário por dados de controle.</span><span class="sxs-lookup"><span data-stu-id="625c3-106">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="625c3-107">Por padrão, ele retorna todos os controles de um locatário e pode explicitamente extrair controles individuais.</span><span class="sxs-lookup"><span data-stu-id="625c3-107">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="625c3-108">Methods</span><span class="sxs-lookup"><span data-stu-id="625c3-108">Methods</span></span>

| <span data-ttu-id="625c3-109">Método</span><span class="sxs-lookup"><span data-stu-id="625c3-109">Method</span></span>   | <span data-ttu-id="625c3-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="625c3-110">Return Type</span></span>|<span data-ttu-id="625c3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="625c3-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="625c3-112">Lista secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="625c3-112">List secureScoreControlProfiles</span></span>](../api/security-list-securescorecontrolprofiles.md) | [<span data-ttu-id="625c3-113">secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="625c3-113">secureScoreControlProfile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="625c3-114">Leia as propriedades e os metadados de um objeto secureScoreControlProfiles.</span><span class="sxs-lookup"><span data-stu-id="625c3-114">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|
|[<span data-ttu-id="625c3-115">Obter secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="625c3-115">Get secureScoreControlProfile</span></span>](../api/securescorecontrolprofile-get.md) | [<span data-ttu-id="625c3-116">securescorecontrolprofile</span><span class="sxs-lookup"><span data-stu-id="625c3-116">securescorecontrolprofile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="625c3-117">Leia as propriedades e os metadados de um objeto secureScoreControlProfiles.</span><span class="sxs-lookup"><span data-stu-id="625c3-117">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|
|[<span data-ttu-id="625c3-118">Atualizar securescorecontrolprofile</span><span class="sxs-lookup"><span data-stu-id="625c3-118">Update securescorecontrolprofile</span></span>](../api/securescorecontrolprofile-update.md) | [<span data-ttu-id="625c3-119">securescorecontrolprofile</span><span class="sxs-lookup"><span data-stu-id="625c3-119">securescorecontrolprofile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="625c3-120">Atualize um objeto securescorecontrolprofile.</span><span class="sxs-lookup"><span data-stu-id="625c3-120">Update an securescorecontrolprofile object.</span></span> |


## <a name="properties"></a><span data-ttu-id="625c3-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="625c3-121">Properties</span></span>

|<span data-ttu-id="625c3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="625c3-122">Name</span></span> |<span data-ttu-id="625c3-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="625c3-123">Type</span></span> |<span data-ttu-id="625c3-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="625c3-124">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="625c3-125">id</span><span class="sxs-lookup"><span data-stu-id="625c3-125">id</span></span>|<span data-ttu-id="625c3-126">String</span><span class="sxs-lookup"><span data-stu-id="625c3-126">String</span></span>|<span data-ttu-id="625c3-127">Identificador GUID/exclusivo gerado pelo provedor.</span><span class="sxs-lookup"><span data-stu-id="625c3-127">Provider-generated GUID/unique identifier.</span></span> <span data-ttu-id="625c3-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="625c3-128">Read-only.</span></span> <span data-ttu-id="625c3-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="625c3-129">Required.</span></span>|
|<span data-ttu-id="625c3-130">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="625c3-130">azureTenantId</span></span>|<span data-ttu-id="625c3-131">String</span><span class="sxs-lookup"><span data-stu-id="625c3-131">String</span></span>|<span data-ttu-id="625c3-132">Cadeia de caracteres GUID para ID do locatário.</span><span class="sxs-lookup"><span data-stu-id="625c3-132">GUID string for tenant ID.</span></span>|
|<span data-ttu-id="625c3-133">actionType</span><span class="sxs-lookup"><span data-stu-id="625c3-133">actionType</span></span>|<span data-ttu-id="625c3-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="625c3-134">String</span></span>|<span data-ttu-id="625c3-135">Tipo de ação de controle (configuração, revisão, comportamento).</span><span class="sxs-lookup"><span data-stu-id="625c3-135">Control action type (Config, Review, Behavior).</span></span>|
|<span data-ttu-id="625c3-136">actionUrl</span><span class="sxs-lookup"><span data-stu-id="625c3-136">actionUrl</span></span>|<span data-ttu-id="625c3-137">String</span><span class="sxs-lookup"><span data-stu-id="625c3-137">String</span></span>|<span data-ttu-id="625c3-138">URL para onde o controle pode ser acionado.</span><span class="sxs-lookup"><span data-stu-id="625c3-138">URL to where the control can be actioned.</span></span> |
|<span data-ttu-id="625c3-139">controlCategory</span><span class="sxs-lookup"><span data-stu-id="625c3-139">controlCategory</span></span>|<span data-ttu-id="625c3-140">String</span><span class="sxs-lookup"><span data-stu-id="625c3-140">String</span></span>|<span data-ttu-id="625c3-141">Categoria de ação de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).</span><span class="sxs-lookup"><span data-stu-id="625c3-141">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span>|
|<span data-ttu-id="625c3-142">title</span><span class="sxs-lookup"><span data-stu-id="625c3-142">title</span></span>|<span data-ttu-id="625c3-143">String</span><span class="sxs-lookup"><span data-stu-id="625c3-143">String</span></span>|<span data-ttu-id="625c3-144">Título do controle.</span><span class="sxs-lookup"><span data-stu-id="625c3-144">Title of the control.</span></span>|
|<span data-ttu-id="625c3-145">preterido</span><span class="sxs-lookup"><span data-stu-id="625c3-145">deprecated</span></span>|<span data-ttu-id="625c3-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="625c3-146">Boolean</span></span>|<span data-ttu-id="625c3-147">Sinalizador para indicar se um controle está depreciado.</span><span class="sxs-lookup"><span data-stu-id="625c3-147">Flag to indicate if a control is depreciated.</span></span>|
|<span data-ttu-id="625c3-148">implementationCost</span><span class="sxs-lookup"><span data-stu-id="625c3-148">implementationCost</span></span>|<span data-ttu-id="625c3-149">String</span><span class="sxs-lookup"><span data-stu-id="625c3-149">String</span></span>|<span data-ttu-id="625c3-150">Custo do recurso do controle implemmentating (baixo, moderado, alto).</span><span class="sxs-lookup"><span data-stu-id="625c3-150">Resource cost of implemmentating control (low, moderate, high).</span></span>|
|<span data-ttu-id="625c3-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="625c3-151">lastModifiedDateTime</span></span>|<span data-ttu-id="625c3-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="625c3-152">DateTimeOffset</span></span>|<span data-ttu-id="625c3-153">Hora em que a entidade de perfil de controle foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="625c3-153">Time at which the control profile entity was last modified.</span></span> <span data-ttu-id="625c3-154">O tipo TIMESTAMP representa data e hora</span><span class="sxs-lookup"><span data-stu-id="625c3-154">The Timestamp type represents date and time</span></span>| 
|<span data-ttu-id="625c3-155">maxScore</span><span class="sxs-lookup"><span data-stu-id="625c3-155">maxScore</span></span>|<span data-ttu-id="625c3-156">Duplo</span><span class="sxs-lookup"><span data-stu-id="625c3-156">Double</span></span>|<span data-ttu-id="625c3-157">Pontuação máxima atingível do controle.</span><span class="sxs-lookup"><span data-stu-id="625c3-157">max attainable score for the control.</span></span>|
|<span data-ttu-id="625c3-158">classificação</span><span class="sxs-lookup"><span data-stu-id="625c3-158">rank</span></span>|<span data-ttu-id="625c3-159">Int32</span><span class="sxs-lookup"><span data-stu-id="625c3-159">Int32</span></span>|<span data-ttu-id="625c3-160">Classificação de pilha da Microsoft de controle.</span><span class="sxs-lookup"><span data-stu-id="625c3-160">Microsoft's stack ranking of control.</span></span>|
|<span data-ttu-id="625c3-161">correção</span><span class="sxs-lookup"><span data-stu-id="625c3-161">remediation</span></span>|<span data-ttu-id="625c3-162">String</span><span class="sxs-lookup"><span data-stu-id="625c3-162">String</span></span>|<span data-ttu-id="625c3-163">Descrição do que o controle ajudará a corrigir.</span><span class="sxs-lookup"><span data-stu-id="625c3-163">Description of what the control will help remediate.</span></span>|
|<span data-ttu-id="625c3-164">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="625c3-164">remediationImpact</span></span>|<span data-ttu-id="625c3-165">String</span><span class="sxs-lookup"><span data-stu-id="625c3-165">String</span></span>|<span data-ttu-id="625c3-166">Descrição do impacto sobre os usuários da correção.</span><span class="sxs-lookup"><span data-stu-id="625c3-166">Description of the impact on users of the remediation.</span></span>|
|<span data-ttu-id="625c3-167">service</span><span class="sxs-lookup"><span data-stu-id="625c3-167">service</span></span>|<span data-ttu-id="625c3-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="625c3-168">String</span></span>|<span data-ttu-id="625c3-169">Serviço que possui o controle (Exchange, SharePoint, Azure AD).</span><span class="sxs-lookup"><span data-stu-id="625c3-169">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span>|
|<span data-ttu-id="625c3-170">las</span><span class="sxs-lookup"><span data-stu-id="625c3-170">threats</span></span>|<span data-ttu-id="625c3-171">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="625c3-171">String collection</span></span>|<span data-ttu-id="625c3-172">Lista de ameaças que o controle atenua (accountBreach, dataexclusão, dataExfiltration, dataderramamento</span><span class="sxs-lookup"><span data-stu-id="625c3-172">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,</span></span>
<span data-ttu-id="625c3-173">elevationOfPrivilege, maliciousInsider, passwordCracking, phishingOrWhaling, falsificação).</span><span class="sxs-lookup"><span data-stu-id="625c3-173">elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span>|
|<span data-ttu-id="625c3-174">camada</span><span class="sxs-lookup"><span data-stu-id="625c3-174">tier</span></span>|<span data-ttu-id="625c3-175">String</span><span class="sxs-lookup"><span data-stu-id="625c3-175">String</span></span>|<span data-ttu-id="625c3-176">Camada de controle (Core, defesa profunda, avançada)</span><span class="sxs-lookup"><span data-stu-id="625c3-176">Control tier (Core, Defense in Depth, Advanced.)</span></span>   |
|<span data-ttu-id="625c3-177">userimpact</span><span class="sxs-lookup"><span data-stu-id="625c3-177">userImpact</span></span>|<span data-ttu-id="625c3-178">String</span><span class="sxs-lookup"><span data-stu-id="625c3-178">String</span></span>|<span data-ttu-id="625c3-179">Impacto do usuário da implementação do controle (baixo, moderado, alto).</span><span class="sxs-lookup"><span data-stu-id="625c3-179">User impact of implementing control (low, moderate, high).</span></span>   |
|<span data-ttu-id="625c3-180">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="625c3-180">complianceInformation</span></span>|<span data-ttu-id="625c3-181">coleção [complianceInformation](complianceinformation.md)</span><span class="sxs-lookup"><span data-stu-id="625c3-181">[complianceInformation](complianceinformation.md) collection</span></span>|<span data-ttu-id="625c3-182">O conjunto de informações de conformidade associadas ao controle de Pontuação segura</span><span class="sxs-lookup"><span data-stu-id="625c3-182">The collection of compliance information associated with secure score control</span></span>|
|<span data-ttu-id="625c3-183">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="625c3-183">controlStateUpdates</span></span>|<span data-ttu-id="625c3-184">coleção [secureScoreControlStateUpdate](securescorecontrolstateupdate.md)</span><span class="sxs-lookup"><span data-stu-id="625c3-184">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection</span></span>|<span data-ttu-id="625c3-185">Sinalizador para indicar onde o locatário marcou um controle (ignorado, terceiros, revisado) (suporta [atualização](../api/securescorecontrolprofile-update.md)).</span><span class="sxs-lookup"><span data-stu-id="625c3-185">Flag to indicate where the tenant has marked a control (ignored, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofile-update.md)).</span></span>|
|<span data-ttu-id="625c3-186">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="625c3-186">vendorInformation</span></span>|[<span data-ttu-id="625c3-187">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="625c3-187">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="625c3-188">Tipo complexo que contém detalhes sobre o fornecedor de produtos/serviços de segurança, o provedor e o subfornecedor (por exemplo, fornecedor = Microsoft; Provider = SecureScore).</span><span class="sxs-lookup"><span data-stu-id="625c3-188">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore).</span></span> <span data-ttu-id="625c3-189">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="625c3-189">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="625c3-190">Relações</span><span class="sxs-lookup"><span data-stu-id="625c3-190">Relationships</span></span>

<span data-ttu-id="625c3-191">Nenhum</span><span class="sxs-lookup"><span data-stu-id="625c3-191">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="625c3-192">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="625c3-192">JSON representation</span></span>

<span data-ttu-id="625c3-193">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="625c3-193">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
}-->

```json
{
  "id": "String (identifier)",
  "azureTenantId": "String",
  "actionType": "String",
  "actionUrl": "String",
  "controlCategory": "String",
  "title": "String", 
  "deprecated": "Boolean",
  "implementationCost": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "maxScore": "Double",
  "rank": "Int32",
  "remediation": "String",
  "remediationImpact": "String",
  "service": "String",
  "threats": ["String"],
  "tier": "String",
  "userImpact": "String",
  "complianceInformation": [{"@odata.type": "microsoft.graph.complianceInformation"}], 
  "controlStateUpdates": [{"@odata.type": "microsoft.graph.secureScoreControlStateUpdate"}],
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

