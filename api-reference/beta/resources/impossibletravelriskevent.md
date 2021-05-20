---
title: Tipo de recurso impossibleTravelRiskEvent
description: Um evento de risco detectado pela Proteção de Identidade Azure Active Directory em que duas insinuidades de conta ocorrem de locais atípicos para o usuário e seria impossível viajar entre os locais durante a duração entre as insinuações. Informações completas sobre eventos de risco podem ser encontradas na documentação da Proteção de Identidade do Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: cloudhandler
ms.openlocfilehash: e05760bc4e3c60d3d4079965cdf01b0d5f630a77
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547005"
---
# <a name="impossibletravelriskevent-resource-type-deprecated"></a><span data-ttu-id="af8b4-103">tipo de recurso impossibleTravelRiskEvent (preterido)</span><span class="sxs-lookup"><span data-stu-id="af8b4-103">impossibleTravelRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="af8b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af8b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="af8b4-105">A **API identityRiskEvents** está preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="af8b4-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="af8b4-106">Para obter detalhes, [consulte Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="af8b4-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="af8b4-107">Um evento de risco detectado pela Proteção de Identidade Azure Active Directory em que duas insinuidades de conta ocorrem de locais atípicos para o usuário e seria impossível viajar entre os locais durante [a](/azure/active-directory/identity-protection/overview-identity-protection) duração entre as insinuações. Informações completas sobre eventos de risco podem ser encontradas na documentação da Proteção de Identidade do [Azure AD.](/azure/active-directory/identity-protection/overview-identity-protection)</span><span class="sxs-lookup"><span data-stu-id="af8b4-107">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="af8b4-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="af8b4-108">Methods</span></span>

