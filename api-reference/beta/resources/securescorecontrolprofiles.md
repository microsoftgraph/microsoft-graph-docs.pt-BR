---
title: tipo de recurso de secureScoreControlProfiles
description: Representa a pontuação seguro de um locatário por dados do controle. Por padrão, ela retorna todos os controles para um inquilino e explicitamente pode extrair controles individuais.
localization_priority: Normal
ms.openlocfilehash: 3e800271f1ef5f8ac7847d14d97ae6f24f1e01cf
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641607"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="8c444-104">tipo de recurso de secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="8c444-104">secureScoreControlProfiles resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c444-105">Representa a pontuação seguro de um locatário por dados do controle.</span><span class="sxs-lookup"><span data-stu-id="8c444-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="8c444-106">Por padrão, ela retorna todos os controles para um inquilino e explicitamente pode extrair controles individuais.</span><span class="sxs-lookup"><span data-stu-id="8c444-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="8c444-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="8c444-107">Methods</span></span>

| <span data-ttu-id="8c444-108">Método</span><span class="sxs-lookup"><span data-stu-id="8c444-108">Method</span></span>   | <span data-ttu-id="8c444-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8c444-109">Return Type</span></span>|<span data-ttu-id="8c444-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c444-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8c444-111">Lista secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="8c444-111">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="8c444-112">secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="8c444-112">secureScoreControlProfiles</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="8c444-113">Leia as propriedades e os metadados de um objeto secureScoreControlProfiles.</span><span class="sxs-lookup"><span data-stu-id="8c444-113">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="8c444-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8c444-114">Properties</span></span>

