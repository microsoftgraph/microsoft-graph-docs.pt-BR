---
title: tipo de recurso de secureScoreControlProfiles
description: Representa a pontuação seguro de um locatário por dados do controle. Por padrão, ela retorna todos os controles para um inquilino e explicitamente pode extrair controles individuais.
localization_priority: Normal
ms.openlocfilehash: 866b2086ff5160744f848292cedf30c3cedf6daa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866217"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="2e1e2-104">tipo de recurso de secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="2e1e2-104">secureScoreControlProfiles resource type</span></span>

> <span data-ttu-id="2e1e2-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2e1e2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2e1e2-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2e1e2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2e1e2-107">Representa a pontuação seguro de um locatário por dados do controle.</span><span class="sxs-lookup"><span data-stu-id="2e1e2-107">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="2e1e2-108">Por padrão, ela retorna todos os controles para um inquilino e explicitamente pode extrair controles individuais.</span><span class="sxs-lookup"><span data-stu-id="2e1e2-108">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="2e1e2-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="2e1e2-109">Methods</span></span>

| <span data-ttu-id="2e1e2-110">Método</span><span class="sxs-lookup"><span data-stu-id="2e1e2-110">Method</span></span>   | <span data-ttu-id="2e1e2-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2e1e2-111">Return Type</span></span>|<span data-ttu-id="2e1e2-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e1e2-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2e1e2-113">Lista secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="2e1e2-113">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="2e1e2-114">secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="2e1e2-114">secureScoreControlProfiles</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="2e1e2-115">Leia as propriedades e os metadados de um objeto secureScoreControlProfiles.</span><span class="sxs-lookup"><span data-stu-id="2e1e2-115">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="2e1e2-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2e1e2-116">Properties</span></span>

