---
title: tipo de recurso riskDetection
description: Representa todas as detecções de riscos em locatários do AzureAD.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 78dac11af0168b6981e98688536064e9cbc5f528
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938727"
---
# <a name="riskdetection-resource-type"></a><span data-ttu-id="48ddf-103">tipo de recurso riskDetection</span><span class="sxs-lookup"><span data-stu-id="48ddf-103">riskDetection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48ddf-104">Representa informações sobre um risco detectado em um locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="48ddf-104">Represents information about a detected risk in an Azure AD tenant.</span></span> 

<span data-ttu-id="48ddf-105">O Azure AD avalia continuamente [os riscos do usuário](riskyuser.md) e os riscos de [entrada do](signin.md) aplicativo ou do usuário com base em vários sinais e aprendizado de máquina.</span><span class="sxs-lookup"><span data-stu-id="48ddf-105">Azure AD continually evaluates [user risks](riskyuser.md) and app or user [sign-in](signin.md) risks based on various signals and machine learning.</span></span> <span data-ttu-id="48ddf-106">Essa API fornece acesso programático a todas as detecções de risco em seu ambiente do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="48ddf-106">This API provides programmatic access to all risk detections in your Azure AD environment.</span></span>

<span data-ttu-id="48ddf-107">Para obter mais informações sobre eventos de risco, consulte [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="48ddf-107">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).</span></span>

>[!NOTE]
><span data-ttu-id="48ddf-108">Você deve ter uma licença do Azure AD Premium P1 ou P2 para usar a API de detecção de risco.</span><span class="sxs-lookup"><span data-stu-id="48ddf-108">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="methods"></a><span data-ttu-id="48ddf-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="48ddf-109">Methods</span></span>

| <span data-ttu-id="48ddf-110">Método</span><span class="sxs-lookup"><span data-stu-id="48ddf-110">Method</span></span>   | <span data-ttu-id="48ddf-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="48ddf-111">Return Type</span></span>|<span data-ttu-id="48ddf-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="48ddf-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="48ddf-113">Listar riskDetection</span><span class="sxs-lookup"><span data-stu-id="48ddf-113">List riskDetection</span></span>](../api/riskdetection-list.md) | <span data-ttu-id="48ddf-114">coleção [riskDetection](riskdetection.md)</span><span class="sxs-lookup"><span data-stu-id="48ddf-114">[riskDetection](riskdetection.md) collection</span></span>|<span data-ttu-id="48ddf-115">Listar detecções de risco e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="48ddf-115">List risk detections and their properties.</span></span>|
|[<span data-ttu-id="48ddf-116">Obter riskDetection</span><span class="sxs-lookup"><span data-stu-id="48ddf-116">Get riskDetection</span></span>](../api/riskdetection-get.md) | [<span data-ttu-id="48ddf-117">riskDetection</span><span class="sxs-lookup"><span data-stu-id="48ddf-117">riskDetection</span></span>](riskdetection.md)|<span data-ttu-id="48ddf-118">Obtenha uma detecção arriscada específica e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="48ddf-118">Get a specific risky detection and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="48ddf-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48ddf-119">Properties</span></span>

