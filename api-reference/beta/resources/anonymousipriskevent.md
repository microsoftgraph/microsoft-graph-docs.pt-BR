---
title: Tipo de recurso anonymousIpRiskEvent
description: Um evento de risco detectado pela Proteção de Identidade do Azure Active Directory em que uma conta de login é tentada de um endereço IP que parece ser anônimo. Informações completas sobre eventos de risco podem ser encontradas na documentação da Proteção de Identidade do Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: 4b5ead2c32368ec29c87fd5d5f05f4e48e5e17a0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433191"
---
# <a name="anonymousipriskevent-resource-type-deprecated"></a><span data-ttu-id="43226-104">Tipo de recurso anonymousIpRiskEvent (preterido)</span><span class="sxs-lookup"><span data-stu-id="43226-104">anonymousIpRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="43226-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43226-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="43226-106">A **API identityRiskEvents** está preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="43226-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="43226-107">Para obter detalhes, [consulte Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="43226-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="43226-108">Um evento de risco detectado pela Proteção de Identidade do [Azure Active Directory](/azure/active-directory/identity-protection/overview-identity-protection) em que uma conta de login é tentada de um endereço IP que parece ser anônimo.</span><span class="sxs-lookup"><span data-stu-id="43226-108">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) where an account sign-in is attempted from an IP address that appears to be anonymous.</span></span> <span data-ttu-id="43226-109">Informações completas sobre eventos de risco podem ser encontradas na documentação da Proteção de Identidade do [Azure AD.](/azure/active-directory/identity-protection/overview-identity-protection)</span><span class="sxs-lookup"><span data-stu-id="43226-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="43226-110">Methods</span><span class="sxs-lookup"><span data-stu-id="43226-110">Methods</span></span>

| <span data-ttu-id="43226-111">Método</span><span class="sxs-lookup"><span data-stu-id="43226-111">Method</span></span>           | <span data-ttu-id="43226-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="43226-112">Return Type</span></span>    |<span data-ttu-id="43226-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="43226-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="43226-114">Obter anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="43226-114">Get anonymousIpRiskEvent</span></span>](../api/anonymousipriskevent-get.md) | [<span data-ttu-id="43226-115">anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="43226-115">anonymousIpRiskEvent</span></span>](anonymousipriskevent.md) |<span data-ttu-id="43226-116">Leia propriedades e relações do objeto anonymousIpRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="43226-116">Read properties and relationships of anonymousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="43226-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="43226-117">Properties</span></span>
| <span data-ttu-id="43226-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43226-118">Property</span></span>     | <span data-ttu-id="43226-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="43226-119">Type</span></span>   |<span data-ttu-id="43226-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="43226-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43226-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="43226-121">closedDateTime</span></span>|<span data-ttu-id="43226-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43226-122">dateTimeOffset</span></span>| <span data-ttu-id="43226-123">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="43226-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="43226-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43226-124">createdDateTime</span></span>|<span data-ttu-id="43226-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43226-125">dateTimeOffset</span></span>| <span data-ttu-id="43226-126">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="43226-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="43226-127">Isso é sempre maior ou igual ao tempo de data do evento de risco em si.</span><span class="sxs-lookup"><span data-stu-id="43226-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="43226-128">Essa é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="43226-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="43226-129">id</span><span class="sxs-lookup"><span data-stu-id="43226-129">id</span></span>|<span data-ttu-id="43226-130">string</span><span class="sxs-lookup"><span data-stu-id="43226-130">string</span></span>| <span data-ttu-id="43226-131">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="43226-131">Read-only</span></span>|
|<span data-ttu-id="43226-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="43226-132">ipAddress</span></span>|<span data-ttu-id="43226-133">string</span><span class="sxs-lookup"><span data-stu-id="43226-133">string</span></span>| <span data-ttu-id="43226-134">O endereço IP da assinatura</span><span class="sxs-lookup"><span data-stu-id="43226-134">The IP address of the sign-in</span></span>|
|<span data-ttu-id="43226-135">location</span><span class="sxs-lookup"><span data-stu-id="43226-135">location</span></span>|<span data-ttu-id="43226-136">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43226-136">string</span></span>| <span data-ttu-id="43226-137">O local anexado ao endereço IP da login</span><span class="sxs-lookup"><span data-stu-id="43226-137">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="43226-138">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="43226-138">riskEventDateTime</span></span>|<span data-ttu-id="43226-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43226-139">dateTimeOffset</span></span>| <span data-ttu-id="43226-140">A data e a hora em que o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="43226-140">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="43226-141">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="43226-141">riskEventStatus</span></span>|<span data-ttu-id="43226-142">string</span><span class="sxs-lookup"><span data-stu-id="43226-142">string</span></span>| <span data-ttu-id="43226-143">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="43226-143">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="43226-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="43226-144">riskLevel</span></span>|<span data-ttu-id="43226-145">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43226-145">string</span></span>| <span data-ttu-id="43226-146">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="43226-146">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="43226-147">riskEventType</span><span class="sxs-lookup"><span data-stu-id="43226-147">riskEventType</span></span>|<span data-ttu-id="43226-148">string</span><span class="sxs-lookup"><span data-stu-id="43226-148">string</span></span>| <span data-ttu-id="43226-149">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="43226-149">The type of risk</span></span>|
|<span data-ttu-id="43226-150">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="43226-150">userDisplayName</span></span>|<span data-ttu-id="43226-151">string</span><span class="sxs-lookup"><span data-stu-id="43226-151">string</span></span>| <span data-ttu-id="43226-152">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="43226-152">The name of the user at risk</span></span>|
|<span data-ttu-id="43226-153">userId</span><span class="sxs-lookup"><span data-stu-id="43226-153">userId</span></span>|<span data-ttu-id="43226-154">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43226-154">string</span></span>| <span data-ttu-id="43226-155">A id do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="43226-155">The id of the user at risk</span></span>|
|<span data-ttu-id="43226-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="43226-156">userPrincipalName</span></span>|<span data-ttu-id="43226-157">string</span><span class="sxs-lookup"><span data-stu-id="43226-157">string</span></span>| <span data-ttu-id="43226-158">O nome principal do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="43226-158">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="43226-159">Relações</span><span class="sxs-lookup"><span data-stu-id="43226-159">Relationships</span></span>
| <span data-ttu-id="43226-160">Relação</span><span class="sxs-lookup"><span data-stu-id="43226-160">Relationship</span></span> | <span data-ttu-id="43226-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="43226-161">Type</span></span>   |<span data-ttu-id="43226-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="43226-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43226-163">impactedUser</span><span class="sxs-lookup"><span data-stu-id="43226-163">impactedUser</span></span>|[<span data-ttu-id="43226-164">user</span><span class="sxs-lookup"><span data-stu-id="43226-164">user</span></span>](user.md)| <span data-ttu-id="43226-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="43226-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="43226-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="43226-167">JSON representation</span></span>

<span data-ttu-id="43226-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="43226-168">Here is a JSON representation of the resource.</span></span>

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