|<span data-ttu-id="2e1e2-117">Nome</span><span class="sxs-lookup"><span data-stu-id="2e1e2-117">Name</span></span> |<span data-ttu-id="2e1e2-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e1e2-118">Type</span></span> |<span data-ttu-id="2e1e2-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e1e2-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="2e1e2-120">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="2e1e2-120">azureTenantId</span></span>   |   <span data-ttu-id="2e1e2-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e1e2-121">String</span></span>  |   <span data-ttu-id="2e1e2-122">ID de cadeia de caracteres do GUID para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="2e1e2-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="2e1e2-123">controlName</span><span class="sxs-lookup"><span data-stu-id="2e1e2-123">controlName</span></span> |   <span data-ttu-id="2e1e2-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e1e2-124">String</span></span>  |   <span data-ttu-id="2e1e2-125">Nome do controle.</span><span class="sxs-lookup"><span data-stu-id="2e1e2-125">Name of the control.</span></span> |
|   <span data-ttu-id="2e1e2-126">title</span><span class="sxs-lookup"><span data-stu-id="2e1e2-126">title</span></span>   |   <span data-ttu-id="2e1e2-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e1e2-127">String</span></span>  |   <span data-ttu-id="2e1e2-128">Título do controle.</span><span class="sxs-lookup"><span data-stu-id="2e1e2-128">Title of the control.</span></span>   |
| <span data-ttu-id="2e1e2-129">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="2e1e2-129">complianceInformation</span></span> | <span data-ttu-id="2e1e2-130">coleção [complianceInformation](complianceinformation.md)</span><span class="sxs-lookup"><span data-stu-id="2e1e2-130">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="2e1e2-131">A coleção de informações de conformidade associadas a proteger o controle de pontuação</span><span class="sxs-lookup"><span data-stu-id="2e1e2-131">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="2e1e2-132">controlCategory</span><span class="sxs-lookup"><span data-stu-id="2e1e2-132">controlCategory</span></span> |   <span data-ttu-id="2e1e2-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e1e2-133">String</span></span>  |   <span data-ttu-id="2e1e2-134">Categoria de ação de controle (conta, dados, dispositivo, aplicativos, infra-estrutura).</span><span class="sxs-lookup"><span data-stu-id="2e1e2-134">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="2e1e2-135">actionType</span><span class="sxs-lookup"><span data-stu-id="2e1e2-135">actionType</span></span>  |   <span data-ttu-id="2e1e2-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e1e2-136">String</span></span>  |   <span data-ttu-id="2e1e2-137">Controlar o tipo de ação (Config, revisão, comportamento).</span><span class="sxs-lookup"><span data-stu-id="2e1e2-137">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="2e1e2-138">service</span><span class="sxs-lookup"><span data-stu-id="2e1e2-138">service</span></span> |   <span data-ttu-id="2e1e2-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e1e2-139">String</span></span>  |   <span data-ttu-id="2e1e2-140">Serviço que possui o controle (Exchange, Sharepoint, Azure AD).</span><span class="sxs-lookup"><span data-stu-id="2e1e2-140">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="2e1e2-141">maxScore</span><span class="sxs-lookup"><span data-stu-id="2e1e2-141">maxScore</span></span> |  <span data-ttu-id="2e1e2-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e1e2-142">String</span></span>  |   <span data-ttu-id="2e1e2-143">Atual obtidos max pontuação na data especificada.</span><span class="sxs-lookup"><span data-stu-id="2e1e2-143">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="2e1e2-144">camada</span><span class="sxs-lookup"><span data-stu-id="2e1e2-144">tier</span></span> |  <span data-ttu-id="2e1e2-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e1e2-145">String</span></span>  |   <span data-ttu-id="2e1e2-146">Camada de controle (Core, defesa em camadas, avançadas.)</span><span class="sxs-lookup"><span data-stu-id="2e1e2-146">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="2e1e2-147">userImpact</span><span class="sxs-lookup"><span data-stu-id="2e1e2-147">userImpact</span></span> |    <span data-ttu-id="2e1e2-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e1e2-148">String</span></span>  | <span data-ttu-id="2e1e2-149">Impacto da implementação de controle (baixa, moderada, alta) do usuário.</span><span class="sxs-lookup"><span data-stu-id="2e1e2-149">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="2e1e2-150">implementationCost</span><span class="sxs-lookup"><span data-stu-id="2e1e2-150">implementationCost</span></span> |    <span data-ttu-id="2e1e2-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e1e2-151">String</span></span>  |   <span data-ttu-id="2e1e2-152">Custo do recurso de controle de implemmentating (baixa, moderada, alta).</span><span class="sxs-lookup"><span data-stu-id="2e1e2-152">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="2e1e2-153">rank</span><span class="sxs-lookup"><span data-stu-id="2e1e2-153">rank</span></span> |  <span data-ttu-id="2e1e2-154">Int32</span><span class="sxs-lookup"><span data-stu-id="2e1e2-154">Int32</span></span>   |   <span data-ttu-id="2e1e2-155">Pilha da Microsoft de classificação do controle.</span><span class="sxs-lookup"><span data-stu-id="2e1e2-155">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="2e1e2-156">ameaças</span><span class="sxs-lookup"><span data-stu-id="2e1e2-156">threats</span></span> |   <span data-ttu-id="2e1e2-157">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e1e2-157">String Collection</span></span>   |   <span data-ttu-id="2e1e2-158">Lista de ameaças reduz o controle (accountBreach, dataDeletion, dataExfiltration, dataSpillage, elevationOfPrivilege, maliciousInsider, passwordCracking, phishingOrWhaling, falsificação).</span><span class="sxs-lookup"><span data-stu-id="2e1e2-158">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="2e1e2-159">preteridos</span><span class="sxs-lookup"><span data-stu-id="2e1e2-159">deprecated</span></span> |    <span data-ttu-id="2e1e2-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="2e1e2-160">Boolean</span></span> |   <span data-ttu-id="2e1e2-161">Sinalizador para indicar se um controle é depreciado.</span><span class="sxs-lookup"><span data-stu-id="2e1e2-161">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="2e1e2-162">remediação</span><span class="sxs-lookup"><span data-stu-id="2e1e2-162">remediation</span></span> |   <span data-ttu-id="2e1e2-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e1e2-163">String</span></span>  |   <span data-ttu-id="2e1e2-164">Descrição do controle que ajudarão remediar.</span><span class="sxs-lookup"><span data-stu-id="2e1e2-164">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="2e1e2-165">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="2e1e2-165">remediationImpact</span></span> | <span data-ttu-id="2e1e2-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e1e2-166">String</span></span>  |   <span data-ttu-id="2e1e2-167">Descrição do impacto sobre os usuários da remediação.</span><span class="sxs-lookup"><span data-stu-id="2e1e2-167">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="2e1e2-168">actionUrl</span><span class="sxs-lookup"><span data-stu-id="2e1e2-168">actionUrl</span></span> | <span data-ttu-id="2e1e2-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e1e2-169">String</span></span>  |   <span data-ttu-id="2e1e2-170">URL para o qual o controle pode ser actioned.</span><span class="sxs-lookup"><span data-stu-id="2e1e2-170">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="2e1e2-171">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="2e1e2-171">controlStateUpdates</span></span> |   <span data-ttu-id="2e1e2-172">coleção [secureScoreControlStateUpdate](securescorecontrolstateupdate.md)</span><span class="sxs-lookup"><span data-stu-id="2e1e2-172">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)   collection</span></span> |    <span data-ttu-id="2e1e2-173">Sinalizador para indicar onde o inquilino tenha marcado a um controle (Ignorar, thirdParty, examinado) (oferece suporte a [atualização](../api/securescorecontrolprofiles-update.md)).</span><span class="sxs-lookup"><span data-stu-id="2e1e2-173">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |

## <a name="relationships"></a><span data-ttu-id="2e1e2-174">Relações</span><span class="sxs-lookup"><span data-stu-id="2e1e2-174">Relationships</span></span>

<span data-ttu-id="2e1e2-175">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2e1e2-175">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e1e2-176">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2e1e2-176">JSON representation</span></span>

<span data-ttu-id="2e1e2-177">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2e1e2-177">The following is a JSON representation of the resource.</span></span>

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
