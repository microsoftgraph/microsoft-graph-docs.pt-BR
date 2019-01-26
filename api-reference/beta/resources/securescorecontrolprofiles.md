---
title: tipo de recurso de secureScoreControlProfiles
description: Representa a pontuação seguro de um locatário por dados do controle. Por padrão, ela retorna todos os controles para um inquilino e explicitamente pode extrair controles individuais.
localization_priority: Normal
ms.openlocfilehash: 4e599bbffd291de51ba478f8661999d01c8c8998
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576056"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="c5110-104">tipo de recurso de secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="c5110-104">secureScoreControlProfiles resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5110-105">Representa a pontuação seguro de um locatário por dados do controle.</span><span class="sxs-lookup"><span data-stu-id="c5110-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="c5110-106">Por padrão, ela retorna todos os controles para um inquilino e explicitamente pode extrair controles individuais.</span><span class="sxs-lookup"><span data-stu-id="c5110-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="c5110-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="c5110-107">Methods</span></span>

| <span data-ttu-id="c5110-108">Método</span><span class="sxs-lookup"><span data-stu-id="c5110-108">Method</span></span>   | <span data-ttu-id="c5110-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c5110-109">Return Type</span></span>|<span data-ttu-id="c5110-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5110-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c5110-111">Lista secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="c5110-111">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="c5110-112">secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="c5110-112">secureScoreControlProfile</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="c5110-113">Leia as propriedades e os metadados de um objeto secureScoreControlProfiles.</span><span class="sxs-lookup"><span data-stu-id="c5110-113">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="c5110-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5110-114">Properties</span></span>

