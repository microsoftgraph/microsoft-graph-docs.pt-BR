---
title: tipo de recurso impossibleTravelRiskEvent
description: Um evento de risco detectado pela proteção de identidade do Azure Active Directory onde dois logons de conta ocorrem de locais atypical para o usuário e não seria possível viajar entre os locais na duração entre os logons. complete information about eventos de risco podem ser encontrados na documentação de proteção de identidade do Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: be2b5db09a20264525e783e05771f6d1da2783e2
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866781"
---
# <a name="impossibletravelriskevent-resource-type"></a><span data-ttu-id="fd290-103">tipo de recurso impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="fd290-103">impossibleTravelRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="fd290-104">A API **identityRiskEvents** foi preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="fd290-104">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="fd290-105">Para obter detalhes, consulte [Preterition of the IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="fd290-105">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="fd290-106">Um evento de risco detectado pela [proteção de identidade do Active Directory do Azure](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) onde dois logons de conta ocorrem a partir de locais atypical para o usuário e seria impossível viajar entre os locais na duração entre as entradas. Complete as informações sobre os eventos de risco podem ser encontradas na [documentação do Azure ad Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="fd290-106">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="fd290-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="fd290-107">Methods</span></span>

| <span data-ttu-id="fd290-108">Método</span><span class="sxs-lookup"><span data-stu-id="fd290-108">Method</span></span>           | <span data-ttu-id="fd290-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fd290-109">Return Type</span></span>    |<span data-ttu-id="fd290-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd290-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fd290-111">Obter impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="fd290-111">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="fd290-112">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="fd290-112">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="fd290-113">Leia as propriedades e os relacionamentos do objeto impossibleTravelRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="fd290-113">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fd290-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fd290-114">Properties</span></span>
| <span data-ttu-id="fd290-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd290-115">Property</span></span>     | <span data-ttu-id="fd290-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd290-116">Type</span></span>   |<span data-ttu-id="fd290-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd290-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd290-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd290-118">closedDateTime</span></span>|<span data-ttu-id="fd290-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd290-119">dateTimeOffset</span></span>| <span data-ttu-id="fd290-120">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="fd290-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="fd290-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fd290-121">createdDateTime</span></span>|<span data-ttu-id="fd290-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd290-122">dateTimeOffset</span></span>| <span data-ttu-id="fd290-123">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="fd290-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="fd290-124">Isso é sempre maior que ou igual ao DateTime do evento de risco propriamente dito.</span><span class="sxs-lookup"><span data-stu-id="fd290-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="fd290-125">Esta é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="fd290-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="fd290-126">deviceInformation</span><span class="sxs-lookup"><span data-stu-id="fd290-126">deviceInformation</span></span>|<span data-ttu-id="fd290-127">string</span><span class="sxs-lookup"><span data-stu-id="fd290-127">string</span></span>| <span data-ttu-id="fd290-128">Informações sobre o dispositivo</span><span class="sxs-lookup"><span data-stu-id="fd290-128">Information about the device</span></span>|
|<span data-ttu-id="fd290-129">id</span><span class="sxs-lookup"><span data-stu-id="fd290-129">id</span></span>|<span data-ttu-id="fd290-130">string</span><span class="sxs-lookup"><span data-stu-id="fd290-130">string</span></span>| <span data-ttu-id="fd290-131">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="fd290-131">Read-only</span></span>|
|<span data-ttu-id="fd290-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="fd290-132">ipAddress</span></span>|<span data-ttu-id="fd290-133">string</span><span class="sxs-lookup"><span data-stu-id="fd290-133">string</span></span>| <span data-ttu-id="fd290-134">O endereço IP da segunda entrada</span><span class="sxs-lookup"><span data-stu-id="fd290-134">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="fd290-135">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="fd290-135">isAtypicalLocation</span></span>|<span data-ttu-id="fd290-136">booliano</span><span class="sxs-lookup"><span data-stu-id="fd290-136">boolean</span></span>| <span data-ttu-id="fd290-137">Se um dos locais for atypical para o usuário</span><span class="sxs-lookup"><span data-stu-id="fd290-137">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="fd290-138">location</span><span class="sxs-lookup"><span data-stu-id="fd290-138">location</span></span>|<span data-ttu-id="fd290-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd290-139">string</span></span>| <span data-ttu-id="fd290-140">O local anexado ao endereço IP da segunda entrada</span><span class="sxs-lookup"><span data-stu-id="fd290-140">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="fd290-141">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="fd290-141">previousIPAddress</span></span>|<span data-ttu-id="fd290-142">string</span><span class="sxs-lookup"><span data-stu-id="fd290-142">string</span></span>| <span data-ttu-id="fd290-143">O endereço IP do primeiro logon</span><span class="sxs-lookup"><span data-stu-id="fd290-143">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="fd290-144">previousLocation</span><span class="sxs-lookup"><span data-stu-id="fd290-144">previousLocation</span></span>|<span data-ttu-id="fd290-145">string</span><span class="sxs-lookup"><span data-stu-id="fd290-145">string</span></span>| <span data-ttu-id="fd290-146">O local anexado ao endereço IP do primeiro logon</span><span class="sxs-lookup"><span data-stu-id="fd290-146">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="fd290-147">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="fd290-147">previousSigninDateTime</span></span>|<span data-ttu-id="fd290-148">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd290-148">dateTimeOffset</span></span>| <span data-ttu-id="fd290-149">A data e a hora da primeira entrada</span><span class="sxs-lookup"><span data-stu-id="fd290-149">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="fd290-150">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="fd290-150">riskEventDateTime</span></span>|<span data-ttu-id="fd290-151">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd290-151">dateTimeOffset</span></span>| <span data-ttu-id="fd290-152">A data e a hora da segunda entrada</span><span class="sxs-lookup"><span data-stu-id="fd290-152">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="fd290-153">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="fd290-153">riskEventStatus</span></span>|<span data-ttu-id="fd290-154">string</span><span class="sxs-lookup"><span data-stu-id="fd290-154">string</span></span>| <span data-ttu-id="fd290-155">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="fd290-155">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="fd290-156">riskLevel</span><span class="sxs-lookup"><span data-stu-id="fd290-156">riskLevel</span></span>|<span data-ttu-id="fd290-157">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd290-157">string</span></span>| <span data-ttu-id="fd290-158">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="fd290-158">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="fd290-159">riskEventType</span><span class="sxs-lookup"><span data-stu-id="fd290-159">riskEventType</span></span>|<span data-ttu-id="fd290-160">string</span><span class="sxs-lookup"><span data-stu-id="fd290-160">string</span></span>| <span data-ttu-id="fd290-161">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="fd290-161">The type of risk</span></span>|
|<span data-ttu-id="fd290-162">userAgent</span><span class="sxs-lookup"><span data-stu-id="fd290-162">userAgent</span></span>|<span data-ttu-id="fd290-163">string</span><span class="sxs-lookup"><span data-stu-id="fd290-163">string</span></span>| <span data-ttu-id="fd290-164">A cadeia de caracteres do agente do usuário do navegador</span><span class="sxs-lookup"><span data-stu-id="fd290-164">The browser's user agent string</span></span>|
|<span data-ttu-id="fd290-165">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="fd290-165">userDisplayName</span></span>|<span data-ttu-id="fd290-166">string</span><span class="sxs-lookup"><span data-stu-id="fd290-166">string</span></span>| <span data-ttu-id="fd290-167">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="fd290-167">The name of the user at risk</span></span>|
|<span data-ttu-id="fd290-168">userId</span><span class="sxs-lookup"><span data-stu-id="fd290-168">userId</span></span>|<span data-ttu-id="fd290-169">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd290-169">string</span></span>| <span data-ttu-id="fd290-170">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="fd290-170">The id of the user at risk</span></span>|
|<span data-ttu-id="fd290-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fd290-171">userPrincipalName</span></span>|<span data-ttu-id="fd290-172">string</span><span class="sxs-lookup"><span data-stu-id="fd290-172">string</span></span>| <span data-ttu-id="fd290-173">O nome principal de usuário do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="fd290-173">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd290-174">Relações</span><span class="sxs-lookup"><span data-stu-id="fd290-174">Relationships</span></span>
| <span data-ttu-id="fd290-175">Relação</span><span class="sxs-lookup"><span data-stu-id="fd290-175">Relationship</span></span> | <span data-ttu-id="fd290-176">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd290-176">Type</span></span>   |<span data-ttu-id="fd290-177">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd290-177">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd290-178">impactedUser</span><span class="sxs-lookup"><span data-stu-id="fd290-178">impactedUser</span></span>|[<span data-ttu-id="fd290-179">Usuário</span><span class="sxs-lookup"><span data-stu-id="fd290-179">user</span></span>](user.md)| <span data-ttu-id="fd290-p103">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="fd290-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fd290-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fd290-182">JSON representation</span></span>

<span data-ttu-id="fd290-183">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fd290-183">Here is a JSON representation of the resource.</span></span>

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
