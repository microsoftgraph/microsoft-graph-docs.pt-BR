---
title: tipo de recurso identityRiskEvent
description: 'Um evento de risco detectado pela proteção de identidade do Azure Active Directory. É o tipo base para cada tipo de evento de risco específico:'
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 555e4dd162b2a5be51e8cf9a7d98b57d6de6c24e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013565"
---
# <a name="identityriskevent-resource-type-deprecated"></a><span data-ttu-id="9716d-104">tipo de recurso identityRiskEvent (preterido)</span><span class="sxs-lookup"><span data-stu-id="9716d-104">identityRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="9716d-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9716d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="9716d-106">A API **identityRiskEvents** foi preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="9716d-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="9716d-107">Para obter detalhes, consulte [Preterition of the IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="9716d-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="9716d-108">Um evento de risco detectado pela [proteção de identidade do Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="9716d-108">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).</span></span> <span data-ttu-id="9716d-109">É o tipo base para cada tipo de evento de risco específico:</span><span class="sxs-lookup"><span data-stu-id="9716d-109">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="9716d-110">Tipo de evento</span><span class="sxs-lookup"><span data-stu-id="9716d-110">Event type</span></span>         | <span data-ttu-id="9716d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9716d-111">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="9716d-112">anonymousipRiskEvent</span><span class="sxs-lookup"><span data-stu-id="9716d-112">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="9716d-113">Entradas de endereços IP anônimos.</span><span class="sxs-lookup"><span data-stu-id="9716d-113">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="9716d-114">malwareRiskEvent</span><span class="sxs-lookup"><span data-stu-id="9716d-114">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="9716d-115">Entradas de dispositivos infectados por malware.</span><span class="sxs-lookup"><span data-stu-id="9716d-115">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="9716d-116">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="9716d-116">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="9716d-117">Impossível viajar para locais do atypical.</span><span class="sxs-lookup"><span data-stu-id="9716d-117">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="9716d-118">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="9716d-118">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="9716d-119">Usuários com credenciais vazadas.</span><span class="sxs-lookup"><span data-stu-id="9716d-119">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="9716d-120">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="9716d-120">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="9716d-121">Entradas de endereços IP suspeitos.</span><span class="sxs-lookup"><span data-stu-id="9716d-121">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="9716d-122">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="9716d-122">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="9716d-123">Entradas de locais desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="9716d-123">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="9716d-124">As informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Azure ad](/azure/active-directory/active-directory-reporting-risk-events).</span><span class="sxs-lookup"><span data-stu-id="9716d-124">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="9716d-125">Methods</span><span class="sxs-lookup"><span data-stu-id="9716d-125">Methods</span></span>

