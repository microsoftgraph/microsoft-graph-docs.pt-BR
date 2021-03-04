---
title: Tipo de recurso identityRiskEvent
description: 'Um evento de risco detectado pela Proteção de Identidade do Azure Active Directory. É o tipo base para cada tipo de evento de risco específico:'
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: acb48ce5ef63abf5ec2a09d8a3365a744bb8a668
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440287"
---
# <a name="identityriskevent-resource-type-deprecated"></a><span data-ttu-id="c76ee-104">Tipo de recurso identityRiskEvent (preterido)</span><span class="sxs-lookup"><span data-stu-id="c76ee-104">identityRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="c76ee-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c76ee-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="c76ee-106">A **API identityRiskEvents** está preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="c76ee-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="c76ee-107">Para obter detalhes, [consulte Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="c76ee-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="c76ee-108">Um evento de risco detectado pela Proteção de Identidade [do Azure Active Directory](/azure/active-directory/identity-protection/overview-identity-protection).</span><span class="sxs-lookup"><span data-stu-id="c76ee-108">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span></span> <span data-ttu-id="c76ee-109">É o tipo base para cada tipo de evento de risco específico:</span><span class="sxs-lookup"><span data-stu-id="c76ee-109">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="c76ee-110">Tipo de evento</span><span class="sxs-lookup"><span data-stu-id="c76ee-110">Event type</span></span>         | <span data-ttu-id="c76ee-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c76ee-111">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="c76ee-112">anonymousipRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c76ee-112">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="c76ee-113">Entrar de endereços IP anônimos.</span><span class="sxs-lookup"><span data-stu-id="c76ee-113">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="c76ee-114">malwareRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c76ee-114">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="c76ee-115">Entrar de dispositivos infectados por malware.</span><span class="sxs-lookup"><span data-stu-id="c76ee-115">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="c76ee-116">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c76ee-116">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="c76ee-117">Viagem impossível para locais atípicos.</span><span class="sxs-lookup"><span data-stu-id="c76ee-117">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="c76ee-118">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c76ee-118">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="c76ee-119">Usuários com credenciais vazadas.</span><span class="sxs-lookup"><span data-stu-id="c76ee-119">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="c76ee-120">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c76ee-120">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="c76ee-121">Entrar de endereços IP suspeitos.</span><span class="sxs-lookup"><span data-stu-id="c76ee-121">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="c76ee-122">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c76ee-122">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="c76ee-123">Entrar de locais desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="c76ee-123">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="c76ee-124">Informações completas sobre eventos de risco podem ser encontradas na documentação da Proteção de Identidade do [Azure AD.](/azure/active-directory/active-directory-reporting-risk-events)</span><span class="sxs-lookup"><span data-stu-id="c76ee-124">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="c76ee-125">Methods</span><span class="sxs-lookup"><span data-stu-id="c76ee-125">Methods</span></span>