|<span data-ttu-id="c5110-115">Nome</span><span class="sxs-lookup"><span data-stu-id="c5110-115">Name</span></span> |<span data-ttu-id="c5110-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5110-116">Type</span></span> |<span data-ttu-id="c5110-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5110-117">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="c5110-118">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="c5110-118">azureTenantId</span></span>   |   <span data-ttu-id="c5110-119">String</span><span class="sxs-lookup"><span data-stu-id="c5110-119">String</span></span>  |   <span data-ttu-id="c5110-120">ID de cadeia de caracteres do GUID para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="c5110-120">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="c5110-121">controlName</span><span class="sxs-lookup"><span data-stu-id="c5110-121">controlName</span></span> |   <span data-ttu-id="c5110-122">String</span><span class="sxs-lookup"><span data-stu-id="c5110-122">String</span></span>  |   <span data-ttu-id="c5110-123">Nome do controle.</span><span class="sxs-lookup"><span data-stu-id="c5110-123">Name of the control.</span></span> |
|   <span data-ttu-id="c5110-124">title</span><span class="sxs-lookup"><span data-stu-id="c5110-124">title</span></span>   |   <span data-ttu-id="c5110-125">String</span><span class="sxs-lookup"><span data-stu-id="c5110-125">String</span></span>  |   <span data-ttu-id="c5110-126">Título do controle.</span><span class="sxs-lookup"><span data-stu-id="c5110-126">Title of the control.</span></span>   |
|   <span data-ttu-id="c5110-127">controlCategory</span><span class="sxs-lookup"><span data-stu-id="c5110-127">controlCategory</span></span> |   <span data-ttu-id="c5110-128">String</span><span class="sxs-lookup"><span data-stu-id="c5110-128">String</span></span>  |   <span data-ttu-id="c5110-129">Categoria de ação de controle (conta, dados, dispositivo, aplicativos, infra-estrutura).</span><span class="sxs-lookup"><span data-stu-id="c5110-129">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="c5110-130">actionType</span><span class="sxs-lookup"><span data-stu-id="c5110-130">actionType</span></span>  |   <span data-ttu-id="c5110-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5110-131">String</span></span>  |   <span data-ttu-id="c5110-132">Controlar o tipo de ação (Config, revisão, comportamento).</span><span class="sxs-lookup"><span data-stu-id="c5110-132">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="c5110-133">service</span><span class="sxs-lookup"><span data-stu-id="c5110-133">service</span></span> |   <span data-ttu-id="c5110-134">String</span><span class="sxs-lookup"><span data-stu-id="c5110-134">String</span></span>  |   <span data-ttu-id="c5110-135">Serviço que possui o controle (Exchange, Sharepoint, Azure AD).</span><span class="sxs-lookup"><span data-stu-id="c5110-135">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="c5110-136">maxScore</span><span class="sxs-lookup"><span data-stu-id="c5110-136">maxScore</span></span> |  <span data-ttu-id="c5110-137">Duplo</span><span class="sxs-lookup"><span data-stu-id="c5110-137">Double</span></span>  |   <span data-ttu-id="c5110-138">Atual obtidos max pontuação na data especificada.</span><span class="sxs-lookup"><span data-stu-id="c5110-138">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="c5110-139">camada</span><span class="sxs-lookup"><span data-stu-id="c5110-139">tier</span></span> |  <span data-ttu-id="c5110-140">String</span><span class="sxs-lookup"><span data-stu-id="c5110-140">String</span></span>  |   <span data-ttu-id="c5110-141">Camada de controle (Core, defesa em camadas, avançadas.)</span><span class="sxs-lookup"><span data-stu-id="c5110-141">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="c5110-142">userImpact</span><span class="sxs-lookup"><span data-stu-id="c5110-142">userImpact</span></span> |    <span data-ttu-id="c5110-143">String</span><span class="sxs-lookup"><span data-stu-id="c5110-143">String</span></span>  | <span data-ttu-id="c5110-144">Impacto da implementação de controle (baixa, moderada, alta) do usuário.</span><span class="sxs-lookup"><span data-stu-id="c5110-144">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="c5110-145">implementationCost</span><span class="sxs-lookup"><span data-stu-id="c5110-145">implementationCost</span></span> |    <span data-ttu-id="c5110-146">String</span><span class="sxs-lookup"><span data-stu-id="c5110-146">String</span></span>  |   <span data-ttu-id="c5110-147">Custo do recurso de controle de implemmentating (baixa, moderada, alta).</span><span class="sxs-lookup"><span data-stu-id="c5110-147">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="c5110-148">rank</span><span class="sxs-lookup"><span data-stu-id="c5110-148">rank</span></span> |  <span data-ttu-id="c5110-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c5110-149">Int32</span></span>   |   <span data-ttu-id="c5110-150">Pilha da Microsoft de classificação do controle.</span><span class="sxs-lookup"><span data-stu-id="c5110-150">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="c5110-151">ameaças</span><span class="sxs-lookup"><span data-stu-id="c5110-151">threats</span></span> |   <span data-ttu-id="c5110-152">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5110-152">String Collection</span></span>   |   <span data-ttu-id="c5110-153">Lista de ameaças reduz o controle (accountBreach, dataDeletion, dataExfiltration, dataSpillage, elevationOfPrivilege, maliciousInsider, passwordCracking, phishingOrWhaling, falsificação).</span><span class="sxs-lookup"><span data-stu-id="c5110-153">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="c5110-154">preteridos</span><span class="sxs-lookup"><span data-stu-id="c5110-154">deprecated</span></span> |    <span data-ttu-id="c5110-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5110-155">Boolean</span></span> |   <span data-ttu-id="c5110-156">Sinalizador para indicar se um controle é depreciado.</span><span class="sxs-lookup"><span data-stu-id="c5110-156">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="c5110-157">remediação</span><span class="sxs-lookup"><span data-stu-id="c5110-157">remediation</span></span> |   <span data-ttu-id="c5110-158">String</span><span class="sxs-lookup"><span data-stu-id="c5110-158">String</span></span>  |   <span data-ttu-id="c5110-159">Descrição do controle que ajudarão remediar.</span><span class="sxs-lookup"><span data-stu-id="c5110-159">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="c5110-160">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="c5110-160">remediationImpact</span></span> | <span data-ttu-id="c5110-161">String</span><span class="sxs-lookup"><span data-stu-id="c5110-161">String</span></span>  |   <span data-ttu-id="c5110-162">Descrição do impacto sobre os usuários da remediação.</span><span class="sxs-lookup"><span data-stu-id="c5110-162">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="c5110-163">actionUrl</span><span class="sxs-lookup"><span data-stu-id="c5110-163">actionUrl</span></span> | <span data-ttu-id="c5110-164">String</span><span class="sxs-lookup"><span data-stu-id="c5110-164">String</span></span>  |   <span data-ttu-id="c5110-165">URL para o qual o controle pode ser actioned.</span><span class="sxs-lookup"><span data-stu-id="c5110-165">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="c5110-166">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5110-166">lastModifiedDateTime</span></span> |  <span data-ttu-id="c5110-167">Cadeia de caracteres (DateTimeOffset)</span><span class="sxs-lookup"><span data-stu-id="c5110-167">String (DateTimeOffset)</span></span> |   <span data-ttu-id="c5110-168">Data da última modificada</span><span class="sxs-lookup"><span data-stu-id="c5110-168">Date last modified</span></span> |
|   <span data-ttu-id="c5110-169">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="c5110-169">controlStateUpdates</span></span> |   <span data-ttu-id="c5110-170">coleção [secureScoreControlStateUpdate](securescorecontrolstateupdate.md)</span><span class="sxs-lookup"><span data-stu-id="c5110-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection</span></span> |  <span data-ttu-id="c5110-171">Sinalizador para indicar onde o inquilino tenha marcado a um controle (Ignorar, thirdParty, examinado) (oferece suporte a [atualização](../api/securescorecontrolprofiles-update.md)).</span><span class="sxs-lookup"><span data-stu-id="c5110-171">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="c5110-172">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="c5110-172">vendorInformation</span></span> | [<span data-ttu-id="c5110-173">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="c5110-173">securityVendorInformation</span></span>](securityvendorinformation.md) | <span data-ttu-id="c5110-174">Contém detalhes sobre o fornecedor de serviço do produto de segurança, o provedor e subprovider (por exemplo, o fornecedor = Microsoft; provider = ATP do Windows Defender; subProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="c5110-174">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5110-175">Relações</span><span class="sxs-lookup"><span data-stu-id="c5110-175">Relationships</span></span>

<span data-ttu-id="c5110-176">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c5110-176">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5110-177">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5110-177">JSON representation</span></span>

<span data-ttu-id="c5110-178">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c5110-178">The following is a JSON representation of the resource.</span></span>

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
    "referenceId": "String", 
    "controlName": "String", 
    "maxScore": "Double",
    "controlCategory": "string",
    "actionType": "string",
    "service": "String",
    "tier": "string",
    "userImpact": "string",
    "implementationCost ": "string",
    "rank ": "Int32",
    "deprecated ": "Boolean",
    "remediation": "String",
    "remediationImpact ": "String",
    "actionUrl": "String",
    "lastModifiedDateTime": "   String (DateTimeOffset)",
    "controlStateUpdates": [{"odata.type":"microsoft.graph.secureScorecontrolStateUpdates"}],
    "tenantNotes": "String",
    "upn": "String",    
    "vendorInformation" : "microsoft.graph.securityVendorInformation"
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
