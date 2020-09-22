---
title: tipo de recurso anonymousIpRiskEvent
description: Um evento de risco detectado pela proteção de identidade do Azure Active Directory em que uma entrada de conta é tentada a partir de um endereço IP que parece ser anônimo. As informações completas sobre eventos de risco podem ser encontradas na documentação de proteção de identidade do Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: e233e1995748f57a5da9eca51bf336b60d5273b7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004267"
---
# <a name="anonymousipriskevent-resource-type-deprecated"></a><span data-ttu-id="0ff55-104">tipo de recurso anonymousIpRiskEvent (preterido)</span><span class="sxs-lookup"><span data-stu-id="0ff55-104">anonymousIpRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="0ff55-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ff55-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="0ff55-106">A API **identityRiskEvents** foi preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="0ff55-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="0ff55-107">Para obter detalhes, consulte [Preterition of the IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="0ff55-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="0ff55-108">Um evento de risco detectado pela [proteção de identidade do Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) em que uma entrada de conta é tentada a partir de um endereço IP que parece ser anônimo.</span><span class="sxs-lookup"><span data-stu-id="0ff55-108">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from an IP address that appears to be anonymous.</span></span> <span data-ttu-id="0ff55-109">As informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Azure ad](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="0ff55-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="0ff55-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="0ff55-110">Methods</span></span>

| <span data-ttu-id="0ff55-111">Método</span><span class="sxs-lookup"><span data-stu-id="0ff55-111">Method</span></span>           | <span data-ttu-id="0ff55-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0ff55-112">Return Type</span></span>    |<span data-ttu-id="0ff55-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ff55-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0ff55-114">Obter anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="0ff55-114">Get anonymousIpRiskEvent</span></span>](../api/anonymousipriskevent-get.md) | [<span data-ttu-id="0ff55-115">anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="0ff55-115">anonymousIpRiskEvent</span></span>](anonymousipriskevent.md) |<span data-ttu-id="0ff55-116">Leia as propriedades e os relacionamentos do objeto anonymousIpRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="0ff55-116">Read properties and relationships of anonymousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0ff55-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ff55-117">Properties</span></span>
| <span data-ttu-id="0ff55-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ff55-118">Property</span></span>     | <span data-ttu-id="0ff55-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ff55-119">Type</span></span>   |<span data-ttu-id="0ff55-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ff55-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ff55-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ff55-121">closedDateTime</span></span>|<span data-ttu-id="0ff55-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ff55-122">dateTimeOffset</span></span>| <span data-ttu-id="0ff55-123">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="0ff55-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="0ff55-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ff55-124">createdDateTime</span></span>|<span data-ttu-id="0ff55-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ff55-125">dateTimeOffset</span></span>| <span data-ttu-id="0ff55-126">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="0ff55-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="0ff55-127">Isso é sempre maior que ou igual ao DateTime do evento de risco propriamente dito.</span><span class="sxs-lookup"><span data-stu-id="0ff55-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="0ff55-128">Esta é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="0ff55-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="0ff55-129">id</span><span class="sxs-lookup"><span data-stu-id="0ff55-129">id</span></span>|<span data-ttu-id="0ff55-130">string</span><span class="sxs-lookup"><span data-stu-id="0ff55-130">string</span></span>| <span data-ttu-id="0ff55-131">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="0ff55-131">Read-only</span></span>|
|<span data-ttu-id="0ff55-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="0ff55-132">ipAddress</span></span>|<span data-ttu-id="0ff55-133">string</span><span class="sxs-lookup"><span data-stu-id="0ff55-133">string</span></span>| <span data-ttu-id="0ff55-134">O endereço IP do logon</span><span class="sxs-lookup"><span data-stu-id="0ff55-134">The IP address of the sign-in</span></span>|
|<span data-ttu-id="0ff55-135">location</span><span class="sxs-lookup"><span data-stu-id="0ff55-135">location</span></span>|<span data-ttu-id="0ff55-136">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ff55-136">string</span></span>| <span data-ttu-id="0ff55-137">O local anexado ao endereço IP do logon</span><span class="sxs-lookup"><span data-stu-id="0ff55-137">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="0ff55-138">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="0ff55-138">riskEventDateTime</span></span>|<span data-ttu-id="0ff55-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ff55-139">dateTimeOffset</span></span>| <span data-ttu-id="0ff55-140">A data e a hora em que o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="0ff55-140">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="0ff55-141">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="0ff55-141">riskEventStatus</span></span>|<span data-ttu-id="0ff55-142">string</span><span class="sxs-lookup"><span data-stu-id="0ff55-142">string</span></span>| <span data-ttu-id="0ff55-143">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="0ff55-143">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="0ff55-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="0ff55-144">riskLevel</span></span>|<span data-ttu-id="0ff55-145">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ff55-145">string</span></span>| <span data-ttu-id="0ff55-146">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="0ff55-146">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="0ff55-147">riskEventType</span><span class="sxs-lookup"><span data-stu-id="0ff55-147">riskEventType</span></span>|<span data-ttu-id="0ff55-148">string</span><span class="sxs-lookup"><span data-stu-id="0ff55-148">string</span></span>| <span data-ttu-id="0ff55-149">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="0ff55-149">The type of risk</span></span>|
|<span data-ttu-id="0ff55-150">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="0ff55-150">userDisplayName</span></span>|<span data-ttu-id="0ff55-151">string</span><span class="sxs-lookup"><span data-stu-id="0ff55-151">string</span></span>| <span data-ttu-id="0ff55-152">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="0ff55-152">The name of the user at risk</span></span>|
|<span data-ttu-id="0ff55-153">userId</span><span class="sxs-lookup"><span data-stu-id="0ff55-153">userId</span></span>|<span data-ttu-id="0ff55-154">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ff55-154">string</span></span>| <span data-ttu-id="0ff55-155">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="0ff55-155">The id of the user at risk</span></span>|
|<span data-ttu-id="0ff55-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0ff55-156">userPrincipalName</span></span>|<span data-ttu-id="0ff55-157">string</span><span class="sxs-lookup"><span data-stu-id="0ff55-157">string</span></span>| <span data-ttu-id="0ff55-158">O nome principal de usuário do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="0ff55-158">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ff55-159">Relações</span><span class="sxs-lookup"><span data-stu-id="0ff55-159">Relationships</span></span>
| <span data-ttu-id="0ff55-160">Relação</span><span class="sxs-lookup"><span data-stu-id="0ff55-160">Relationship</span></span> | <span data-ttu-id="0ff55-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ff55-161">Type</span></span>   |<span data-ttu-id="0ff55-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ff55-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ff55-163">impactedUser</span><span class="sxs-lookup"><span data-stu-id="0ff55-163">impactedUser</span></span>|[<span data-ttu-id="0ff55-164">user</span><span class="sxs-lookup"><span data-stu-id="0ff55-164">user</span></span>](user.md)| <span data-ttu-id="0ff55-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="0ff55-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0ff55-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ff55-167">JSON representation</span></span>

<span data-ttu-id="0ff55-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ff55-168">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
   "baseType":"microsoft.graph.locatedRiskEvent",
  "@odata.type": "microsoft.graph.anonymousIpRiskEvent"
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
  "description": "anonymousIpRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