| <span data-ttu-id="48ddf-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48ddf-120">Property</span></span>   | <span data-ttu-id="48ddf-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="48ddf-121">Type</span></span>|<span data-ttu-id="48ddf-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="48ddf-122">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="48ddf-123">ID exclusiva da detecção de risco.</span><span class="sxs-lookup"><span data-stu-id="48ddf-123">Unique ID of the risk detection.</span></span> |
|`requestId`|`string`|<span data-ttu-id="48ddf-124">ID de solicitação da entrada associada à detecção de risco.</span><span class="sxs-lookup"><span data-stu-id="48ddf-124">Request ID of the sign-in associated with the risk detection.</span></span> <span data-ttu-id="48ddf-125">Essa propriedade será NULL se a detecção de risco não estiver associada a uma entrada.</span><span class="sxs-lookup"><span data-stu-id="48ddf-125">This property is null if the risk detection is not associated with a sign-in.</span></span>|
|`correlationId`|`string`|<span data-ttu-id="48ddf-126">ID de correlação da entrada associada à detecção de risco.</span><span class="sxs-lookup"><span data-stu-id="48ddf-126">Correlation ID of the sign-in associated with the risk detection.</span></span> <span data-ttu-id="48ddf-127">Essa propriedade será NULL se a detecção de risco não estiver associada a uma entrada.</span><span class="sxs-lookup"><span data-stu-id="48ddf-127">This property is null if the risk detection is not associated with a sign-in.</span></span> |
|`riskType`|`riskEventType`|<span data-ttu-id="48ddf-128">O tipo de evento de risco detectado.</span><span class="sxs-lookup"><span data-stu-id="48ddf-128">The type of risk event detected.</span></span> <span data-ttu-id="48ddf-129">Os valores possíveis são unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, genericadminConfirmedUserCompromised , mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP e unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="48ddf-129">The possible values are unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, genericadminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, and unknownFutureValue.</span></span> |
|`riskState`|`riskState`|<span data-ttu-id="48ddf-130">O estado de um usuário ou logon arriscado detectado.</span><span class="sxs-lookup"><span data-stu-id="48ddf-130">The state of a detected risky user or sign-in.</span></span> <span data-ttu-id="48ddf-131">Os valores possíveis são nenhum, confirmedSafe, corrigido, descartado, atRisk, confirmedCompromised e unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="48ddf-131">The possible values are none, confirmedSafe, remediated, dismissed, atRisk, confirmedCompromised, and unknownFutureValue.</span></span> |
|`riskLevel`|`riskLevel`|<span data-ttu-id="48ddf-132">Nível do risco detectado.</span><span class="sxs-lookup"><span data-stu-id="48ddf-132">Level of the detected risk.</span></span> <span data-ttu-id="48ddf-133">Os valores possíveis são baixo, médio, alto, oculto, nenhum, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="48ddf-133">The possible values are low, medium, high, hidden, none, unknownFutureValue.</span></span> <span data-ttu-id="48ddf-134">**Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="48ddf-134">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="48ddf-135">Os clientes P1 serão retornados `hidden`.</span><span class="sxs-lookup"><span data-stu-id="48ddf-135">P1 customers will be returned `hidden`.</span></span>|
|`riskDetail`|`riskDetail`|<span data-ttu-id="48ddf-136">Detalhes do risco detectado.</span><span class="sxs-lookup"><span data-stu-id="48ddf-136">Details of the detected risk.</span></span> <span data-ttu-id="48ddf-137">Os valores possíveis são None, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, oculto, adminConfirmedUserCompromised, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="48ddf-137">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span> <span data-ttu-id="48ddf-138">**Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="48ddf-138">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="48ddf-139">Os clientes P1 serão retornados `hidden`.</span><span class="sxs-lookup"><span data-stu-id="48ddf-139">P1 customers will be returned `hidden`.</span></span>|
|`source`|`string`|<span data-ttu-id="48ddf-140">Fonte da detecção de risco.</span><span class="sxs-lookup"><span data-stu-id="48ddf-140">Source of the risk detection.</span></span> <span data-ttu-id="48ddf-141">Por exemplo, "activeDirectory".</span><span class="sxs-lookup"><span data-stu-id="48ddf-141">For example, "activeDirectory".</span></span> |
|`detectionTimingType`|`riskDetectionTimingType`|<span data-ttu-id="48ddf-142">Intervalo do risco detectado (em tempo real/offline).</span><span class="sxs-lookup"><span data-stu-id="48ddf-142">Timing of the detected risk (real-time/offline).</span></span> <span data-ttu-id="48ddf-143">Os valores possíveis são não definidos, em tempo real, nearRealtime, offline, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="48ddf-143">The possible values are notDefined, realtime, nearRealtime, offline, unknownFutureValue.</span></span> |
|`activity`|`activityType`|<span data-ttu-id="48ddf-144">Indica o tipo de atividade ao qual o risco detectado está vinculado.</span><span class="sxs-lookup"><span data-stu-id="48ddf-144">Indicates the activity type the detected risk is linked to.</span></span> <span data-ttu-id="48ddf-145">Os valores possíveis são entrar, User, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="48ddf-145">The possible values are signin, user, unknownFutureValue.</span></span> |
|`tokenIssuerType`|`tokenIssuerType`|<span data-ttu-id="48ddf-146">Indica o tipo de emissor de token para o risco de entrada detectado.</span><span class="sxs-lookup"><span data-stu-id="48ddf-146">Indicates the type of token issuer for the detected sign-in risk.</span></span> <span data-ttu-id="48ddf-147">Os valores possíveis são AzureAD, ADFederationServices e unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="48ddf-147">The possible values are AzureAD, ADFederationServices, and unknownFutureValue.</span></span> |
|`ipAddress`|`string`|<span data-ttu-id="48ddf-148">Fornece o endereço IP do cliente de onde o risco ocorreu.</span><span class="sxs-lookup"><span data-stu-id="48ddf-148">Provides the IP address of the client from where the risk occurred.</span></span> |
|`location`|[`signInLocation`](signinlocation.md)|<span data-ttu-id="48ddf-149">Local de entrada.</span><span class="sxs-lookup"><span data-stu-id="48ddf-149">Location of the sign-in.</span></span> |
|`activityDateTime`|`datetimeoffset`|<span data-ttu-id="48ddf-150">Data e hora em que a atividade arriscada ocorreu.</span><span class="sxs-lookup"><span data-stu-id="48ddf-150">Date and time that the risky activity occurred.</span></span> |
|`detectedDateTime`|`datetimeoffset`|<span data-ttu-id="48ddf-151">Data e hora em que o risco foi detectado.</span><span class="sxs-lookup"><span data-stu-id="48ddf-151">Date and time that the risk was detected.</span></span> |
|`lastUpdatedDateTime`|`datetime`|<span data-ttu-id="48ddf-152">Data e hora da última atualização do risco.</span><span class="sxs-lookup"><span data-stu-id="48ddf-152">Date and time that the risk detection was last updated.</span></span> |
|`userId`|`string`|<span data-ttu-id="48ddf-153">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="48ddf-153">Unique ID of the user.</span></span> |
|`userDisplayName`|`string`|<span data-ttu-id="48ddf-154">Nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="48ddf-154">Name of the user.</span></span> |
|`userPrincipalName`|`string`|<span data-ttu-id="48ddf-155">O nome UPN do usuário.</span><span class="sxs-lookup"><span data-stu-id="48ddf-155">The user principal name (UPN) of the user.</span></span> |
|`additionalInfo`|`string`|<span data-ttu-id="48ddf-156">Informações adicionais associadas à detecção de riscos no formato JSON.</span><span class="sxs-lookup"><span data-stu-id="48ddf-156">Additional information associated with the risk detection in JSON format.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="48ddf-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48ddf-157">JSON representation</span></span>

<span data-ttu-id="48ddf-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="48ddf-158">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskDetection"
}-->

```json
{
 "id": "string",
    "requestId": "string",
    "correlationId": "string",
    "riskType": {"@odata.type": "microsoft.graph.riskEventType"},
    "riskState": {"@odata.type": "microsoft.graph.riskState"},
    "riskLevel": {"@odata.type": "microsoft.graph.riskLevel"},
    "riskDetail": {"@odata.type": "microsoft.graph.riskDetail"},
    "source": "string",
    "detectionTimingType": {"@odata.type": "microsoft.graph.riskDetectionTimingType"},
    "activity": {"@odata.type": "microsoft.graph.riskUserActivity"},
    "tokenIssuerType": {"@odata.type": "microsoft.graph.tokenIssuerType"},
    "ipAddress": "string",
    "location": {"@odata.type": "microsoft.graph.signInLocation"},
    "activityDateTime": "string (timestamp)",
    "detectedDateTime": "string (timestamp)",
    "lastUpdatedDateTime": "string (timestamp)",
    "userId": "string",
    "userDisplayName": "string",
    "userPrincipalName": "string",
    "additionalInfo": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskDetections resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
