---
title: tipo de recurso secureScoreControlProfiles
description: Representa a pontuação segura de um locatário por dados de controle. Por padrão, ele retorna todos os controles de um locatário e pode explicitamente extrair controles individuais.
localization_priority: Normal
ms.openlocfilehash: 3e800271f1ef5f8ac7847d14d97ae6f24f1e01cf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549171"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="eef90-104">tipo de recurso secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="eef90-104">secureScoreControlProfiles resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eef90-105">Representa a pontuação segura de um locatário por dados de controle.</span><span class="sxs-lookup"><span data-stu-id="eef90-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="eef90-106">Por padrão, ele retorna todos os controles de um locatário e pode explicitamente extrair controles individuais.</span><span class="sxs-lookup"><span data-stu-id="eef90-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="eef90-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="eef90-107">Methods</span></span>

| <span data-ttu-id="eef90-108">Método</span><span class="sxs-lookup"><span data-stu-id="eef90-108">Method</span></span>   | <span data-ttu-id="eef90-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eef90-109">Return Type</span></span>|<span data-ttu-id="eef90-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="eef90-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eef90-111">Lista secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="eef90-111">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="eef90-112">secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="eef90-112">secureScoreControlProfiles</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="eef90-113">Leia as propriedades e os metadados de um objeto secureScoreControlProfiles.</span><span class="sxs-lookup"><span data-stu-id="eef90-113">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="eef90-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eef90-114">Properties</span></span>