|<span data-ttu-id="8c444-115">Nome</span><span class="sxs-lookup"><span data-stu-id="8c444-115">Name</span></span> |<span data-ttu-id="8c444-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c444-116">Type</span></span> |<span data-ttu-id="8c444-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c444-117">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="8c444-118">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="8c444-118">azureTenantId</span></span>   |   <span data-ttu-id="8c444-119">String</span><span class="sxs-lookup"><span data-stu-id="8c444-119">String</span></span>  |   <span data-ttu-id="8c444-120">ID de cadeia de caracteres do GUID para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="8c444-120">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="8c444-121">controlName</span><span class="sxs-lookup"><span data-stu-id="8c444-121">controlName</span></span> |   <span data-ttu-id="8c444-122">String</span><span class="sxs-lookup"><span data-stu-id="8c444-122">String</span></span>  |   <span data-ttu-id="8c444-123">Nome do controle.</span><span class="sxs-lookup"><span data-stu-id="8c444-123">Name of the control.</span></span> |
|   <span data-ttu-id="8c444-124">title</span><span class="sxs-lookup"><span data-stu-id="8c444-124">title</span></span>   |   <span data-ttu-id="8c444-125">String</span><span class="sxs-lookup"><span data-stu-id="8c444-125">String</span></span>  |   <span data-ttu-id="8c444-126">Título do controle.</span><span class="sxs-lookup"><span data-stu-id="8c444-126">Title of the control.</span></span>   |
| <span data-ttu-id="8c444-127">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="8c444-127">complianceInformation</span></span> | <span data-ttu-id="8c444-128">coleção [complianceInformation](complianceinformation.md)</span><span class="sxs-lookup"><span data-stu-id="8c444-128">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="8c444-129">A coleção de informações de conformidade associadas a proteger o controle de pontuação</span><span class="sxs-lookup"><span data-stu-id="8c444-129">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="8c444-130">controlCategory</span><span class="sxs-lookup"><span data-stu-id="8c444-130">controlCategory</span></span> |   <span data-ttu-id="8c444-131">String</span><span class="sxs-lookup"><span data-stu-id="8c444-131">String</span></span>  |   <span data-ttu-id="8c444-132">Categoria de ação de controle (conta, dados, dispositivo, aplicativos, infra-estrutura).</span><span class="sxs-lookup"><span data-stu-id="8c444-132">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="8c444-133">actionType</span><span class="sxs-lookup"><span data-stu-id="8c444-133">actionType</span></span>  |   <span data-ttu-id="8c444-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c444-134">String</span></span>  |   <span data-ttu-id="8c444-135">Controlar o tipo de ação (Config, revisão, comportamento).</span><span class="sxs-lookup"><span data-stu-id="8c444-135">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="8c444-136">service</span><span class="sxs-lookup"><span data-stu-id="8c444-136">service</span></span> |   <span data-ttu-id="8c444-137">String</span><span class="sxs-lookup"><span data-stu-id="8c444-137">String</span></span>  |   <span data-ttu-id="8c444-138">Serviço que possui o controle (Exchange, Sharepoint, Azure AD).</span><span class="sxs-lookup"><span data-stu-id="8c444-138">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="8c444-139">maxScore</span><span class="sxs-lookup"><span data-stu-id="8c444-139">maxScore</span></span> |  <span data-ttu-id="8c444-140">String</span><span class="sxs-lookup"><span data-stu-id="8c444-140">String</span></span>  |   <span data-ttu-id="8c444-141">Atual obtidos max pontuação na data especificada.</span><span class="sxs-lookup"><span data-stu-id="8c444-141">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="8c444-142">camada</span><span class="sxs-lookup"><span data-stu-id="8c444-142">tier</span></span> |  <span data-ttu-id="8c444-143">String</span><span class="sxs-lookup"><span data-stu-id="8c444-143">String</span></span>  |   <span data-ttu-id="8c444-144">Camada de controle (Core, defesa em camadas, avançadas.)</span><span class="sxs-lookup"><span data-stu-id="8c444-144">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="8c444-145">userImpact</span><span class="sxs-lookup"><span data-stu-id="8c444-145">userImpact</span></span> |    <span data-ttu-id="8c444-146">String</span><span class="sxs-lookup"><span data-stu-id="8c444-146">String</span></span>  | <span data-ttu-id="8c444-147">Impacto da implementação de controle (baixa, moderada, alta) do usuário.</span><span class="sxs-lookup"><span data-stu-id="8c444-147">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="8c444-148">implementationCost</span><span class="sxs-lookup"><span data-stu-id="8c444-148">implementationCost</span></span> |    <span data-ttu-id="8c444-149">String</span><span class="sxs-lookup"><span data-stu-id="8c444-149">String</span></span>  |   <span data-ttu-id="8c444-150">Custo do recurso de controle de implemmentating (baixa, moderada, alta).</span><span class="sxs-lookup"><span data-stu-id="8c444-150">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="8c444-151">rank</span><span class="sxs-lookup"><span data-stu-id="8c444-151">rank</span></span> |  <span data-ttu-id="8c444-152">Int32</span><span class="sxs-lookup"><span data-stu-id="8c444-152">Int32</span></span>   |   <span data-ttu-id="8c444-153">Pilha da Microsoft de classificação do controle.</span><span class="sxs-lookup"><span data-stu-id="8c444-153">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="8c444-154">ameaças</span><span class="sxs-lookup"><span data-stu-id="8c444-154">threats</span></span> |   <span data-ttu-id="8c444-155">String Collection</span><span class="sxs-lookup"><span data-stu-id="8c444-155">String Collection</span></span>   |   <span data-ttu-id="8c444-156">Lista de ameaças reduz o controle (accountBreach, dataDeletion, dataExfiltration, dataSpillage, elevationOfPrivilege, maliciousInsider, passwordCracking, phishingOrWhaling, falsificação).</span><span class="sxs-lookup"><span data-stu-id="8c444-156">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="8c444-157">preteridos</span><span class="sxs-lookup"><span data-stu-id="8c444-157">deprecated</span></span> |    <span data-ttu-id="8c444-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="8c444-158">Boolean</span></span> |   <span data-ttu-id="8c444-159">Sinalizador para indicar se um controle é depreciado.</span><span class="sxs-lookup"><span data-stu-id="8c444-159">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="8c444-160">remediação</span><span class="sxs-lookup"><span data-stu-id="8c444-160">remediation</span></span> |   <span data-ttu-id="8c444-161">String</span><span class="sxs-lookup"><span data-stu-id="8c444-161">String</span></span>  |   <span data-ttu-id="8c444-162">Descrição do controle que ajudarão remediar.</span><span class="sxs-lookup"><span data-stu-id="8c444-162">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="8c444-163">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="8c444-163">remediationImpact</span></span> | <span data-ttu-id="8c444-164">String</span><span class="sxs-lookup"><span data-stu-id="8c444-164">String</span></span>  |   <span data-ttu-id="8c444-165">Descrição do impacto sobre os usuários da remediação.</span><span class="sxs-lookup"><span data-stu-id="8c444-165">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="8c444-166">actionUrl</span><span class="sxs-lookup"><span data-stu-id="8c444-166">actionUrl</span></span> | <span data-ttu-id="8c444-167">String</span><span class="sxs-lookup"><span data-stu-id="8c444-167">String</span></span>  |   <span data-ttu-id="8c444-168">URL para o qual o controle pode ser actioned.</span><span class="sxs-lookup"><span data-stu-id="8c444-168">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="8c444-169">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="8c444-169">controlStateUpdates</span></span> |   <span data-ttu-id="8c444-170">coleção [secureScoreControlStateUpdate](securescorecontrolstateupdate.md)</span><span class="sxs-lookup"><span data-stu-id="8c444-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)   collection</span></span> |    <span data-ttu-id="8c444-171">Sinalizador para indicar onde o inquilino tenha marcado a um controle (Ignorar, thirdParty, examinado) (oferece suporte a [atualização](../api/securescorecontrolprofiles-update.md)).</span><span class="sxs-lookup"><span data-stu-id="8c444-171">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |

## <a name="relationships"></a><span data-ttu-id="8c444-172">Relações</span><span class="sxs-lookup"><span data-stu-id="8c444-172">Relationships</span></span>

<span data-ttu-id="8c444-173">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8c444-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c444-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8c444-174">JSON representation</span></span>

<span data-ttu-id="8c444-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8c444-175">The following is a JSON representation of the resource.</span></span>

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


<!--
{
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securescorecontrolprofiles.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
