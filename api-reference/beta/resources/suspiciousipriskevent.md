---
title: tipo de recurso suspiciousIpRiskEvent
description: Um evento de risco detectado pela proteção de identidade do Azure Active Directory em que uma entrada de conta é tentada a partir de um endereço IP suspeito. As informações completas sobre eventos de risco podem ser encontradas na documentação de proteção de identidade do Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: fe4b0069c6ed12a5d74fc32d1d8a71b5dd8dffde
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078154"
---
# <a name="suspiciousipriskevent-resource-type-deprecated"></a><span data-ttu-id="801c3-104">tipo de recurso suspiciousIpRiskEvent (preterido)</span><span class="sxs-lookup"><span data-stu-id="801c3-104">suspiciousIpRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="801c3-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="801c3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="801c3-106">A API **identityRiskEvents** foi preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="801c3-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="801c3-107">Para obter detalhes, consulte [Preterition of the IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="801c3-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="801c3-108">Um evento de risco detectado pela [proteção de identidade do Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) em que uma entrada de conta é tentada a partir de um endereço IP suspeito.</span><span class="sxs-lookup"><span data-stu-id="801c3-108">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from a suspicious IP address.</span></span> <span data-ttu-id="801c3-109">As informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Azure ad](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="801c3-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="801c3-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="801c3-110">Methods</span></span>

| <span data-ttu-id="801c3-111">Método</span><span class="sxs-lookup"><span data-stu-id="801c3-111">Method</span></span>           | <span data-ttu-id="801c3-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="801c3-112">Return Type</span></span>    |<span data-ttu-id="801c3-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="801c3-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="801c3-114">Obter suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="801c3-114">Get suspiciousIpRiskEvent</span></span>](../api/suspiciousipriskevent-get.md) | [<span data-ttu-id="801c3-115">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="801c3-115">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) |<span data-ttu-id="801c3-116">Leia as propriedades e os relacionamentos do objeto suspiciousIpRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="801c3-116">Read properties and relationships of suspiciousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="801c3-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="801c3-117">Properties</span></span>
| <span data-ttu-id="801c3-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="801c3-118">Property</span></span>     | <span data-ttu-id="801c3-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="801c3-119">Type</span></span>   |<span data-ttu-id="801c3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="801c3-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="801c3-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="801c3-121">closedDateTime</span></span>|<span data-ttu-id="801c3-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="801c3-122">dateTimeOffset</span></span>| <span data-ttu-id="801c3-123">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="801c3-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="801c3-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="801c3-124">createdDateTime</span></span>|<span data-ttu-id="801c3-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="801c3-125">dateTimeOffset</span></span>| <span data-ttu-id="801c3-126">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="801c3-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="801c3-127">Isso é sempre maior que ou igual ao DateTime do evento de risco propriamente dito.</span><span class="sxs-lookup"><span data-stu-id="801c3-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="801c3-128">Esta é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="801c3-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="801c3-129">id</span><span class="sxs-lookup"><span data-stu-id="801c3-129">id</span></span>|<span data-ttu-id="801c3-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="801c3-130">string</span></span>| <span data-ttu-id="801c3-131">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="801c3-131">Read-only</span></span>|
|<span data-ttu-id="801c3-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="801c3-132">ipAddress</span></span>|<span data-ttu-id="801c3-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="801c3-133">string</span></span>| <span data-ttu-id="801c3-134">O endereço IP do logon</span><span class="sxs-lookup"><span data-stu-id="801c3-134">The IP address of the sign-in</span></span>|
|<span data-ttu-id="801c3-135">location</span><span class="sxs-lookup"><span data-stu-id="801c3-135">location</span></span>|<span data-ttu-id="801c3-136">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="801c3-136">string</span></span>| <span data-ttu-id="801c3-137">O local anexado ao endereço IP do logon</span><span class="sxs-lookup"><span data-stu-id="801c3-137">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="801c3-138">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="801c3-138">riskEventDateTime</span></span>|<span data-ttu-id="801c3-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="801c3-139">dateTimeOffset</span></span>| <span data-ttu-id="801c3-140">A data e a hora em que o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="801c3-140">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="801c3-141">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="801c3-141">riskEventStatus</span></span>|<span data-ttu-id="801c3-142">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="801c3-142">string</span></span>| <span data-ttu-id="801c3-143">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="801c3-143">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="801c3-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="801c3-144">riskLevel</span></span>|<span data-ttu-id="801c3-145">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="801c3-145">string</span></span>| <span data-ttu-id="801c3-146">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="801c3-146">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="801c3-147">riskEventType</span><span class="sxs-lookup"><span data-stu-id="801c3-147">riskEventType</span></span>|<span data-ttu-id="801c3-148">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="801c3-148">string</span></span>| <span data-ttu-id="801c3-149">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="801c3-149">The type of risk</span></span>|
|<span data-ttu-id="801c3-150">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="801c3-150">userDisplayName</span></span>|<span data-ttu-id="801c3-151">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="801c3-151">string</span></span>| <span data-ttu-id="801c3-152">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="801c3-152">The name of the user at risk</span></span>|
|<span data-ttu-id="801c3-153">userId</span><span class="sxs-lookup"><span data-stu-id="801c3-153">userId</span></span>|<span data-ttu-id="801c3-154">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="801c3-154">string</span></span>| <span data-ttu-id="801c3-155">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="801c3-155">The id of the user at risk</span></span>|
|<span data-ttu-id="801c3-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="801c3-156">userPrincipalName</span></span>|<span data-ttu-id="801c3-157">string</span><span class="sxs-lookup"><span data-stu-id="801c3-157">string</span></span>| <span data-ttu-id="801c3-158">O nome principal de usuário do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="801c3-158">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="801c3-159">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="801c3-159">Relationships</span></span>
| <span data-ttu-id="801c3-160">Relação</span><span class="sxs-lookup"><span data-stu-id="801c3-160">Relationship</span></span> | <span data-ttu-id="801c3-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="801c3-161">Type</span></span>   |<span data-ttu-id="801c3-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="801c3-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="801c3-163">impactedUser</span><span class="sxs-lookup"><span data-stu-id="801c3-163">impactedUser</span></span>|[<span data-ttu-id="801c3-164">usuário</span><span class="sxs-lookup"><span data-stu-id="801c3-164">user</span></span>](user.md)| <span data-ttu-id="801c3-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="801c3-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="801c3-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="801c3-167">JSON representation</span></span>

<span data-ttu-id="801c3-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="801c3-168">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.suspiciousIpRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "ipAddress": "string",
  "location": "string",
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
  "description": "suspiciousIpRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