| <span data-ttu-id="c76ee-126">Método</span><span class="sxs-lookup"><span data-stu-id="c76ee-126">Method</span></span>           | <span data-ttu-id="c76ee-127">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c76ee-127">Return Type</span></span>    |<span data-ttu-id="c76ee-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="c76ee-128">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c76ee-129">Obter identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c76ee-129">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="c76ee-130">identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c76ee-130">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="c76ee-131">Leia propriedades e relações do objeto identityRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="c76ee-131">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c76ee-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c76ee-132">Properties</span></span>
| <span data-ttu-id="c76ee-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c76ee-133">Property</span></span>     | <span data-ttu-id="c76ee-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="c76ee-134">Type</span></span>   |<span data-ttu-id="c76ee-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="c76ee-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c76ee-136">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="c76ee-136">closedDateTime</span></span>|<span data-ttu-id="c76ee-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c76ee-137">dateTimeOffset</span></span>| <span data-ttu-id="c76ee-138">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="c76ee-138">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="c76ee-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c76ee-139">createdDateTime</span></span>|<span data-ttu-id="c76ee-140">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c76ee-140">dateTimeOffset</span></span>| <span data-ttu-id="c76ee-141">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="c76ee-141">The date and time that the risk event was created.</span></span> <span data-ttu-id="c76ee-142">Isso é sempre maior ou igual ao tempo de data do evento de risco em si.</span><span class="sxs-lookup"><span data-stu-id="c76ee-142">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="c76ee-143">Essa é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="c76ee-143">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="c76ee-144">id</span><span class="sxs-lookup"><span data-stu-id="c76ee-144">id</span></span>|<span data-ttu-id="c76ee-145">string</span><span class="sxs-lookup"><span data-stu-id="c76ee-145">string</span></span>| <span data-ttu-id="c76ee-146">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="c76ee-146">Read-only</span></span>|
|<span data-ttu-id="c76ee-147">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="c76ee-147">riskEventDateTime</span></span>|<span data-ttu-id="c76ee-148">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c76ee-148">dateTimeOffset</span></span>| <span data-ttu-id="c76ee-149">A data e a hora em que o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="c76ee-149">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="c76ee-150">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="c76ee-150">riskEventStatus</span></span>|<span data-ttu-id="c76ee-151">string</span><span class="sxs-lookup"><span data-stu-id="c76ee-151">string</span></span>| <span data-ttu-id="c76ee-152">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="c76ee-152">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="c76ee-153">riskLevel</span><span class="sxs-lookup"><span data-stu-id="c76ee-153">riskLevel</span></span>|<span data-ttu-id="c76ee-154">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c76ee-154">string</span></span>| <span data-ttu-id="c76ee-155">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="c76ee-155">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="c76ee-156">riskEventType</span><span class="sxs-lookup"><span data-stu-id="c76ee-156">riskEventType</span></span>|<span data-ttu-id="c76ee-157">string</span><span class="sxs-lookup"><span data-stu-id="c76ee-157">string</span></span>| <span data-ttu-id="c76ee-158">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="c76ee-158">The type of risk</span></span>|
|<span data-ttu-id="c76ee-159">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c76ee-159">userDisplayName</span></span>|<span data-ttu-id="c76ee-160">string</span><span class="sxs-lookup"><span data-stu-id="c76ee-160">string</span></span>| <span data-ttu-id="c76ee-161">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="c76ee-161">The name of the user at risk</span></span>|
|<span data-ttu-id="c76ee-162">userId</span><span class="sxs-lookup"><span data-stu-id="c76ee-162">userId</span></span>|<span data-ttu-id="c76ee-163">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c76ee-163">string</span></span>| <span data-ttu-id="c76ee-164">A id do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="c76ee-164">The id of the user at risk</span></span>|
|<span data-ttu-id="c76ee-165">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c76ee-165">userPrincipalName</span></span>|<span data-ttu-id="c76ee-166">string</span><span class="sxs-lookup"><span data-stu-id="c76ee-166">string</span></span>| <span data-ttu-id="c76ee-167">O nome principal do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="c76ee-167">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="c76ee-168">Relações</span><span class="sxs-lookup"><span data-stu-id="c76ee-168">Relationships</span></span>
| <span data-ttu-id="c76ee-169">Relação</span><span class="sxs-lookup"><span data-stu-id="c76ee-169">Relationship</span></span> | <span data-ttu-id="c76ee-170">Tipo</span><span class="sxs-lookup"><span data-stu-id="c76ee-170">Type</span></span>   |<span data-ttu-id="c76ee-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="c76ee-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c76ee-172">impactedUser</span><span class="sxs-lookup"><span data-stu-id="c76ee-172">impactedUser</span></span>|[<span data-ttu-id="c76ee-173">user</span><span class="sxs-lookup"><span data-stu-id="c76ee-173">user</span></span>](user.md)| <span data-ttu-id="c76ee-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="c76ee-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c76ee-176">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c76ee-176">JSON representation</span></span>

<span data-ttu-id="c76ee-177">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c76ee-177">Here is a JSON representation of the resource.</span></span>

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
