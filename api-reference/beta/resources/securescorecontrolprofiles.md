---
title: tipo de recurso de secureScoreControlProfiles
description: Representa a pontuação seguro de um locatário por dados do controle. Por padrão, ela retorna todos os controles para um inquilino e explicitamente pode extrair controles individuais.
ms.openlocfilehash: 3e7dc463d7521e1980b41034ae4121ab610dd8f5
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380580"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="f2384-104">tipo de recurso de secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="f2384-104">secureScoreControlProfiles resource type</span></span>

> <span data-ttu-id="f2384-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f2384-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2384-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f2384-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f2384-107">Representa a pontuação seguro de um locatário por dados do controle.</span><span class="sxs-lookup"><span data-stu-id="f2384-107">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="f2384-108">Por padrão, ela retorna todos os controles para um inquilino e explicitamente pode extrair controles individuais.</span><span class="sxs-lookup"><span data-stu-id="f2384-108">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="f2384-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="f2384-109">Methods</span></span>

| <span data-ttu-id="f2384-110">Método		</span><span class="sxs-lookup"><span data-stu-id="f2384-110">Method</span></span>   | <span data-ttu-id="f2384-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f2384-111">Return Type</span></span>|<span data-ttu-id="f2384-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2384-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f2384-113">Lista secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="f2384-113">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="f2384-114">secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="f2384-114">secureScoreControlProfiles</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="f2384-115">Leia as propriedades e os metadados de um objeto secureScoreControlProfiles.</span><span class="sxs-lookup"><span data-stu-id="f2384-115">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="f2384-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2384-116">Properties</span></span>

