---
title: tipo de recurso identityRiskEvent
description: 'Um evento de risco detectado pela proteção de identidade do Azure Active Directory. É o tipo base para cada tipo de evento de risco específico:'
author: cloudhandler
localization_priority: Normal
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 7ea0a11931021e828660cc7b03991b8ea96ef1f1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005797"
---
# <a name="identityriskevent-resource-type"></a><span data-ttu-id="4a8a0-104">tipo de recurso identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="4a8a0-104">identityRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a8a0-105">Um evento de risco detectado pela [proteção de identidade do Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="4a8a0-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span> <span data-ttu-id="4a8a0-106">É o tipo base para cada tipo de evento de risco específico:</span><span class="sxs-lookup"><span data-stu-id="4a8a0-106">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="4a8a0-107">Tipo de evento</span><span class="sxs-lookup"><span data-stu-id="4a8a0-107">Event type</span></span>         | <span data-ttu-id="4a8a0-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a8a0-108">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="4a8a0-109">anonymousipRiskEvent</span><span class="sxs-lookup"><span data-stu-id="4a8a0-109">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="4a8a0-110">Entradas de endereços IP anônimos.</span><span class="sxs-lookup"><span data-stu-id="4a8a0-110">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="4a8a0-111">malwareRiskEvent</span><span class="sxs-lookup"><span data-stu-id="4a8a0-111">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="4a8a0-112">Entradas de dispositivos infectados por malware.</span><span class="sxs-lookup"><span data-stu-id="4a8a0-112">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="4a8a0-113">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="4a8a0-113">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="4a8a0-114">Impossível viajar para locais do atypical.</span><span class="sxs-lookup"><span data-stu-id="4a8a0-114">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="4a8a0-115">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="4a8a0-115">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="4a8a0-116">Usuários com credenciais vazadas.</span><span class="sxs-lookup"><span data-stu-id="4a8a0-116">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="4a8a0-117">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="4a8a0-117">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="4a8a0-118">Entradas de endereços IP suspeitos.</span><span class="sxs-lookup"><span data-stu-id="4a8a0-118">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="4a8a0-119">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="4a8a0-119">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="4a8a0-120">Entradas de locais desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="4a8a0-120">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="4a8a0-121">As informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Azure ad](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span><span class="sxs-lookup"><span data-stu-id="4a8a0-121">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="4a8a0-122">Métodos</span><span class="sxs-lookup"><span data-stu-id="4a8a0-122">Methods</span></span>

| <span data-ttu-id="4a8a0-123">Método</span><span class="sxs-lookup"><span data-stu-id="4a8a0-123">Method</span></span>           | <span data-ttu-id="4a8a0-124">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4a8a0-124">Return Type</span></span>    |<span data-ttu-id="4a8a0-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a8a0-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4a8a0-126">Obter identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="4a8a0-126">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="4a8a0-127">identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="4a8a0-127">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="4a8a0-128">Leia as propriedades e os relacionamentos do objeto identityRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="4a8a0-128">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4a8a0-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a8a0-129">Properties</span></span>
| <span data-ttu-id="4a8a0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a8a0-130">Property</span></span>     | <span data-ttu-id="4a8a0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a8a0-131">Type</span></span>   |<span data-ttu-id="4a8a0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a8a0-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a8a0-133">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a8a0-133">closedDateTime</span></span>|<span data-ttu-id="4a8a0-134">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a8a0-134">dateTimeOffset</span></span>| <span data-ttu-id="4a8a0-135">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="4a8a0-135">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="4a8a0-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4a8a0-136">createdDateTime</span></span>|<span data-ttu-id="4a8a0-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a8a0-137">dateTimeOffset</span></span>| <span data-ttu-id="4a8a0-138">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="4a8a0-138">The date and time that the risk event was created.</span></span> <span data-ttu-id="4a8a0-139">Isso é sempre maior que ou igual ao DateTime do evento de risco propriamente dito.</span><span class="sxs-lookup"><span data-stu-id="4a8a0-139">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="4a8a0-140">Esta é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="4a8a0-140">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="4a8a0-141">id</span><span class="sxs-lookup"><span data-stu-id="4a8a0-141">id</span></span>|<span data-ttu-id="4a8a0-142">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a8a0-142">string</span></span>| <span data-ttu-id="4a8a0-143">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="4a8a0-143">Read-only</span></span>|
|<span data-ttu-id="4a8a0-144">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="4a8a0-144">riskEventDateTime</span></span>|<span data-ttu-id="4a8a0-145">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a8a0-145">dateTimeOffset</span></span>| <span data-ttu-id="4a8a0-146">A data e a hora em que o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="4a8a0-146">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="4a8a0-147">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="4a8a0-147">riskEventStatus</span></span>|<span data-ttu-id="4a8a0-148">string</span><span class="sxs-lookup"><span data-stu-id="4a8a0-148">string</span></span>| <span data-ttu-id="4a8a0-149">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="4a8a0-149">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="4a8a0-150">riskLevel</span><span class="sxs-lookup"><span data-stu-id="4a8a0-150">riskLevel</span></span>|<span data-ttu-id="4a8a0-151">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a8a0-151">string</span></span>| <span data-ttu-id="4a8a0-152">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="4a8a0-152">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="4a8a0-153">riskEventType</span><span class="sxs-lookup"><span data-stu-id="4a8a0-153">riskEventType</span></span>|<span data-ttu-id="4a8a0-154">string</span><span class="sxs-lookup"><span data-stu-id="4a8a0-154">string</span></span>| <span data-ttu-id="4a8a0-155">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="4a8a0-155">The type of risk</span></span>|
|<span data-ttu-id="4a8a0-156">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4a8a0-156">userDisplayName</span></span>|<span data-ttu-id="4a8a0-157">string</span><span class="sxs-lookup"><span data-stu-id="4a8a0-157">string</span></span>| <span data-ttu-id="4a8a0-158">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="4a8a0-158">The name of the user at risk</span></span>|
|<span data-ttu-id="4a8a0-159">userId</span><span class="sxs-lookup"><span data-stu-id="4a8a0-159">userId</span></span>|<span data-ttu-id="4a8a0-160">string</span><span class="sxs-lookup"><span data-stu-id="4a8a0-160">string</span></span>| <span data-ttu-id="4a8a0-161">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="4a8a0-161">The id of the user at risk</span></span>|
|<span data-ttu-id="4a8a0-162">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4a8a0-162">userPrincipalName</span></span>|<span data-ttu-id="4a8a0-163">string</span><span class="sxs-lookup"><span data-stu-id="4a8a0-163">string</span></span>| <span data-ttu-id="4a8a0-164">O nome principal de usuário do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="4a8a0-164">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a8a0-165">Relações</span><span class="sxs-lookup"><span data-stu-id="4a8a0-165">Relationships</span></span>
| <span data-ttu-id="4a8a0-166">Relação</span><span class="sxs-lookup"><span data-stu-id="4a8a0-166">Relationship</span></span> | <span data-ttu-id="4a8a0-167">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a8a0-167">Type</span></span>   |<span data-ttu-id="4a8a0-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a8a0-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a8a0-169">impactedUser</span><span class="sxs-lookup"><span data-stu-id="4a8a0-169">impactedUser</span></span>|[<span data-ttu-id="4a8a0-170">Usuário</span><span class="sxs-lookup"><span data-stu-id="4a8a0-170">user</span></span>](user.md)| <span data-ttu-id="4a8a0-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="4a8a0-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4a8a0-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a8a0-173">JSON representation</span></span>

<span data-ttu-id="4a8a0-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4a8a0-174">Here is a JSON representation of the resource.</span></span> 

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
