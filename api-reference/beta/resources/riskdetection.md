---
title: Tipo de recurso riskDetection
description: Representa todas as detecções de risco em locatários do AzureAD.
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 40fa938f94f5f43a61c191a3d3c14b0dbbb10d6f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440133"
---
# <a name="riskdetection-resource-type"></a><span data-ttu-id="f4e8c-103">Tipo de recurso riskDetection</span><span class="sxs-lookup"><span data-stu-id="f4e8c-103">riskDetection resource type</span></span>

<span data-ttu-id="f4e8c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4e8c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4e8c-105">Representa informações sobre um risco detectado em um locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-105">Represents information about a detected risk in an Azure AD tenant.</span></span> 

<span data-ttu-id="f4e8c-106">O Azure AD [](riskyuser.md) avalia continuamente os [](signin.md) riscos do usuário e os riscos de entrada de aplicativo ou usuário com base em vários sinais e aprendizado de máquina.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-106">Azure AD continually evaluates [user risks](riskyuser.md) and app or user [sign-in](signin.md) risks based on various signals and machine learning.</span></span> <span data-ttu-id="f4e8c-107">Essa API fornece acesso programático a todas as detecções de risco em seu ambiente do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-107">This API provides programmatic access to all risk detections in your Azure AD environment.</span></span>