| <span data-ttu-id="af8b4-109">Método</span><span class="sxs-lookup"><span data-stu-id="af8b4-109">Method</span></span>           | <span data-ttu-id="af8b4-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="af8b4-110">Return Type</span></span>    |<span data-ttu-id="af8b4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="af8b4-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="af8b4-112">Obter impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="af8b4-112">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="af8b4-113">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="af8b4-113">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="af8b4-114">Ler propriedades e relações do objeto impossibleTravelRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="af8b4-114">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="af8b4-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="af8b4-115">Properties</span></span>
| <span data-ttu-id="af8b4-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af8b4-116">Property</span></span>     | <span data-ttu-id="af8b4-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="af8b4-117">Type</span></span>   |<span data-ttu-id="af8b4-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="af8b4-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af8b4-119">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="af8b4-119">closedDateTime</span></span>|<span data-ttu-id="af8b4-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af8b4-120">dateTimeOffset</span></span>| <span data-ttu-id="af8b4-121">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="af8b4-121">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="af8b4-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="af8b4-122">createdDateTime</span></span>|<span data-ttu-id="af8b4-123">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af8b4-123">dateTimeOffset</span></span>| <span data-ttu-id="af8b4-124">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="af8b4-124">The date and time that the risk event was created.</span></span> <span data-ttu-id="af8b4-125">Isso é sempre maior ou igual ao tempo de data do evento de risco em si.</span><span class="sxs-lookup"><span data-stu-id="af8b4-125">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="af8b4-126">Essa é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="af8b4-126">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="af8b4-127">deviceInformation</span><span class="sxs-lookup"><span data-stu-id="af8b4-127">deviceInformation</span></span>|<span data-ttu-id="af8b4-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af8b4-128">string</span></span>| <span data-ttu-id="af8b4-129">Informações sobre o dispositivo</span><span class="sxs-lookup"><span data-stu-id="af8b4-129">Information about the device</span></span>|
|<span data-ttu-id="af8b4-130">id</span><span class="sxs-lookup"><span data-stu-id="af8b4-130">id</span></span>|<span data-ttu-id="af8b4-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af8b4-131">string</span></span>| <span data-ttu-id="af8b4-132">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="af8b4-132">Read-only</span></span>|
|<span data-ttu-id="af8b4-133">ipAddress</span><span class="sxs-lookup"><span data-stu-id="af8b4-133">ipAddress</span></span>|<span data-ttu-id="af8b4-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af8b4-134">string</span></span>| <span data-ttu-id="af8b4-135">O endereço IP do segundo login</span><span class="sxs-lookup"><span data-stu-id="af8b4-135">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="af8b4-136">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="af8b4-136">isAtypicalLocation</span></span>|<span data-ttu-id="af8b4-137">booliano</span><span class="sxs-lookup"><span data-stu-id="af8b4-137">boolean</span></span>| <span data-ttu-id="af8b4-138">Se um dos locais for atípico para o usuário</span><span class="sxs-lookup"><span data-stu-id="af8b4-138">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="af8b4-139">location</span><span class="sxs-lookup"><span data-stu-id="af8b4-139">location</span></span>|<span data-ttu-id="af8b4-140">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af8b4-140">string</span></span>| <span data-ttu-id="af8b4-141">O local anexado ao endereço IP do segundo login</span><span class="sxs-lookup"><span data-stu-id="af8b4-141">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="af8b4-142">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="af8b4-142">previousIPAddress</span></span>|<span data-ttu-id="af8b4-143">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af8b4-143">string</span></span>| <span data-ttu-id="af8b4-144">O endereço IP do primeiro login</span><span class="sxs-lookup"><span data-stu-id="af8b4-144">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="af8b4-145">previousLocation</span><span class="sxs-lookup"><span data-stu-id="af8b4-145">previousLocation</span></span>|<span data-ttu-id="af8b4-146">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af8b4-146">string</span></span>| <span data-ttu-id="af8b4-147">O local anexado ao endereço IP do primeiro login</span><span class="sxs-lookup"><span data-stu-id="af8b4-147">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="af8b4-148">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="af8b4-148">previousSigninDateTime</span></span>|<span data-ttu-id="af8b4-149">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af8b4-149">dateTimeOffset</span></span>| <span data-ttu-id="af8b4-150">A data e a hora do primeiro login</span><span class="sxs-lookup"><span data-stu-id="af8b4-150">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="af8b4-151">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="af8b4-151">riskEventDateTime</span></span>|<span data-ttu-id="af8b4-152">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af8b4-152">dateTimeOffset</span></span>| <span data-ttu-id="af8b4-153">A data e a hora do segundo login</span><span class="sxs-lookup"><span data-stu-id="af8b4-153">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="af8b4-154">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="af8b4-154">riskEventStatus</span></span>|<span data-ttu-id="af8b4-155">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af8b4-155">string</span></span>| <span data-ttu-id="af8b4-156">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="af8b4-156">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="af8b4-157">riskLevel</span><span class="sxs-lookup"><span data-stu-id="af8b4-157">riskLevel</span></span>|<span data-ttu-id="af8b4-158">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af8b4-158">string</span></span>| <span data-ttu-id="af8b4-159">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="af8b4-159">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="af8b4-160">riskEventType</span><span class="sxs-lookup"><span data-stu-id="af8b4-160">riskEventType</span></span>|<span data-ttu-id="af8b4-161">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af8b4-161">string</span></span>| <span data-ttu-id="af8b4-162">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="af8b4-162">The type of risk</span></span>|
|<span data-ttu-id="af8b4-163">userAgent</span><span class="sxs-lookup"><span data-stu-id="af8b4-163">userAgent</span></span>|<span data-ttu-id="af8b4-164">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af8b4-164">string</span></span>| <span data-ttu-id="af8b4-165">Cadeia de caracteres de agente de usuário do navegador</span><span class="sxs-lookup"><span data-stu-id="af8b4-165">The browser's user agent string</span></span>|
|<span data-ttu-id="af8b4-166">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="af8b4-166">userDisplayName</span></span>|<span data-ttu-id="af8b4-167">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af8b4-167">string</span></span>| <span data-ttu-id="af8b4-168">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="af8b4-168">The name of the user at risk</span></span>|
|<span data-ttu-id="af8b4-169">userId</span><span class="sxs-lookup"><span data-stu-id="af8b4-169">userId</span></span>|<span data-ttu-id="af8b4-170">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af8b4-170">string</span></span>| <span data-ttu-id="af8b4-171">A id do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="af8b4-171">The id of the user at risk</span></span>|
|<span data-ttu-id="af8b4-172">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="af8b4-172">userPrincipalName</span></span>|<span data-ttu-id="af8b4-173">string</span><span class="sxs-lookup"><span data-stu-id="af8b4-173">string</span></span>| <span data-ttu-id="af8b4-174">O nome principal do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="af8b4-174">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="af8b4-175">Relações</span><span class="sxs-lookup"><span data-stu-id="af8b4-175">Relationships</span></span>
| <span data-ttu-id="af8b4-176">Relação</span><span class="sxs-lookup"><span data-stu-id="af8b4-176">Relationship</span></span> | <span data-ttu-id="af8b4-177">Tipo</span><span class="sxs-lookup"><span data-stu-id="af8b4-177">Type</span></span>   |<span data-ttu-id="af8b4-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="af8b4-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af8b4-179">impactedUser</span><span class="sxs-lookup"><span data-stu-id="af8b4-179">impactedUser</span></span>|[<span data-ttu-id="af8b4-180">user</span><span class="sxs-lookup"><span data-stu-id="af8b4-180">user</span></span>](user.md)| <span data-ttu-id="af8b4-p103">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="af8b4-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="af8b4-183">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="af8b4-183">JSON representation</span></span>

<span data-ttu-id="af8b4-184">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="af8b4-184">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.impossibleTravelRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "deviceInformation": "string",
  "id": "string (identifier)",
  "ipAddress": "string",
  "isAtypicalLocation": true,
  "location": "string",
  "previousIPAddress": "string",
  "previousLocation": "string",
  "previousSigninDateTime": "String (timestamp)",
  "riskEventDateTime": "String (timestamp)",
  "riskEventStatus": "string",
  "riskLevel": "string",
  "riskType": "string",
  "userAgent": "string",
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
  "description": "impossibleTravelRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
