---
title: tipo de recurso de secureScoreControlProfiles
description: Representa a pontuação seguro de um locatário por dados do controle. Por padrão, ela retorna todos os controles para um inquilino e explicitamente pode extrair controles individuais.
ms.openlocfilehash: e02c9ae3b1431b131576e2e0e115377dd3480bc2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038542"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="cd936-104">tipo de recurso de secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="cd936-104">secureScoreControlProfiles resource type</span></span>

> <span data-ttu-id="cd936-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cd936-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd936-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cd936-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd936-107">Representa a pontuação seguro de um locatário por dados do controle.</span><span class="sxs-lookup"><span data-stu-id="cd936-107">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="cd936-108">Por padrão, ela retorna todos os controles para um inquilino e explicitamente pode extrair controles individuais.</span><span class="sxs-lookup"><span data-stu-id="cd936-108">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="cd936-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="cd936-109">Methods</span></span>

| <span data-ttu-id="cd936-110">Método</span><span class="sxs-lookup"><span data-stu-id="cd936-110">Method</span></span>   | <span data-ttu-id="cd936-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cd936-111">Return Type</span></span>|<span data-ttu-id="cd936-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd936-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cd936-113">Lista secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="cd936-113">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="cd936-114">secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="cd936-114">secureScoreControlProfiles</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="cd936-115">Leia as propriedades e os metadados de um objeto secureScoreControlProfiles.</span><span class="sxs-lookup"><span data-stu-id="cd936-115">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="cd936-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cd936-116">Properties</span></span>