|<span data-ttu-id="f2384-117">Nome</span><span class="sxs-lookup"><span data-stu-id="f2384-117">Name</span></span> |<span data-ttu-id="f2384-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2384-118">Type</span></span> |<span data-ttu-id="f2384-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2384-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="f2384-120">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="f2384-120">azureTenantId</span></span>   |   <span data-ttu-id="f2384-121">String</span><span class="sxs-lookup"><span data-stu-id="f2384-121">String</span></span>  |   <span data-ttu-id="f2384-122">ID de cadeia de caracteres do GUID para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f2384-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="f2384-123">controlName</span><span class="sxs-lookup"><span data-stu-id="f2384-123">controlName</span></span> |   <span data-ttu-id="f2384-124">String</span><span class="sxs-lookup"><span data-stu-id="f2384-124">String</span></span>  |   <span data-ttu-id="f2384-125">Nome do controle.</span><span class="sxs-lookup"><span data-stu-id="f2384-125">Name of the control.</span></span> |
|   <span data-ttu-id="f2384-126">title</span><span class="sxs-lookup"><span data-stu-id="f2384-126">title</span></span>   |   <span data-ttu-id="f2384-127">String</span><span class="sxs-lookup"><span data-stu-id="f2384-127">String</span></span>  |   <span data-ttu-id="f2384-128">Título do controle.</span><span class="sxs-lookup"><span data-stu-id="f2384-128">Title of the control.</span></span>   |
| <span data-ttu-id="f2384-129">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="f2384-129">complianceInformation</span></span> | <span data-ttu-id="f2384-130">coleção [complianceInformation](complianceinformation.md)</span><span class="sxs-lookup"><span data-stu-id="f2384-130">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="f2384-131">A coleção de informações de conformidade associadas a proteger o controle de pontuação</span><span class="sxs-lookup"><span data-stu-id="f2384-131">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="f2384-132">controlCategory</span><span class="sxs-lookup"><span data-stu-id="f2384-132">controlCategory</span></span> |   <span data-ttu-id="f2384-133">String</span><span class="sxs-lookup"><span data-stu-id="f2384-133">String</span></span>  |   <span data-ttu-id="f2384-134">Categoria de ação de controle (conta, dados, dispositivo, aplicativos, infra-estrutura).</span><span class="sxs-lookup"><span data-stu-id="f2384-134">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="f2384-135">actionType</span><span class="sxs-lookup"><span data-stu-id="f2384-135">actionType</span></span>  |   <span data-ttu-id="f2384-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2384-136">String</span></span>  |   <span data-ttu-id="f2384-137">Controlar o tipo de ação (Config, revisão, comportamento).</span><span class="sxs-lookup"><span data-stu-id="f2384-137">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="f2384-138">service</span><span class="sxs-lookup"><span data-stu-id="f2384-138">service</span></span> |   <span data-ttu-id="f2384-139">String</span><span class="sxs-lookup"><span data-stu-id="f2384-139">String</span></span>  |   <span data-ttu-id="f2384-140">Serviço que possui o controle (Exchange, Sharepoint, Azure AD).</span><span class="sxs-lookup"><span data-stu-id="f2384-140">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="f2384-141">maxScore</span><span class="sxs-lookup"><span data-stu-id="f2384-141">maxScore</span></span> |  <span data-ttu-id="f2384-142">String</span><span class="sxs-lookup"><span data-stu-id="f2384-142">String</span></span>  |   <span data-ttu-id="f2384-143">Atual obtidos max pontuação na data especificada.</span><span class="sxs-lookup"><span data-stu-id="f2384-143">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="f2384-144">camada</span><span class="sxs-lookup"><span data-stu-id="f2384-144">tier</span></span> |  <span data-ttu-id="f2384-145">String</span><span class="sxs-lookup"><span data-stu-id="f2384-145">String</span></span>  |   <span data-ttu-id="f2384-146">Camada de controle (Core, defesa em camadas, avançadas.)</span><span class="sxs-lookup"><span data-stu-id="f2384-146">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="f2384-147">userImpact</span><span class="sxs-lookup"><span data-stu-id="f2384-147">userImpact</span></span> |    <span data-ttu-id="f2384-148">String</span><span class="sxs-lookup"><span data-stu-id="f2384-148">String</span></span>  | <span data-ttu-id="f2384-149">Impacto da implementação de controle (baixa, moderada, alta) do usuário.</span><span class="sxs-lookup"><span data-stu-id="f2384-149">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="f2384-150">implementationCost</span><span class="sxs-lookup"><span data-stu-id="f2384-150">implementationCost</span></span> |    <span data-ttu-id="f2384-151">String</span><span class="sxs-lookup"><span data-stu-id="f2384-151">String</span></span>  |   <span data-ttu-id="f2384-152">Custo do recurso de controle de implemmentating (baixa, moderada, alta).</span><span class="sxs-lookup"><span data-stu-id="f2384-152">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="f2384-153">rank</span><span class="sxs-lookup"><span data-stu-id="f2384-153">rank</span></span> |  <span data-ttu-id="f2384-154">Int32</span><span class="sxs-lookup"><span data-stu-id="f2384-154">Int32</span></span>   |   <span data-ttu-id="f2384-155">Pilha da Microsoft de classificação do controle.</span><span class="sxs-lookup"><span data-stu-id="f2384-155">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="f2384-156">ameaças</span><span class="sxs-lookup"><span data-stu-id="f2384-156">threats</span></span> |   <span data-ttu-id="f2384-157">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2384-157">String Collection</span></span>   |   <span data-ttu-id="f2384-158">Lista de ameaças reduz o controle (accountBreach, dataDeletion, dataExfiltration, dataSpillage, elevationOfPrivilege, maliciousInsider, passwordCracking, phishingOrWhaling, falsificação).</span><span class="sxs-lookup"><span data-stu-id="f2384-158">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="f2384-159">preteridos</span><span class="sxs-lookup"><span data-stu-id="f2384-159">deprecated</span></span> |    <span data-ttu-id="f2384-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="f2384-160">Boolean</span></span> |   <span data-ttu-id="f2384-161">Sinalizador para indicar se um controle é depreciado.</span><span class="sxs-lookup"><span data-stu-id="f2384-161">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="f2384-162">remediação</span><span class="sxs-lookup"><span data-stu-id="f2384-162">remediation</span></span> |   <span data-ttu-id="f2384-163">String</span><span class="sxs-lookup"><span data-stu-id="f2384-163">String</span></span>  |   <span data-ttu-id="f2384-164">Descrição do controle que ajudarão remediar.</span><span class="sxs-lookup"><span data-stu-id="f2384-164">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="f2384-165">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="f2384-165">remediationImpact</span></span> | <span data-ttu-id="f2384-166">String</span><span class="sxs-lookup"><span data-stu-id="f2384-166">String</span></span>  |   <span data-ttu-id="f2384-167">Descrição do impacto sobre os usuários da remediação.</span><span class="sxs-lookup"><span data-stu-id="f2384-167">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="f2384-168">actionUrl</span><span class="sxs-lookup"><span data-stu-id="f2384-168">actionUrl</span></span> | <span data-ttu-id="f2384-169">String</span><span class="sxs-lookup"><span data-stu-id="f2384-169">String</span></span>  |   <span data-ttu-id="f2384-170">URL para o qual o controle pode ser actioned.</span><span class="sxs-lookup"><span data-stu-id="f2384-170">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="f2384-171">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="f2384-171">controlStateUpdates</span></span> |   <span data-ttu-id="f2384-172">coleção [secureScoreControlStateUpdate](securescorecontrolstateupdate.md)</span><span class="sxs-lookup"><span data-stu-id="f2384-172">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)   collection</span></span> |    <span data-ttu-id="f2384-173">Sinalizador para indicar onde o inquilino tenha marcado a um controle (Ignorar, thirdParty, examinado) (oferece suporte a [atualização](../api/securescorecontrolprofiles-update.md)).</span><span class="sxs-lookup"><span data-stu-id="f2384-173">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |

## <a name="relationships"></a><span data-ttu-id="f2384-174">Relações</span><span class="sxs-lookup"><span data-stu-id="f2384-174">Relationships</span></span>

<span data-ttu-id="f2384-175">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f2384-175">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2384-176">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2384-176">JSON representation</span></span>

<span data-ttu-id="f2384-177">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f2384-177">The following is a JSON representation of the resource.</span></span>

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
