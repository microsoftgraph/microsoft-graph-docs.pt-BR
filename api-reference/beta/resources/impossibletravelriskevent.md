---
title: tipo de recurso impossibleTravelRiskEvent
description: Um evento de risco detectado pela proteção de identidade do Azure Active Directory onde dois logons de conta ocorrem de locais atypical para o usuário e não seria possível viajar entre os locais na duração entre os logons. complete information about eventos de risco podem ser encontrados na documentação de proteção de identidade do Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2b66755924022b4fa30637cc8e97c4f944ad2d79
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005769"
---
# <a name="impossibletravelriskevent-resource-type"></a><span data-ttu-id="d59f4-103">tipo de recurso impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="d59f4-103">impossibleTravelRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d59f4-104">Um evento de risco detectado pela [proteção de identidade do Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) onde dois logons de conta ocorrem a partir de locais atypical para o usuário e seria impossível viajar entre os locais na duração entre os logins. Complete as informações sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Azure ad](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="d59f4-104">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="d59f4-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="d59f4-105">Methods</span></span>

| <span data-ttu-id="d59f4-106">Método</span><span class="sxs-lookup"><span data-stu-id="d59f4-106">Method</span></span>           | <span data-ttu-id="d59f4-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d59f4-107">Return Type</span></span>    |<span data-ttu-id="d59f4-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d59f4-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d59f4-109">Obter impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="d59f4-109">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="d59f4-110">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="d59f4-110">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="d59f4-111">Leia as propriedades e os relacionamentos do objeto impossibleTravelRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="d59f4-111">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d59f4-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d59f4-112">Properties</span></span>
| <span data-ttu-id="d59f4-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d59f4-113">Property</span></span>     | <span data-ttu-id="d59f4-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="d59f4-114">Type</span></span>   |<span data-ttu-id="d59f4-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="d59f4-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d59f4-116">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="d59f4-116">closedDateTime</span></span>|<span data-ttu-id="d59f4-117">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d59f4-117">dateTimeOffset</span></span>| <span data-ttu-id="d59f4-118">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="d59f4-118">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="d59f4-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d59f4-119">createdDateTime</span></span>|<span data-ttu-id="d59f4-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d59f4-120">dateTimeOffset</span></span>| <span data-ttu-id="d59f4-121">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="d59f4-121">The date and time that the risk event was created.</span></span> <span data-ttu-id="d59f4-122">Isso é sempre maior que ou igual ao DateTime do evento de risco propriamente dito.</span><span class="sxs-lookup"><span data-stu-id="d59f4-122">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="d59f4-123">Esta é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="d59f4-123">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="d59f4-124">deviceInformation</span><span class="sxs-lookup"><span data-stu-id="d59f4-124">deviceInformation</span></span>|<span data-ttu-id="d59f4-125">string</span><span class="sxs-lookup"><span data-stu-id="d59f4-125">string</span></span>| <span data-ttu-id="d59f4-126">Informações sobre o dispositivo</span><span class="sxs-lookup"><span data-stu-id="d59f4-126">Information about the device</span></span>|
|<span data-ttu-id="d59f4-127">id</span><span class="sxs-lookup"><span data-stu-id="d59f4-127">id</span></span>|<span data-ttu-id="d59f4-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d59f4-128">string</span></span>| <span data-ttu-id="d59f4-129">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="d59f4-129">Read-only</span></span>|
|<span data-ttu-id="d59f4-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="d59f4-130">ipAddress</span></span>|<span data-ttu-id="d59f4-131">string</span><span class="sxs-lookup"><span data-stu-id="d59f4-131">string</span></span>| <span data-ttu-id="d59f4-132">O endereço IP da segunda entrada</span><span class="sxs-lookup"><span data-stu-id="d59f4-132">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="d59f4-133">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="d59f4-133">isAtypicalLocation</span></span>|<span data-ttu-id="d59f4-134">booliano</span><span class="sxs-lookup"><span data-stu-id="d59f4-134">boolean</span></span>| <span data-ttu-id="d59f4-135">Se um dos locais for atypical para o usuário</span><span class="sxs-lookup"><span data-stu-id="d59f4-135">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="d59f4-136">location</span><span class="sxs-lookup"><span data-stu-id="d59f4-136">location</span></span>|<span data-ttu-id="d59f4-137">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d59f4-137">string</span></span>| <span data-ttu-id="d59f4-138">O local anexado ao endereço IP da segunda entrada</span><span class="sxs-lookup"><span data-stu-id="d59f4-138">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="d59f4-139">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="d59f4-139">previousIPAddress</span></span>|<span data-ttu-id="d59f4-140">string</span><span class="sxs-lookup"><span data-stu-id="d59f4-140">string</span></span>| <span data-ttu-id="d59f4-141">O endereço IP do primeiro logon</span><span class="sxs-lookup"><span data-stu-id="d59f4-141">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="d59f4-142">previousLocation</span><span class="sxs-lookup"><span data-stu-id="d59f4-142">previousLocation</span></span>|<span data-ttu-id="d59f4-143">string</span><span class="sxs-lookup"><span data-stu-id="d59f4-143">string</span></span>| <span data-ttu-id="d59f4-144">O local anexado ao endereço IP do primeiro logon</span><span class="sxs-lookup"><span data-stu-id="d59f4-144">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="d59f4-145">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="d59f4-145">previousSigninDateTime</span></span>|<span data-ttu-id="d59f4-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d59f4-146">dateTimeOffset</span></span>| <span data-ttu-id="d59f4-147">A data e a hora da primeira entrada</span><span class="sxs-lookup"><span data-stu-id="d59f4-147">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="d59f4-148">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="d59f4-148">riskEventDateTime</span></span>|<span data-ttu-id="d59f4-149">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d59f4-149">dateTimeOffset</span></span>| <span data-ttu-id="d59f4-150">A data e a hora da segunda entrada</span><span class="sxs-lookup"><span data-stu-id="d59f4-150">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="d59f4-151">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="d59f4-151">riskEventStatus</span></span>|<span data-ttu-id="d59f4-152">string</span><span class="sxs-lookup"><span data-stu-id="d59f4-152">string</span></span>| <span data-ttu-id="d59f4-153">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="d59f4-153">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="d59f4-154">riskLevel</span><span class="sxs-lookup"><span data-stu-id="d59f4-154">riskLevel</span></span>|<span data-ttu-id="d59f4-155">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d59f4-155">string</span></span>| <span data-ttu-id="d59f4-156">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="d59f4-156">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="d59f4-157">riskEventType</span><span class="sxs-lookup"><span data-stu-id="d59f4-157">riskEventType</span></span>|<span data-ttu-id="d59f4-158">string</span><span class="sxs-lookup"><span data-stu-id="d59f4-158">string</span></span>| <span data-ttu-id="d59f4-159">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="d59f4-159">The type of risk</span></span>|
|<span data-ttu-id="d59f4-160">userAgent</span><span class="sxs-lookup"><span data-stu-id="d59f4-160">userAgent</span></span>|<span data-ttu-id="d59f4-161">string</span><span class="sxs-lookup"><span data-stu-id="d59f4-161">string</span></span>| <span data-ttu-id="d59f4-162">A cadeia de caracteres do agente do usuário do navegador</span><span class="sxs-lookup"><span data-stu-id="d59f4-162">The browser's user agent string</span></span>|
|<span data-ttu-id="d59f4-163">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d59f4-163">userDisplayName</span></span>|<span data-ttu-id="d59f4-164">string</span><span class="sxs-lookup"><span data-stu-id="d59f4-164">string</span></span>| <span data-ttu-id="d59f4-165">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="d59f4-165">The name of the user at risk</span></span>|
|<span data-ttu-id="d59f4-166">userId</span><span class="sxs-lookup"><span data-stu-id="d59f4-166">userId</span></span>|<span data-ttu-id="d59f4-167">string</span><span class="sxs-lookup"><span data-stu-id="d59f4-167">string</span></span>| <span data-ttu-id="d59f4-168">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="d59f4-168">The id of the user at risk</span></span>|
|<span data-ttu-id="d59f4-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d59f4-169">userPrincipalName</span></span>|<span data-ttu-id="d59f4-170">string</span><span class="sxs-lookup"><span data-stu-id="d59f4-170">string</span></span>| <span data-ttu-id="d59f4-171">O nome principal de usuário do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="d59f4-171">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="d59f4-172">Relações</span><span class="sxs-lookup"><span data-stu-id="d59f4-172">Relationships</span></span>
| <span data-ttu-id="d59f4-173">Relação</span><span class="sxs-lookup"><span data-stu-id="d59f4-173">Relationship</span></span> | <span data-ttu-id="d59f4-174">Tipo</span><span class="sxs-lookup"><span data-stu-id="d59f4-174">Type</span></span>   |<span data-ttu-id="d59f4-175">Descrição</span><span class="sxs-lookup"><span data-stu-id="d59f4-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d59f4-176">impactedUser</span><span class="sxs-lookup"><span data-stu-id="d59f4-176">impactedUser</span></span>|[<span data-ttu-id="d59f4-177">Usuário</span><span class="sxs-lookup"><span data-stu-id="d59f4-177">user</span></span>](user.md)| <span data-ttu-id="d59f4-p102">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="d59f4-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d59f4-180">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d59f4-180">JSON representation</span></span>

<span data-ttu-id="d59f4-181">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d59f4-181">Here is a JSON representation of the resource.</span></span>

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