|<span data-ttu-id="cd936-117">Nome</span><span class="sxs-lookup"><span data-stu-id="cd936-117">Name</span></span> |<span data-ttu-id="cd936-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd936-118">Type</span></span> |<span data-ttu-id="cd936-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd936-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="cd936-120">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="cd936-120">azureTenantId</span></span>   |   <span data-ttu-id="cd936-121">String</span><span class="sxs-lookup"><span data-stu-id="cd936-121">String</span></span>  |   <span data-ttu-id="cd936-122">ID de cadeia de caracteres do GUID para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="cd936-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="cd936-123">controlName</span><span class="sxs-lookup"><span data-stu-id="cd936-123">controlName</span></span> |   <span data-ttu-id="cd936-124">String</span><span class="sxs-lookup"><span data-stu-id="cd936-124">String</span></span>  |   <span data-ttu-id="cd936-125">Nome do controle.</span><span class="sxs-lookup"><span data-stu-id="cd936-125">Name of the control.</span></span> |
|   <span data-ttu-id="cd936-126">title</span><span class="sxs-lookup"><span data-stu-id="cd936-126">title</span></span>   |   <span data-ttu-id="cd936-127">String</span><span class="sxs-lookup"><span data-stu-id="cd936-127">String</span></span>  |   <span data-ttu-id="cd936-128">Título do controle.</span><span class="sxs-lookup"><span data-stu-id="cd936-128">Title of the control.</span></span>   |
|   <span data-ttu-id="cd936-129">controlCategory</span><span class="sxs-lookup"><span data-stu-id="cd936-129">controlCategory</span></span> |   <span data-ttu-id="cd936-130">String</span><span class="sxs-lookup"><span data-stu-id="cd936-130">String</span></span>  |   <span data-ttu-id="cd936-131">Categoria de ação de controle (conta, dados, dispositivo, aplicativos, infra-estrutura).</span><span class="sxs-lookup"><span data-stu-id="cd936-131">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="cd936-132">actionType</span><span class="sxs-lookup"><span data-stu-id="cd936-132">actionType</span></span>  |   <span data-ttu-id="cd936-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd936-133">String</span></span>  |   <span data-ttu-id="cd936-134">Controlar o tipo de ação (Config, revisão, comportamento).</span><span class="sxs-lookup"><span data-stu-id="cd936-134">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="cd936-135">service</span><span class="sxs-lookup"><span data-stu-id="cd936-135">service</span></span> |   <span data-ttu-id="cd936-136">String</span><span class="sxs-lookup"><span data-stu-id="cd936-136">String</span></span>  |   <span data-ttu-id="cd936-137">Serviço que possui o controle (Exchange, Sharepoint, Azure AD).</span><span class="sxs-lookup"><span data-stu-id="cd936-137">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="cd936-138">maxScore</span><span class="sxs-lookup"><span data-stu-id="cd936-138">maxScore</span></span> |  <span data-ttu-id="cd936-139">String</span><span class="sxs-lookup"><span data-stu-id="cd936-139">String</span></span>  |   <span data-ttu-id="cd936-140">Atual obtidos max pontuação na data especificada.</span><span class="sxs-lookup"><span data-stu-id="cd936-140">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="cd936-141">camada</span><span class="sxs-lookup"><span data-stu-id="cd936-141">tier</span></span> |  <span data-ttu-id="cd936-142">String</span><span class="sxs-lookup"><span data-stu-id="cd936-142">String</span></span>  |   <span data-ttu-id="cd936-143">Camada de controle (Core, defesa em camadas, avançadas.)</span><span class="sxs-lookup"><span data-stu-id="cd936-143">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="cd936-144">userImpact</span><span class="sxs-lookup"><span data-stu-id="cd936-144">userImpact</span></span> |    <span data-ttu-id="cd936-145">String</span><span class="sxs-lookup"><span data-stu-id="cd936-145">String</span></span>  | <span data-ttu-id="cd936-146">Impacto da implementação de controle (baixa, moderada, alta) do usuário.</span><span class="sxs-lookup"><span data-stu-id="cd936-146">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="cd936-147">implementationCost</span><span class="sxs-lookup"><span data-stu-id="cd936-147">implementationCost</span></span> |    <span data-ttu-id="cd936-148">String</span><span class="sxs-lookup"><span data-stu-id="cd936-148">String</span></span>  |   <span data-ttu-id="cd936-149">Custo do recurso de controle de implemmentating (baixa, moderada, alta).</span><span class="sxs-lookup"><span data-stu-id="cd936-149">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="cd936-150">rank</span><span class="sxs-lookup"><span data-stu-id="cd936-150">rank</span></span> |  <span data-ttu-id="cd936-151">Int32</span><span class="sxs-lookup"><span data-stu-id="cd936-151">Int32</span></span>   |   <span data-ttu-id="cd936-152">Pilha da Microsoft de classificação do controle.</span><span class="sxs-lookup"><span data-stu-id="cd936-152">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="cd936-153">ameaças</span><span class="sxs-lookup"><span data-stu-id="cd936-153">threats</span></span> |   <span data-ttu-id="cd936-154">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd936-154">String Collection</span></span>   |   <span data-ttu-id="cd936-155">Lista de ameaças reduz o controle (accountBreach, dataDeletion, dataExfiltration, dataSpillage, elevationOfPrivilege, maliciousInsider, passwordCracking, phishingOrWhaling, falsificação).</span><span class="sxs-lookup"><span data-stu-id="cd936-155">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="cd936-156">preteridos</span><span class="sxs-lookup"><span data-stu-id="cd936-156">deprecated</span></span> |    <span data-ttu-id="cd936-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="cd936-157">Boolean</span></span> |   <span data-ttu-id="cd936-158">Sinalizador para indicar se um controle é depreciado.</span><span class="sxs-lookup"><span data-stu-id="cd936-158">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="cd936-159">remediação</span><span class="sxs-lookup"><span data-stu-id="cd936-159">remediation</span></span> |   <span data-ttu-id="cd936-160">String</span><span class="sxs-lookup"><span data-stu-id="cd936-160">String</span></span>  |   <span data-ttu-id="cd936-161">Descrição do controle que ajudarão remediar.</span><span class="sxs-lookup"><span data-stu-id="cd936-161">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="cd936-162">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="cd936-162">remediationImpact</span></span> | <span data-ttu-id="cd936-163">String</span><span class="sxs-lookup"><span data-stu-id="cd936-163">String</span></span>  |   <span data-ttu-id="cd936-164">Descrição do impacto sobre os usuários da remediação.</span><span class="sxs-lookup"><span data-stu-id="cd936-164">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="cd936-165">actionUrl</span><span class="sxs-lookup"><span data-stu-id="cd936-165">actionUrl</span></span> | <span data-ttu-id="cd936-166">String</span><span class="sxs-lookup"><span data-stu-id="cd936-166">String</span></span>  |   <span data-ttu-id="cd936-167">URL para o qual o controle pode ser actioned.</span><span class="sxs-lookup"><span data-stu-id="cd936-167">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="cd936-168">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="cd936-168">controlStateUpdates</span></span> |   <span data-ttu-id="cd936-169">String</span><span class="sxs-lookup"><span data-stu-id="cd936-169">String</span></span>  |   <span data-ttu-id="cd936-170">Sinalizador para indicar onde o inquilino tenha marcado a um controle (Ignorar, thirdParty, examinado) (oferece suporte a [atualização](../api/securescorecontrolprofiles-update.md)).</span><span class="sxs-lookup"><span data-stu-id="cd936-170">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="cd936-171">tenantNote</span><span class="sxs-lookup"><span data-stu-id="cd936-171">tenantNote</span></span> |    <span data-ttu-id="cd936-172">String</span><span class="sxs-lookup"><span data-stu-id="cd936-172">String</span></span>  |   <span data-ttu-id="cd936-173">Inquilino pode ser definida por comentários do controle (suporta a [atualização](../api/securescorecontrolprofiles-update.md)).</span><span class="sxs-lookup"><span data-stu-id="cd936-173">Tenant can set per control comments (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="cd936-174">assignedTo</span><span class="sxs-lookup"><span data-stu-id="cd936-174">assignedTo</span></span> |    <span data-ttu-id="cd936-175">String</span><span class="sxs-lookup"><span data-stu-id="cd936-175">String</span></span>  |   <span data-ttu-id="cd936-176">Inquilino pode atribuir o controle a um indivíduo (suporta a [atualização](../api/securescorecontrolprofiles-update.md)).</span><span class="sxs-lookup"><span data-stu-id="cd936-176">Tenant can assign the control to a individual (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="cd936-177">updatedBy</span><span class="sxs-lookup"><span data-stu-id="cd936-177">updatedBy</span></span> | <span data-ttu-id="cd936-178">String</span><span class="sxs-lookup"><span data-stu-id="cd936-178">String</span></span>  |   <span data-ttu-id="cd936-179">Nome principal do usuário de quem fez as alterações para o estado de um controle.</span><span class="sxs-lookup"><span data-stu-id="cd936-179">User principal name of who made changes to a control's state.</span></span> |

## <a name="relationships"></a><span data-ttu-id="cd936-180">Relações</span><span class="sxs-lookup"><span data-stu-id="cd936-180">Relationships</span></span>

<span data-ttu-id="cd936-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cd936-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd936-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cd936-182">JSON representation</span></span>

<span data-ttu-id="cd936-183">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cd936-183">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScores"
}-->

```json
{
"title": "String", 
"azureTenantId": "Guid", 
"referenceId": "String", 
"controlName": "String", 
"maxScore": "Int32",
"actionCategory": "Collection(microsoft.graph.SecureScore.actionCategory)",
"actionType": "Collection(microsoft.graph.SecureScore.actionType)",
"service": "String",
"tier": "Collection(microsoft.graph.SecureScore.tier)",
"userImpact": "Collection(microsoft.graph.SecureScore.ranking)",
"implementationCost ": "Collection(microsoft.graph.SecureScore.ranking)",
"rank ": "Int32",
"threats": "Collection(microsoft.graph.SecureScore.threat)",
"deprecated ": "Boolean",
"remediation": "String",
"remediationImpact ": "String",
"actionUrl": "String",
"controlStateUpdates": "Collection(microsoft.graph.SecureScore.controlStateUpdates)",
"tenantNotes": "String",
"upn": "String",
"comments": "String",
}


```


<!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
