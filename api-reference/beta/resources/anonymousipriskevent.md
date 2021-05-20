---
title: Tipo de recurso anonymousIpRiskEvent
description: Um evento de risco detectado pela Azure Active Directory Identity Protection em que uma conta de login é tentada a partir de um endereço IP que parece ser anônimo. Informações completas sobre eventos de risco podem ser encontradas na documentação da Proteção de Identidade do Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: cloudhandler
ms.openlocfilehash: d4acf5d9b3d5d05a2769178657b397b22f1cb3f2
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547545"
---
# <a name="anonymousipriskevent-resource-type-deprecated"></a><span data-ttu-id="77a97-104">Tipo de recurso anonymousIpRiskEvent (preterido)</span><span class="sxs-lookup"><span data-stu-id="77a97-104">anonymousIpRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="77a97-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77a97-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="77a97-106">A **API identityRiskEvents** está preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="77a97-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="77a97-107">Para obter detalhes, [consulte Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="77a97-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="77a97-108">Um evento de risco detectado pela [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) em que uma conta de login é tentada a partir de um endereço IP que parece ser anônimo.</span><span class="sxs-lookup"><span data-stu-id="77a97-108">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) where an account sign-in is attempted from an IP address that appears to be anonymous.</span></span> <span data-ttu-id="77a97-109">Informações completas sobre eventos de risco podem ser encontradas na documentação da Proteção de Identidade do [Azure AD.](/azure/active-directory/identity-protection/overview-identity-protection)</span><span class="sxs-lookup"><span data-stu-id="77a97-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="77a97-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="77a97-110">Methods</span></span>

| <span data-ttu-id="77a97-111">Método</span><span class="sxs-lookup"><span data-stu-id="77a97-111">Method</span></span>           | <span data-ttu-id="77a97-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="77a97-112">Return Type</span></span>    |<span data-ttu-id="77a97-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="77a97-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="77a97-114">Obter anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="77a97-114">Get anonymousIpRiskEvent</span></span>](../api/anonymousipriskevent-get.md) | [<span data-ttu-id="77a97-115">anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="77a97-115">anonymousIpRiskEvent</span></span>](anonymousipriskevent.md) |<span data-ttu-id="77a97-116">Leia propriedades e relações do objeto anonymousIpRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="77a97-116">Read properties and relationships of anonymousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="77a97-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="77a97-117">Properties</span></span>
| <span data-ttu-id="77a97-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77a97-118">Property</span></span>     | <span data-ttu-id="77a97-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="77a97-119">Type</span></span>   |<span data-ttu-id="77a97-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="77a97-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77a97-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="77a97-121">closedDateTime</span></span>|<span data-ttu-id="77a97-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77a97-122">dateTimeOffset</span></span>| <span data-ttu-id="77a97-123">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="77a97-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="77a97-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77a97-124">createdDateTime</span></span>|<span data-ttu-id="77a97-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77a97-125">dateTimeOffset</span></span>| <span data-ttu-id="77a97-126">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="77a97-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="77a97-127">Isso é sempre maior ou igual ao tempo de data do evento de risco em si.</span><span class="sxs-lookup"><span data-stu-id="77a97-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="77a97-128">Essa é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="77a97-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="77a97-129">id</span><span class="sxs-lookup"><span data-stu-id="77a97-129">id</span></span>|<span data-ttu-id="77a97-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77a97-130">string</span></span>| <span data-ttu-id="77a97-131">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="77a97-131">Read-only</span></span>|
|<span data-ttu-id="77a97-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="77a97-132">ipAddress</span></span>|<span data-ttu-id="77a97-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77a97-133">string</span></span>| <span data-ttu-id="77a97-134">O endereço IP da assinatura</span><span class="sxs-lookup"><span data-stu-id="77a97-134">The IP address of the sign-in</span></span>|
|<span data-ttu-id="77a97-135">location</span><span class="sxs-lookup"><span data-stu-id="77a97-135">location</span></span>|<span data-ttu-id="77a97-136">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77a97-136">string</span></span>| <span data-ttu-id="77a97-137">O local anexado ao endereço IP da login</span><span class="sxs-lookup"><span data-stu-id="77a97-137">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="77a97-138">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="77a97-138">riskEventDateTime</span></span>|<span data-ttu-id="77a97-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77a97-139">dateTimeOffset</span></span>| <span data-ttu-id="77a97-140">A data e a hora em que o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="77a97-140">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="77a97-141">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="77a97-141">riskEventStatus</span></span>|<span data-ttu-id="77a97-142">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77a97-142">string</span></span>| <span data-ttu-id="77a97-143">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="77a97-143">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="77a97-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="77a97-144">riskLevel</span></span>|<span data-ttu-id="77a97-145">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77a97-145">string</span></span>| <span data-ttu-id="77a97-146">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="77a97-146">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="77a97-147">riskEventType</span><span class="sxs-lookup"><span data-stu-id="77a97-147">riskEventType</span></span>|<span data-ttu-id="77a97-148">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77a97-148">string</span></span>| <span data-ttu-id="77a97-149">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="77a97-149">The type of risk</span></span>|
|<span data-ttu-id="77a97-150">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="77a97-150">userDisplayName</span></span>|<span data-ttu-id="77a97-151">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77a97-151">string</span></span>| <span data-ttu-id="77a97-152">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="77a97-152">The name of the user at risk</span></span>|
|<span data-ttu-id="77a97-153">userId</span><span class="sxs-lookup"><span data-stu-id="77a97-153">userId</span></span>|<span data-ttu-id="77a97-154">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77a97-154">string</span></span>| <span data-ttu-id="77a97-155">A id do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="77a97-155">The id of the user at risk</span></span>|
|<span data-ttu-id="77a97-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="77a97-156">userPrincipalName</span></span>|<span data-ttu-id="77a97-157">string</span><span class="sxs-lookup"><span data-stu-id="77a97-157">string</span></span>| <span data-ttu-id="77a97-158">O nome principal do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="77a97-158">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="77a97-159">Relações</span><span class="sxs-lookup"><span data-stu-id="77a97-159">Relationships</span></span>
| <span data-ttu-id="77a97-160">Relação</span><span class="sxs-lookup"><span data-stu-id="77a97-160">Relationship</span></span> | <span data-ttu-id="77a97-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="77a97-161">Type</span></span>   |<span data-ttu-id="77a97-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="77a97-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77a97-163">impactedUser</span><span class="sxs-lookup"><span data-stu-id="77a97-163">impactedUser</span></span>|[<span data-ttu-id="77a97-164">user</span><span class="sxs-lookup"><span data-stu-id="77a97-164">user</span></span>](user.md)| <span data-ttu-id="77a97-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="77a97-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="77a97-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="77a97-167">JSON representation</span></span>

<span data-ttu-id="77a97-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="77a97-168">Here is a JSON representation of the resource.</span></span>

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