|<span data-ttu-id="eef90-115">Nome</span><span class="sxs-lookup"><span data-stu-id="eef90-115">Name</span></span> |<span data-ttu-id="eef90-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="eef90-116">Type</span></span> |<span data-ttu-id="eef90-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="eef90-117">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="eef90-118">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="eef90-118">azureTenantId</span></span>   |   <span data-ttu-id="eef90-119">String</span><span class="sxs-lookup"><span data-stu-id="eef90-119">String</span></span>  |   <span data-ttu-id="eef90-120">Cadeia de caracteres GUID para ID do locatário.</span><span class="sxs-lookup"><span data-stu-id="eef90-120">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="eef90-121">controlName</span><span class="sxs-lookup"><span data-stu-id="eef90-121">controlName</span></span> |   <span data-ttu-id="eef90-122">String</span><span class="sxs-lookup"><span data-stu-id="eef90-122">String</span></span>  |   <span data-ttu-id="eef90-123">Nome do controle.</span><span class="sxs-lookup"><span data-stu-id="eef90-123">Name of the control.</span></span> |
|   <span data-ttu-id="eef90-124">title</span><span class="sxs-lookup"><span data-stu-id="eef90-124">title</span></span>   |   <span data-ttu-id="eef90-125">String</span><span class="sxs-lookup"><span data-stu-id="eef90-125">String</span></span>  |   <span data-ttu-id="eef90-126">Título do controle.</span><span class="sxs-lookup"><span data-stu-id="eef90-126">Title of the control.</span></span>   |
| <span data-ttu-id="eef90-127">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="eef90-127">complianceInformation</span></span> | <span data-ttu-id="eef90-128">coleção [complianceInformation](complianceinformation.md)</span><span class="sxs-lookup"><span data-stu-id="eef90-128">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="eef90-129">O conjunto de informações de conformidade associadas ao controle de Pontuação segura</span><span class="sxs-lookup"><span data-stu-id="eef90-129">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="eef90-130">controlCategory</span><span class="sxs-lookup"><span data-stu-id="eef90-130">controlCategory</span></span> |   <span data-ttu-id="eef90-131">String</span><span class="sxs-lookup"><span data-stu-id="eef90-131">String</span></span>  |   <span data-ttu-id="eef90-132">Categoria de ação de controle (conta, dados, dispositivo, aplicativos, infraestrutura).</span><span class="sxs-lookup"><span data-stu-id="eef90-132">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="eef90-133">actionType</span><span class="sxs-lookup"><span data-stu-id="eef90-133">actionType</span></span>  |   <span data-ttu-id="eef90-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eef90-134">String</span></span>  |   <span data-ttu-id="eef90-135">Tipo de ação de controle (configuração, revisão, comportamento).</span><span class="sxs-lookup"><span data-stu-id="eef90-135">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="eef90-136">service</span><span class="sxs-lookup"><span data-stu-id="eef90-136">service</span></span> |   <span data-ttu-id="eef90-137">String</span><span class="sxs-lookup"><span data-stu-id="eef90-137">String</span></span>  |   <span data-ttu-id="eef90-138">Serviço que possui o controle (Exchange, SharePoint, Azure AD).</span><span class="sxs-lookup"><span data-stu-id="eef90-138">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="eef90-139">maxScore</span><span class="sxs-lookup"><span data-stu-id="eef90-139">maxScore</span></span> |  <span data-ttu-id="eef90-140">String</span><span class="sxs-lookup"><span data-stu-id="eef90-140">String</span></span>  |   <span data-ttu-id="eef90-141">A pontuação máxima obtida na data especificada.</span><span class="sxs-lookup"><span data-stu-id="eef90-141">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="eef90-142">camada</span><span class="sxs-lookup"><span data-stu-id="eef90-142">tier</span></span> |  <span data-ttu-id="eef90-143">String</span><span class="sxs-lookup"><span data-stu-id="eef90-143">String</span></span>  |   <span data-ttu-id="eef90-144">Camada de controle (Core, defesa profunda, avançada)</span><span class="sxs-lookup"><span data-stu-id="eef90-144">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="eef90-145">userImpact</span><span class="sxs-lookup"><span data-stu-id="eef90-145">userImpact</span></span> |    <span data-ttu-id="eef90-146">String</span><span class="sxs-lookup"><span data-stu-id="eef90-146">String</span></span>  | <span data-ttu-id="eef90-147">Impacto do usuário da implementação do controle (baixo, moderado, alto).</span><span class="sxs-lookup"><span data-stu-id="eef90-147">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="eef90-148">implementationCost</span><span class="sxs-lookup"><span data-stu-id="eef90-148">implementationCost</span></span> |    <span data-ttu-id="eef90-149">String</span><span class="sxs-lookup"><span data-stu-id="eef90-149">String</span></span>  |   <span data-ttu-id="eef90-150">Custo do recurso do controle implemmentating (baixo, moderado, alto).</span><span class="sxs-lookup"><span data-stu-id="eef90-150">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="eef90-151">classificação</span><span class="sxs-lookup"><span data-stu-id="eef90-151">rank</span></span> |  <span data-ttu-id="eef90-152">Int32</span><span class="sxs-lookup"><span data-stu-id="eef90-152">Int32</span></span>   |   <span data-ttu-id="eef90-153">Classificação de pilha da Microsoft de controle.</span><span class="sxs-lookup"><span data-stu-id="eef90-153">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="eef90-154">las</span><span class="sxs-lookup"><span data-stu-id="eef90-154">threats</span></span> |   <span data-ttu-id="eef90-155">String Collection</span><span class="sxs-lookup"><span data-stu-id="eef90-155">String Collection</span></span>   |   <span data-ttu-id="eef90-156">Lista de ameaças o controle atenua (accountBreach, dataExclusão, dataExfiltration, dataDerramamento, elevationOfPrivilege, maliciousInsider, passwordCracking, phishingOrWhaling, falsificação).</span><span class="sxs-lookup"><span data-stu-id="eef90-156">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="eef90-157">preterido</span><span class="sxs-lookup"><span data-stu-id="eef90-157">deprecated</span></span> |    <span data-ttu-id="eef90-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="eef90-158">Boolean</span></span> |   <span data-ttu-id="eef90-159">Sinalizador para indicar se um controle está depreciado.</span><span class="sxs-lookup"><span data-stu-id="eef90-159">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="eef90-160">correção</span><span class="sxs-lookup"><span data-stu-id="eef90-160">remediation</span></span> |   <span data-ttu-id="eef90-161">String</span><span class="sxs-lookup"><span data-stu-id="eef90-161">String</span></span>  |   <span data-ttu-id="eef90-162">Descrição do que o controle ajudará a corrigir.</span><span class="sxs-lookup"><span data-stu-id="eef90-162">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="eef90-163">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="eef90-163">remediationImpact</span></span> | <span data-ttu-id="eef90-164">String</span><span class="sxs-lookup"><span data-stu-id="eef90-164">String</span></span>  |   <span data-ttu-id="eef90-165">Descrição do impacto sobre os usuários da correção.</span><span class="sxs-lookup"><span data-stu-id="eef90-165">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="eef90-166">actionUrl</span><span class="sxs-lookup"><span data-stu-id="eef90-166">actionUrl</span></span> | <span data-ttu-id="eef90-167">String</span><span class="sxs-lookup"><span data-stu-id="eef90-167">String</span></span>  |   <span data-ttu-id="eef90-168">URL para onde o controle pode ser acionado.</span><span class="sxs-lookup"><span data-stu-id="eef90-168">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="eef90-169">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="eef90-169">controlStateUpdates</span></span> |   <span data-ttu-id="eef90-170">coleção [secureScoreControlStateUpdate](securescorecontrolstateupdate.md)</span><span class="sxs-lookup"><span data-stu-id="eef90-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)   collection</span></span> |    <span data-ttu-id="eef90-171">Sinalizador para indicar onde o locatário marcou um controle (ignore, terceiros, revisado) (suporta [atualização](../api/securescorecontrolprofiles-update.md)).</span><span class="sxs-lookup"><span data-stu-id="eef90-171">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |

## <a name="relationships"></a><span data-ttu-id="eef90-172">Relações</span><span class="sxs-lookup"><span data-stu-id="eef90-172">Relationships</span></span>

<span data-ttu-id="eef90-173">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eef90-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="eef90-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eef90-174">JSON representation</span></span>

<span data-ttu-id="eef90-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eef90-175">The following is a JSON representation of the resource.</span></span>

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