| <span data-ttu-id="9716d-126">Método</span><span class="sxs-lookup"><span data-stu-id="9716d-126">Method</span></span>           | <span data-ttu-id="9716d-127">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9716d-127">Return Type</span></span>    |<span data-ttu-id="9716d-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="9716d-128">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9716d-129">Obter identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="9716d-129">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="9716d-130">identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="9716d-130">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="9716d-131">Leia as propriedades e os relacionamentos do objeto identityRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="9716d-131">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9716d-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9716d-132">Properties</span></span>
| <span data-ttu-id="9716d-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9716d-133">Property</span></span>     | <span data-ttu-id="9716d-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="9716d-134">Type</span></span>   |<span data-ttu-id="9716d-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="9716d-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9716d-136">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="9716d-136">closedDateTime</span></span>|<span data-ttu-id="9716d-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9716d-137">dateTimeOffset</span></span>| <span data-ttu-id="9716d-138">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="9716d-138">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="9716d-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9716d-139">createdDateTime</span></span>|<span data-ttu-id="9716d-140">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9716d-140">dateTimeOffset</span></span>| <span data-ttu-id="9716d-141">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="9716d-141">The date and time that the risk event was created.</span></span> <span data-ttu-id="9716d-142">Isso é sempre maior que ou igual ao DateTime do evento de risco propriamente dito.</span><span class="sxs-lookup"><span data-stu-id="9716d-142">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="9716d-143">Esta é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="9716d-143">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="9716d-144">id</span><span class="sxs-lookup"><span data-stu-id="9716d-144">id</span></span>|<span data-ttu-id="9716d-145">string</span><span class="sxs-lookup"><span data-stu-id="9716d-145">string</span></span>| <span data-ttu-id="9716d-146">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="9716d-146">Read-only</span></span>|
|<span data-ttu-id="9716d-147">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="9716d-147">riskEventDateTime</span></span>|<span data-ttu-id="9716d-148">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9716d-148">dateTimeOffset</span></span>| <span data-ttu-id="9716d-149">A data e a hora em que o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="9716d-149">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="9716d-150">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="9716d-150">riskEventStatus</span></span>|<span data-ttu-id="9716d-151">string</span><span class="sxs-lookup"><span data-stu-id="9716d-151">string</span></span>| <span data-ttu-id="9716d-152">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="9716d-152">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="9716d-153">riskLevel</span><span class="sxs-lookup"><span data-stu-id="9716d-153">riskLevel</span></span>|<span data-ttu-id="9716d-154">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9716d-154">string</span></span>| <span data-ttu-id="9716d-155">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="9716d-155">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="9716d-156">riskEventType</span><span class="sxs-lookup"><span data-stu-id="9716d-156">riskEventType</span></span>|<span data-ttu-id="9716d-157">string</span><span class="sxs-lookup"><span data-stu-id="9716d-157">string</span></span>| <span data-ttu-id="9716d-158">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="9716d-158">The type of risk</span></span>|
|<span data-ttu-id="9716d-159">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="9716d-159">userDisplayName</span></span>|<span data-ttu-id="9716d-160">string</span><span class="sxs-lookup"><span data-stu-id="9716d-160">string</span></span>| <span data-ttu-id="9716d-161">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="9716d-161">The name of the user at risk</span></span>|
|<span data-ttu-id="9716d-162">userId</span><span class="sxs-lookup"><span data-stu-id="9716d-162">userId</span></span>|<span data-ttu-id="9716d-163">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9716d-163">string</span></span>| <span data-ttu-id="9716d-164">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="9716d-164">The id of the user at risk</span></span>|
|<span data-ttu-id="9716d-165">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9716d-165">userPrincipalName</span></span>|<span data-ttu-id="9716d-166">string</span><span class="sxs-lookup"><span data-stu-id="9716d-166">string</span></span>| <span data-ttu-id="9716d-167">O nome principal de usuário do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="9716d-167">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="9716d-168">Relações</span><span class="sxs-lookup"><span data-stu-id="9716d-168">Relationships</span></span>
| <span data-ttu-id="9716d-169">Relação</span><span class="sxs-lookup"><span data-stu-id="9716d-169">Relationship</span></span> | <span data-ttu-id="9716d-170">Tipo</span><span class="sxs-lookup"><span data-stu-id="9716d-170">Type</span></span>   |<span data-ttu-id="9716d-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="9716d-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9716d-172">impactedUser</span><span class="sxs-lookup"><span data-stu-id="9716d-172">impactedUser</span></span>|[<span data-ttu-id="9716d-173">user</span><span class="sxs-lookup"><span data-stu-id="9716d-173">user</span></span>](user.md)| <span data-ttu-id="9716d-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="9716d-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9716d-176">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9716d-176">JSON representation</span></span>

<span data-ttu-id="9716d-177">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9716d-177">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identityRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "riskEventDateTime": "String (timestamp)",
  "riskEventStatus": "string",
  "riskLevel": "string",
  "riskType": "string",
  "userDisplayName": "string",
  "userId": "string",
  "userPrincipalName": "string",
  "riskEventType": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


