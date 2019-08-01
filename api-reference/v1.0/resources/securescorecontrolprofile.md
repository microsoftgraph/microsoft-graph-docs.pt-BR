---
title: tipo de recurso secureScoreControlProfile
description: Representa a pontuação segura de um locatário por dados de controle. Por padrão, ele retorna todos os controles de um locatário e pode explicitamente extrair controles individuais.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 40bee951d3030772973911510ebba7cc90f412ae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034486"
---
# <a name="securescorecontrolprofile-resource-type"></a><span data-ttu-id="b9684-104">tipo de recurso secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="b9684-104">secureScoreControlProfile resource type</span></span>

<span data-ttu-id="b9684-105">Representa a pontuação segura de um locatário por dados de controle.</span><span class="sxs-lookup"><span data-stu-id="b9684-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="b9684-106">Por padrão, ele retorna todos os controles de um locatário e pode explicitamente extrair controles individuais.</span><span class="sxs-lookup"><span data-stu-id="b9684-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="b9684-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="b9684-107">Methods</span></span>

| <span data-ttu-id="b9684-108">Método</span><span class="sxs-lookup"><span data-stu-id="b9684-108">Method</span></span>   | <span data-ttu-id="b9684-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b9684-109">Return Type</span></span>|<span data-ttu-id="b9684-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9684-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b9684-111">Lista secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="b9684-111">List secureScoreControlProfiles</span></span>](../api/security-list-securescorecontrolprofiles.md) | [<span data-ttu-id="b9684-112">secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="b9684-112">secureScoreControlProfile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="b9684-113">Leia as propriedades e os metadados de um objeto secureScoreControlProfiles.</span><span class="sxs-lookup"><span data-stu-id="b9684-113">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|
|[<span data-ttu-id="b9684-114">Obter secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="b9684-114">Get secureScoreControlProfile</span></span>](../api/securescorecontrolprofile-get.md) | [<span data-ttu-id="b9684-115">securescorecontrolprofile</span><span class="sxs-lookup"><span data-stu-id="b9684-115">securescorecontrolprofile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="b9684-116">Leia as propriedades e os metadados de um objeto secureScoreControlProfiles.</span><span class="sxs-lookup"><span data-stu-id="b9684-116">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|
|[<span data-ttu-id="b9684-117">Atualizar securescorecontrolprofile</span><span class="sxs-lookup"><span data-stu-id="b9684-117">Update securescorecontrolprofile</span></span>](../api/securescorecontrolprofile-update.md) | [<span data-ttu-id="b9684-118">securescorecontrolprofile</span><span class="sxs-lookup"><span data-stu-id="b9684-118">securescorecontrolprofile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="b9684-119">Atualize um objeto securescorecontrolprofile.</span><span class="sxs-lookup"><span data-stu-id="b9684-119">Update an securescorecontrolprofile object.</span></span> |


## <a name="properties"></a><span data-ttu-id="b9684-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9684-120">Properties</span></span>

|<span data-ttu-id="b9684-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b9684-121">Name</span></span> |<span data-ttu-id="b9684-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9684-122">Type</span></span> |<span data-ttu-id="b9684-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9684-123">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="b9684-124">id</span><span class="sxs-lookup"><span data-stu-id="b9684-124">id</span></span>|<span data-ttu-id="b9684-125">String</span><span class="sxs-lookup"><span data-stu-id="b9684-125">String</span></span>|<span data-ttu-id="b9684-126">Identificador GUID/exclusivo gerado pelo provedor.</span><span class="sxs-lookup"><span data-stu-id="b9684-126">Provider-generated GUID/unique identifier.</span></span> <span data-ttu-id="b9684-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b9684-127">Read-only.</span></span> <span data-ttu-id="b9684-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9684-128">Required.</span></span>|
|<span data-ttu-id="b9684-129">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="b9684-129">azureTenantId</span></span>|<span data-ttu-id="b9684-130">String</span><span class="sxs-lookup"><span data-stu-id="b9684-130">String</span></span>|<span data-ttu-id="b9684-131">Cadeia de caracteres GUID para ID do locatário.</span><span class="sxs-lookup"><span data-stu-id="b9684-131">GUID string for tenant ID.</span></span>|
|<span data-ttu-id="b9684-132">actionType</span><span class="sxs-lookup"><span data-stu-id="b9684-132">actionType</span></span>|<span data-ttu-id="b9684-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9684-133">String</span></span>|<span data-ttu-id="b9684-134">Tipo de ação de controle (configuração, revisão, comportamento).</span><span class="sxs-lookup"><span data-stu-id="b9684-134">Control action type (Config, Review, Behavior).</span></span>|
|<span data-ttu-id="b9684-135">actionUrl</span><span class="sxs-lookup"><span data-stu-id="b9684-135">actionUrl</span></span>|<span data-ttu-id="b9684-136">String</span><span class="sxs-lookup"><span data-stu-id="b9684-136">String</span></span>|<span data-ttu-id="b9684-137">URL para onde o controle pode ser acionado.</span><span class="sxs-lookup"><span data-stu-id="b9684-137">URL to where the control can be actioned.</span></span> |
|<span data-ttu-id="b9684-138">controlCategory</span><span class="sxs-lookup"><span data-stu-id="b9684-138">controlCategory</span></span>|<span data-ttu-id="b9684-139">String</span><span class="sxs-lookup"><span data-stu-id="b9684-139">String</span></span>|<span data-ttu-id="b9684-140">Categoria de ação de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).</span><span class="sxs-lookup"><span data-stu-id="b9684-140">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span>|
|<span data-ttu-id="b9684-141">title</span><span class="sxs-lookup"><span data-stu-id="b9684-141">title</span></span>|<span data-ttu-id="b9684-142">String</span><span class="sxs-lookup"><span data-stu-id="b9684-142">String</span></span>|<span data-ttu-id="b9684-143">Título do controle.</span><span class="sxs-lookup"><span data-stu-id="b9684-143">Title of the control.</span></span>|
|<span data-ttu-id="b9684-144">preterido</span><span class="sxs-lookup"><span data-stu-id="b9684-144">deprecated</span></span>|<span data-ttu-id="b9684-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="b9684-145">Boolean</span></span>|<span data-ttu-id="b9684-146">Sinalizador para indicar se um controle está depreciado.</span><span class="sxs-lookup"><span data-stu-id="b9684-146">Flag to indicate if a control is depreciated.</span></span>|
|<span data-ttu-id="b9684-147">implementationCost</span><span class="sxs-lookup"><span data-stu-id="b9684-147">implementationCost</span></span>|<span data-ttu-id="b9684-148">String</span><span class="sxs-lookup"><span data-stu-id="b9684-148">String</span></span>|<span data-ttu-id="b9684-149">Custo do recurso do controle implemmentating (baixo, moderado, alto).</span><span class="sxs-lookup"><span data-stu-id="b9684-149">Resource cost of implemmentating control (low, moderate, high).</span></span>|
|<span data-ttu-id="b9684-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9684-150">lastModifiedDateTime</span></span>|<span data-ttu-id="b9684-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9684-151">DateTimeOffset</span></span>|<span data-ttu-id="b9684-152">Hora em que a entidade de perfil de controle foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b9684-152">Time at which the control profile entity was last modified.</span></span> <span data-ttu-id="b9684-153">O tipo TIMESTAMP representa data e hora</span><span class="sxs-lookup"><span data-stu-id="b9684-153">The Timestamp type represents date and time</span></span>| 
|<span data-ttu-id="b9684-154">maxScore</span><span class="sxs-lookup"><span data-stu-id="b9684-154">maxScore</span></span>|<span data-ttu-id="b9684-155">Duplo</span><span class="sxs-lookup"><span data-stu-id="b9684-155">Double</span></span>|<span data-ttu-id="b9684-156">Pontuação máxima atingível do controle.</span><span class="sxs-lookup"><span data-stu-id="b9684-156">max attainable score for the control.</span></span>|
|<span data-ttu-id="b9684-157">classificação</span><span class="sxs-lookup"><span data-stu-id="b9684-157">rank</span></span>|<span data-ttu-id="b9684-158">Int32</span><span class="sxs-lookup"><span data-stu-id="b9684-158">Int32</span></span>|<span data-ttu-id="b9684-159">Classificação de pilha da Microsoft de controle.</span><span class="sxs-lookup"><span data-stu-id="b9684-159">Microsoft's stack ranking of control.</span></span>|
|<span data-ttu-id="b9684-160">correção</span><span class="sxs-lookup"><span data-stu-id="b9684-160">remediation</span></span>|<span data-ttu-id="b9684-161">String</span><span class="sxs-lookup"><span data-stu-id="b9684-161">String</span></span>|<span data-ttu-id="b9684-162">Descrição do que o controle ajudará a corrigir.</span><span class="sxs-lookup"><span data-stu-id="b9684-162">Description of what the control will help remediate.</span></span>|
|<span data-ttu-id="b9684-163">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="b9684-163">remediationImpact</span></span>|<span data-ttu-id="b9684-164">String</span><span class="sxs-lookup"><span data-stu-id="b9684-164">String</span></span>|<span data-ttu-id="b9684-165">Descrição do impacto sobre os usuários da correção.</span><span class="sxs-lookup"><span data-stu-id="b9684-165">Description of the impact on users of the remediation.</span></span>|
|<span data-ttu-id="b9684-166">service</span><span class="sxs-lookup"><span data-stu-id="b9684-166">service</span></span>|<span data-ttu-id="b9684-167">String</span><span class="sxs-lookup"><span data-stu-id="b9684-167">String</span></span>|<span data-ttu-id="b9684-168">Serviço que possui o controle (Exchange, SharePoint, Azure AD).</span><span class="sxs-lookup"><span data-stu-id="b9684-168">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span>|
|<span data-ttu-id="b9684-169">las</span><span class="sxs-lookup"><span data-stu-id="b9684-169">threats</span></span>|<span data-ttu-id="b9684-170">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9684-170">String collection</span></span>|<span data-ttu-id="b9684-171">Lista de ameaças que o controle atenua (accountBreach, dataexclusão, dataExfiltration, dataderramamento</span><span class="sxs-lookup"><span data-stu-id="b9684-171">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,</span></span>
<span data-ttu-id="b9684-172">elevationOfPrivilege, maliciousInsider, passwordCracking, phishingOrWhaling, falsificação).</span><span class="sxs-lookup"><span data-stu-id="b9684-172">elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span>|
|<span data-ttu-id="b9684-173">camada</span><span class="sxs-lookup"><span data-stu-id="b9684-173">tier</span></span>|<span data-ttu-id="b9684-174">String</span><span class="sxs-lookup"><span data-stu-id="b9684-174">String</span></span>|<span data-ttu-id="b9684-175">Camada de controle (Core, defesa profunda, avançada)</span><span class="sxs-lookup"><span data-stu-id="b9684-175">Control tier (Core, Defense in Depth, Advanced.)</span></span>   |
|<span data-ttu-id="b9684-176">userimpact</span><span class="sxs-lookup"><span data-stu-id="b9684-176">userImpact</span></span>|<span data-ttu-id="b9684-177">String</span><span class="sxs-lookup"><span data-stu-id="b9684-177">String</span></span>|<span data-ttu-id="b9684-178">Impacto do usuário da implementação do controle (baixo, moderado, alto).</span><span class="sxs-lookup"><span data-stu-id="b9684-178">User impact of implementing control (low, moderate, high).</span></span>   |
|<span data-ttu-id="b9684-179">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="b9684-179">complianceInformation</span></span>|<span data-ttu-id="b9684-180">coleção [complianceInformation](complianceinformation.md)</span><span class="sxs-lookup"><span data-stu-id="b9684-180">[complianceInformation](complianceinformation.md) collection</span></span>|<span data-ttu-id="b9684-181">O conjunto de informações de conformidade associadas ao controle de Pontuação segura</span><span class="sxs-lookup"><span data-stu-id="b9684-181">The collection of compliance information associated with secure score control</span></span>|
|<span data-ttu-id="b9684-182">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="b9684-182">controlStateUpdates</span></span>|<span data-ttu-id="b9684-183">coleção [secureScoreControlStateUpdate](securescorecontrolstateupdate.md)</span><span class="sxs-lookup"><span data-stu-id="b9684-183">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection</span></span>|<span data-ttu-id="b9684-184">Sinalizador para indicar onde o locatário marcou um controle (ignorado, terceiros, revisado) (suporta [atualização](../api/securescorecontrolprofile-update.md)).</span><span class="sxs-lookup"><span data-stu-id="b9684-184">Flag to indicate where the tenant has marked a control (ignored, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofile-update.md)).</span></span>|
|<span data-ttu-id="b9684-185">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="b9684-185">vendorInformation</span></span>|[<span data-ttu-id="b9684-186">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="b9684-186">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="b9684-187">Tipo complexo que contém detalhes sobre o fornecedor de produtos/serviços de segurança, o provedor e o subfornecedor (por exemplo, fornecedor = Microsoft; Provider = SecureScore).</span><span class="sxs-lookup"><span data-stu-id="b9684-187">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore).</span></span> <span data-ttu-id="b9684-188">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9684-188">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9684-189">Relações</span><span class="sxs-lookup"><span data-stu-id="b9684-189">Relationships</span></span>

<span data-ttu-id="b9684-190">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b9684-190">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9684-191">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9684-191">JSON representation</span></span>

<span data-ttu-id="b9684-192">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b9684-192">The following is a JSON representation of the resource.</span></span>

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