<span data-ttu-id="f4e8c-108">Para obter mais informações sobre eventos de risco, consulte [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span><span class="sxs-lookup"><span data-stu-id="f4e8c-108">For more information about risk events, see [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>

>[!NOTE]
><span data-ttu-id="f4e8c-109">Você deve ter uma licença do Azure AD Premium P1 ou P2 para usar a API de detecção de riscos.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-109">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="methods"></a><span data-ttu-id="f4e8c-110">Methods</span><span class="sxs-lookup"><span data-stu-id="f4e8c-110">Methods</span></span>

| <span data-ttu-id="f4e8c-111">Método</span><span class="sxs-lookup"><span data-stu-id="f4e8c-111">Method</span></span>   | <span data-ttu-id="f4e8c-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f4e8c-112">Return Type</span></span>|<span data-ttu-id="f4e8c-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4e8c-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f4e8c-114">Listar riskDetection</span><span class="sxs-lookup"><span data-stu-id="f4e8c-114">List riskDetection</span></span>](../api/riskdetection-list.md) | <span data-ttu-id="f4e8c-115">[Coleção riskDetection](riskdetection.md)</span><span class="sxs-lookup"><span data-stu-id="f4e8c-115">[riskDetection](riskdetection.md) collection</span></span>|<span data-ttu-id="f4e8c-116">Listar detecções de risco e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-116">List risk detections and their properties.</span></span>|
|[<span data-ttu-id="f4e8c-117">Obter riskDetection</span><span class="sxs-lookup"><span data-stu-id="f4e8c-117">Get riskDetection</span></span>](../api/riskdetection-get.md) | [<span data-ttu-id="f4e8c-118">riskDetection</span><span class="sxs-lookup"><span data-stu-id="f4e8c-118">riskDetection</span></span>](riskdetection.md)|<span data-ttu-id="f4e8c-119">Obter uma detecção arriscada específica e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-119">Get a specific risky detection and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="f4e8c-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4e8c-120">Properties</span></span>

| <span data-ttu-id="f4e8c-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4e8c-121">Property</span></span>   | <span data-ttu-id="f4e8c-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4e8c-122">Type</span></span>|<span data-ttu-id="f4e8c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4e8c-123">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="f4e8c-124">ID exclusiva da detecção de risco.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-124">Unique ID of the risk detection.</span></span> |
|`requestId`|`string`|<span data-ttu-id="f4e8c-125">ID da solicitação da login associada à detecção de risco.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-125">Request ID of the sign-in associated with the risk detection.</span></span> <span data-ttu-id="f4e8c-126">Essa propriedade será nula se a detecção de risco não estiver associada a uma login.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-126">This property is null if the risk detection is not associated with a sign-in.</span></span>|
|`correlationId`|`string`|<span data-ttu-id="f4e8c-127">ID de correlação do sign-in associado à detecção de risco.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-127">Correlation ID of the sign-in associated with the risk detection.</span></span> <span data-ttu-id="f4e8c-128">Essa propriedade será nula se a detecção de risco não estiver associada a uma login.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-128">This property is null if the risk detection is not associated with a sign-in.</span></span> |
|`riskEventType`|`string`|<span data-ttu-id="f4e8c-129">O tipo de evento de risco detectado.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-129">The type of risk event detected.</span></span> <span data-ttu-id="f4e8c-130">Os valores possíveis `unlikelyTravel` são , , , , , , , `anonymizedIPAddress` , , , , `maliciousIPAddress` , , `unfamiliarFeatures` , , `malwareInfectedIPAddress` e `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="f4e8c-130">The possible values are `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `genericadminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, and `unknownFutureValue`.</span></span> |
|`riskType`|`riskEventType`|<span data-ttu-id="f4e8c-131">Lista de tipos de eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-131">List of risk event types.</span></span><br/><span data-ttu-id="f4e8c-132">**Observação:** Essa propriedade é preterida.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-132">**Note:** This property is deprecated.</span></span> <span data-ttu-id="f4e8c-133">Use **riskEventTypes** em vez disso.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-133">Use **riskEventTypes** instead.</span></span> |
|`riskState`|`riskState`|<span data-ttu-id="f4e8c-134">O estado de um usuário ou de login de risco detectado.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-134">The state of a detected risky user or sign-in.</span></span> <span data-ttu-id="f4e8c-135">Os valores possíveis são none, confirmedSafe, remediado, ignorado, atRisk, confirmedCompromised e unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-135">The possible values are none, confirmedSafe, remediated, dismissed, atRisk, confirmedCompromised, and unknownFutureValue.</span></span> |
|`riskLevel`|`riskLevel`|<span data-ttu-id="f4e8c-136">Nível do risco detectado.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-136">Level of the detected risk.</span></span> <span data-ttu-id="f4e8c-137">Os valores possíveis são baixo, médio, alto, oculto, nenhum, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-137">The possible values are low, medium, high, hidden, none, unknownFutureValue.</span></span> <span data-ttu-id="f4e8c-138">**Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-138">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="f4e8c-139">Clientes P1 serão retornados `hidden` .</span><span class="sxs-lookup"><span data-stu-id="f4e8c-139">P1 customers will be returned `hidden`.</span></span>|
|`riskDetail`|`riskDetail`|<span data-ttu-id="f4e8c-140">Detalhes do risco detectado.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-140">Details of the detected risk.</span></span> <span data-ttu-id="f4e8c-141">Os valores possíveis não são nenhum, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-141">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span> <span data-ttu-id="f4e8c-142">**Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-142">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="f4e8c-143">Clientes P1 serão retornados `hidden` .</span><span class="sxs-lookup"><span data-stu-id="f4e8c-143">P1 customers will be returned `hidden`.</span></span>|
|`source`|`string`|<span data-ttu-id="f4e8c-144">Origem da detecção de risco.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-144">Source of the risk detection.</span></span> <span data-ttu-id="f4e8c-145">Por exemplo, "activeDirectory".</span><span class="sxs-lookup"><span data-stu-id="f4e8c-145">For example, "activeDirectory".</span></span> |
|`detectionTimingType`|`riskDetectionTimingType`|<span data-ttu-id="f4e8c-146">Tempo do risco detectado (em tempo real/offline).</span><span class="sxs-lookup"><span data-stu-id="f4e8c-146">Timing of the detected risk (real-time/offline).</span></span> <span data-ttu-id="f4e8c-147">Os valores possíveis não sãoDefined, realtime, nearRealtime, offline, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-147">The possible values are notDefined, realtime, nearRealtime, offline, unknownFutureValue.</span></span> |
|`activity`|`activityType`|<span data-ttu-id="f4e8c-148">Indica o tipo de atividade ao qual o risco detectado está vinculado.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-148">Indicates the activity type the detected risk is linked to.</span></span> <span data-ttu-id="f4e8c-149">Os valores possíveis são signin, user, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-149">The possible values are signin, user, unknownFutureValue.</span></span> |
|`tokenIssuerType`|`tokenIssuerType`|<span data-ttu-id="f4e8c-150">Indica o tipo de emissor de token para o risco de entrar detectado.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-150">Indicates the type of token issuer for the detected sign-in risk.</span></span> <span data-ttu-id="f4e8c-151">Os valores possíveis são AzureAD, ADFederationServices e unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-151">The possible values are AzureAD, ADFederationServices, and unknownFutureValue.</span></span> |
|`ipAddress`|`string`|<span data-ttu-id="f4e8c-152">Fornece o endereço IP do cliente de onde o risco ocorreu.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-152">Provides the IP address of the client from where the risk occurred.</span></span> |
|`location`|[<span data-ttu-id="f4e8c-153">signInLocation</span><span class="sxs-lookup"><span data-stu-id="f4e8c-153">signInLocation</span></span>](signinlocation.md)|<span data-ttu-id="f4e8c-154">Local da assinatura.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-154">Location of the sign-in.</span></span> |
|`activityDateTime`|`datetimeoffset`|<span data-ttu-id="f4e8c-155">Data e hora em que a atividade arriscada ocorreu.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-155">Date and time that the risky activity occurred.</span></span> |
|`detectedDateTime`|`datetimeoffset`|<span data-ttu-id="f4e8c-156">Data e hora em que o risco foi detectado.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-156">Date and time that the risk was detected.</span></span> |
|`lastUpdatedDateTime`|`datetime`|<span data-ttu-id="f4e8c-157">Data e hora em que a detecção de risco foi atualizada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-157">Date and time that the risk detection was last updated.</span></span> |
|`userId`|`string`|<span data-ttu-id="f4e8c-158">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-158">Unique ID of the user.</span></span> |
|`userDisplayName`|`string`|<span data-ttu-id="f4e8c-159">Nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-159">Name of the user.</span></span> |
|`userPrincipalName`|`string`|<span data-ttu-id="f4e8c-160">O nome UPN do usuário.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-160">The user principal name (UPN) of the user.</span></span> |
|`additionalInfo`|`string`|<span data-ttu-id="f4e8c-161">Informações adicionais associadas à detecção de risco no formato JSON.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-161">Additional information associated with the risk detection in JSON format.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f4e8c-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4e8c-162">JSON representation</span></span>

<span data-ttu-id="f4e8c-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f4e8c-163">The following is a JSON representation of the resource.</span></span>

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
