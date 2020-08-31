---
title: tipo de recurso impossibleTravelRiskEvent
description: Um evento de risco detectado pela proteção de identidade do Azure Active Directory onde dois logons de conta ocorrem de locais atypical para o usuário e não seria possível viajar entre os locais na duração entre as entradas. As informações completas sobre eventos de risco podem ser encontradas na documentação de proteção de identidade do Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: 9100bd22426c634fedb16a776114ba973d4db531
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/29/2020
ms.locfileid: "47312030"
---
# <a name="impossibletravelriskevent-resource-type-deprecated"></a><span data-ttu-id="760fb-103">tipo de recurso impossibleTravelRiskEvent (preterido)</span><span class="sxs-lookup"><span data-stu-id="760fb-103">impossibleTravelRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="760fb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="760fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="760fb-105">A API **identityRiskEvents** foi preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="760fb-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="760fb-106">Para obter detalhes, consulte [Preterition of the IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="760fb-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="760fb-107">Um evento de risco detectado pela [proteção de identidade do Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) onde dois logons de conta ocorrem de locais atypical para o usuário e não seria possível viajar entre os locais na duração entre as entradas. As informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Azure ad](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="760fb-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="760fb-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="760fb-108">Methods</span></span>

| <span data-ttu-id="760fb-109">Método</span><span class="sxs-lookup"><span data-stu-id="760fb-109">Method</span></span>           | <span data-ttu-id="760fb-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="760fb-110">Return Type</span></span>    |<span data-ttu-id="760fb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="760fb-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="760fb-112">Obter impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="760fb-112">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="760fb-113">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="760fb-113">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="760fb-114">Leia as propriedades e os relacionamentos do objeto impossibleTravelRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="760fb-114">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="760fb-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="760fb-115">Properties</span></span>
| <span data-ttu-id="760fb-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="760fb-116">Property</span></span>     | <span data-ttu-id="760fb-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="760fb-117">Type</span></span>   |<span data-ttu-id="760fb-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="760fb-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="760fb-119">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="760fb-119">closedDateTime</span></span>|<span data-ttu-id="760fb-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="760fb-120">dateTimeOffset</span></span>| <span data-ttu-id="760fb-121">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="760fb-121">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="760fb-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="760fb-122">createdDateTime</span></span>|<span data-ttu-id="760fb-123">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="760fb-123">dateTimeOffset</span></span>| <span data-ttu-id="760fb-124">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="760fb-124">The date and time that the risk event was created.</span></span> <span data-ttu-id="760fb-125">Isso é sempre maior que ou igual ao DateTime do evento de risco propriamente dito.</span><span class="sxs-lookup"><span data-stu-id="760fb-125">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="760fb-126">Esta é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="760fb-126">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="760fb-127">deviceInformation</span><span class="sxs-lookup"><span data-stu-id="760fb-127">deviceInformation</span></span>|<span data-ttu-id="760fb-128">string</span><span class="sxs-lookup"><span data-stu-id="760fb-128">string</span></span>| <span data-ttu-id="760fb-129">Informações sobre o dispositivo</span><span class="sxs-lookup"><span data-stu-id="760fb-129">Information about the device</span></span>|
|<span data-ttu-id="760fb-130">id</span><span class="sxs-lookup"><span data-stu-id="760fb-130">id</span></span>|<span data-ttu-id="760fb-131">string</span><span class="sxs-lookup"><span data-stu-id="760fb-131">string</span></span>| <span data-ttu-id="760fb-132">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="760fb-132">Read-only</span></span>|
|<span data-ttu-id="760fb-133">ipAddress</span><span class="sxs-lookup"><span data-stu-id="760fb-133">ipAddress</span></span>|<span data-ttu-id="760fb-134">string</span><span class="sxs-lookup"><span data-stu-id="760fb-134">string</span></span>| <span data-ttu-id="760fb-135">O endereço IP da segunda entrada</span><span class="sxs-lookup"><span data-stu-id="760fb-135">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="760fb-136">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="760fb-136">isAtypicalLocation</span></span>|<span data-ttu-id="760fb-137">booliano</span><span class="sxs-lookup"><span data-stu-id="760fb-137">boolean</span></span>| <span data-ttu-id="760fb-138">Se um dos locais for atypical para o usuário</span><span class="sxs-lookup"><span data-stu-id="760fb-138">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="760fb-139">location</span><span class="sxs-lookup"><span data-stu-id="760fb-139">location</span></span>|<span data-ttu-id="760fb-140">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="760fb-140">string</span></span>| <span data-ttu-id="760fb-141">O local anexado ao endereço IP da segunda entrada</span><span class="sxs-lookup"><span data-stu-id="760fb-141">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="760fb-142">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="760fb-142">previousIPAddress</span></span>|<span data-ttu-id="760fb-143">string</span><span class="sxs-lookup"><span data-stu-id="760fb-143">string</span></span>| <span data-ttu-id="760fb-144">O endereço IP do primeiro logon</span><span class="sxs-lookup"><span data-stu-id="760fb-144">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="760fb-145">previousLocation</span><span class="sxs-lookup"><span data-stu-id="760fb-145">previousLocation</span></span>|<span data-ttu-id="760fb-146">string</span><span class="sxs-lookup"><span data-stu-id="760fb-146">string</span></span>| <span data-ttu-id="760fb-147">O local anexado ao endereço IP do primeiro logon</span><span class="sxs-lookup"><span data-stu-id="760fb-147">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="760fb-148">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="760fb-148">previousSigninDateTime</span></span>|<span data-ttu-id="760fb-149">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="760fb-149">dateTimeOffset</span></span>| <span data-ttu-id="760fb-150">A data e a hora da primeira entrada</span><span class="sxs-lookup"><span data-stu-id="760fb-150">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="760fb-151">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="760fb-151">riskEventDateTime</span></span>|<span data-ttu-id="760fb-152">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="760fb-152">dateTimeOffset</span></span>| <span data-ttu-id="760fb-153">A data e a hora da segunda entrada</span><span class="sxs-lookup"><span data-stu-id="760fb-153">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="760fb-154">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="760fb-154">riskEventStatus</span></span>|<span data-ttu-id="760fb-155">string</span><span class="sxs-lookup"><span data-stu-id="760fb-155">string</span></span>| <span data-ttu-id="760fb-156">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="760fb-156">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="760fb-157">riskLevel</span><span class="sxs-lookup"><span data-stu-id="760fb-157">riskLevel</span></span>|<span data-ttu-id="760fb-158">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="760fb-158">string</span></span>| <span data-ttu-id="760fb-159">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="760fb-159">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="760fb-160">riskEventType</span><span class="sxs-lookup"><span data-stu-id="760fb-160">riskEventType</span></span>|<span data-ttu-id="760fb-161">string</span><span class="sxs-lookup"><span data-stu-id="760fb-161">string</span></span>| <span data-ttu-id="760fb-162">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="760fb-162">The type of risk</span></span>|
|<span data-ttu-id="760fb-163">userAgent</span><span class="sxs-lookup"><span data-stu-id="760fb-163">userAgent</span></span>|<span data-ttu-id="760fb-164">string</span><span class="sxs-lookup"><span data-stu-id="760fb-164">string</span></span>| <span data-ttu-id="760fb-165">A cadeia de caracteres do agente do usuário do navegador</span><span class="sxs-lookup"><span data-stu-id="760fb-165">The browser's user agent string</span></span>|
|<span data-ttu-id="760fb-166">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="760fb-166">userDisplayName</span></span>|<span data-ttu-id="760fb-167">string</span><span class="sxs-lookup"><span data-stu-id="760fb-167">string</span></span>| <span data-ttu-id="760fb-168">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="760fb-168">The name of the user at risk</span></span>|
|<span data-ttu-id="760fb-169">userId</span><span class="sxs-lookup"><span data-stu-id="760fb-169">userId</span></span>|<span data-ttu-id="760fb-170">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="760fb-170">string</span></span>| <span data-ttu-id="760fb-171">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="760fb-171">The id of the user at risk</span></span>|
|<span data-ttu-id="760fb-172">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="760fb-172">userPrincipalName</span></span>|<span data-ttu-id="760fb-173">string</span><span class="sxs-lookup"><span data-stu-id="760fb-173">string</span></span>| <span data-ttu-id="760fb-174">O nome principal de usuário do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="760fb-174">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="760fb-175">Relações</span><span class="sxs-lookup"><span data-stu-id="760fb-175">Relationships</span></span>
| <span data-ttu-id="760fb-176">Relação</span><span class="sxs-lookup"><span data-stu-id="760fb-176">Relationship</span></span> | <span data-ttu-id="760fb-177">Tipo</span><span class="sxs-lookup"><span data-stu-id="760fb-177">Type</span></span>   |<span data-ttu-id="760fb-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="760fb-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="760fb-179">impactedUser</span><span class="sxs-lookup"><span data-stu-id="760fb-179">impactedUser</span></span>|[<span data-ttu-id="760fb-180">user</span><span class="sxs-lookup"><span data-stu-id="760fb-180">user</span></span>](user.md)| <span data-ttu-id="760fb-p103">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="760fb-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="760fb-183">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="760fb-183">JSON representation</span></span>

<span data-ttu-id="760fb-184">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="760fb-184">Here is a JSON representation of the resource.</span></span>

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
