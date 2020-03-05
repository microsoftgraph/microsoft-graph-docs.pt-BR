---
title: tipo de recurso impossibleTravelRiskEvent
description: Um evento de risco detectado pela proteção de identidade do Azure Active Directory onde dois logons de conta ocorrem de locais atypical para o usuário e não seria possível viajar entre os locais na duração entre os logons. complete information about eventos de risco podem ser encontrados na documentação de proteção de identidade do Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 39cfbc804fc786875b7cb1b6ee8058ae2a0571e0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496387"
---
# <a name="impossibletravelriskevent-resource-type"></a><span data-ttu-id="fbb07-103">tipo de recurso impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="fbb07-103">impossibleTravelRiskEvent resource type</span></span>

<span data-ttu-id="fbb07-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fbb07-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="fbb07-105">A API **identityRiskEvents** foi preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="fbb07-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="fbb07-106">Para obter detalhes, consulte [Preterition of the IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="fbb07-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="fbb07-107">Um evento de risco detectado pela [proteção de identidade do Active Directory do Azure](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) onde dois logons de conta ocorrem a partir de locais atypical para o usuário e seria impossível viajar entre os locais na duração entre as entradas. Complete as informações sobre os eventos de risco podem ser encontradas na [documentação do Azure ad Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="fbb07-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="fbb07-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="fbb07-108">Methods</span></span>

| <span data-ttu-id="fbb07-109">Método</span><span class="sxs-lookup"><span data-stu-id="fbb07-109">Method</span></span>           | <span data-ttu-id="fbb07-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fbb07-110">Return Type</span></span>    |<span data-ttu-id="fbb07-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbb07-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fbb07-112">Obter impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="fbb07-112">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="fbb07-113">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="fbb07-113">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="fbb07-114">Leia as propriedades e os relacionamentos do objeto impossibleTravelRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="fbb07-114">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fbb07-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fbb07-115">Properties</span></span>
| <span data-ttu-id="fbb07-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbb07-116">Property</span></span>     | <span data-ttu-id="fbb07-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbb07-117">Type</span></span>   |<span data-ttu-id="fbb07-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbb07-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbb07-119">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="fbb07-119">closedDateTime</span></span>|<span data-ttu-id="fbb07-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbb07-120">dateTimeOffset</span></span>| <span data-ttu-id="fbb07-121">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="fbb07-121">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="fbb07-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fbb07-122">createdDateTime</span></span>|<span data-ttu-id="fbb07-123">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbb07-123">dateTimeOffset</span></span>| <span data-ttu-id="fbb07-124">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="fbb07-124">The date and time that the risk event was created.</span></span> <span data-ttu-id="fbb07-125">Isso é sempre maior que ou igual ao DateTime do evento de risco propriamente dito.</span><span class="sxs-lookup"><span data-stu-id="fbb07-125">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="fbb07-126">Esta é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="fbb07-126">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="fbb07-127">deviceInformation</span><span class="sxs-lookup"><span data-stu-id="fbb07-127">deviceInformation</span></span>|<span data-ttu-id="fbb07-128">string</span><span class="sxs-lookup"><span data-stu-id="fbb07-128">string</span></span>| <span data-ttu-id="fbb07-129">Informações sobre o dispositivo</span><span class="sxs-lookup"><span data-stu-id="fbb07-129">Information about the device</span></span>|
|<span data-ttu-id="fbb07-130">id</span><span class="sxs-lookup"><span data-stu-id="fbb07-130">id</span></span>|<span data-ttu-id="fbb07-131">string</span><span class="sxs-lookup"><span data-stu-id="fbb07-131">string</span></span>| <span data-ttu-id="fbb07-132">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="fbb07-132">Read-only</span></span>|
|<span data-ttu-id="fbb07-133">ipAddress</span><span class="sxs-lookup"><span data-stu-id="fbb07-133">ipAddress</span></span>|<span data-ttu-id="fbb07-134">string</span><span class="sxs-lookup"><span data-stu-id="fbb07-134">string</span></span>| <span data-ttu-id="fbb07-135">O endereço IP da segunda entrada</span><span class="sxs-lookup"><span data-stu-id="fbb07-135">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="fbb07-136">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="fbb07-136">isAtypicalLocation</span></span>|<span data-ttu-id="fbb07-137">booliano</span><span class="sxs-lookup"><span data-stu-id="fbb07-137">boolean</span></span>| <span data-ttu-id="fbb07-138">Se um dos locais for atypical para o usuário</span><span class="sxs-lookup"><span data-stu-id="fbb07-138">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="fbb07-139">location</span><span class="sxs-lookup"><span data-stu-id="fbb07-139">location</span></span>|<span data-ttu-id="fbb07-140">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbb07-140">string</span></span>| <span data-ttu-id="fbb07-141">O local anexado ao endereço IP da segunda entrada</span><span class="sxs-lookup"><span data-stu-id="fbb07-141">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="fbb07-142">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="fbb07-142">previousIPAddress</span></span>|<span data-ttu-id="fbb07-143">string</span><span class="sxs-lookup"><span data-stu-id="fbb07-143">string</span></span>| <span data-ttu-id="fbb07-144">O endereço IP do primeiro logon</span><span class="sxs-lookup"><span data-stu-id="fbb07-144">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="fbb07-145">previousLocation</span><span class="sxs-lookup"><span data-stu-id="fbb07-145">previousLocation</span></span>|<span data-ttu-id="fbb07-146">string</span><span class="sxs-lookup"><span data-stu-id="fbb07-146">string</span></span>| <span data-ttu-id="fbb07-147">O local anexado ao endereço IP do primeiro logon</span><span class="sxs-lookup"><span data-stu-id="fbb07-147">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="fbb07-148">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="fbb07-148">previousSigninDateTime</span></span>|<span data-ttu-id="fbb07-149">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbb07-149">dateTimeOffset</span></span>| <span data-ttu-id="fbb07-150">A data e a hora da primeira entrada</span><span class="sxs-lookup"><span data-stu-id="fbb07-150">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="fbb07-151">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="fbb07-151">riskEventDateTime</span></span>|<span data-ttu-id="fbb07-152">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbb07-152">dateTimeOffset</span></span>| <span data-ttu-id="fbb07-153">A data e a hora da segunda entrada</span><span class="sxs-lookup"><span data-stu-id="fbb07-153">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="fbb07-154">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="fbb07-154">riskEventStatus</span></span>|<span data-ttu-id="fbb07-155">string</span><span class="sxs-lookup"><span data-stu-id="fbb07-155">string</span></span>| <span data-ttu-id="fbb07-156">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="fbb07-156">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="fbb07-157">riskLevel</span><span class="sxs-lookup"><span data-stu-id="fbb07-157">riskLevel</span></span>|<span data-ttu-id="fbb07-158">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbb07-158">string</span></span>| <span data-ttu-id="fbb07-159">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="fbb07-159">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="fbb07-160">riskEventType</span><span class="sxs-lookup"><span data-stu-id="fbb07-160">riskEventType</span></span>|<span data-ttu-id="fbb07-161">string</span><span class="sxs-lookup"><span data-stu-id="fbb07-161">string</span></span>| <span data-ttu-id="fbb07-162">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="fbb07-162">The type of risk</span></span>|
|<span data-ttu-id="fbb07-163">userAgent</span><span class="sxs-lookup"><span data-stu-id="fbb07-163">userAgent</span></span>|<span data-ttu-id="fbb07-164">string</span><span class="sxs-lookup"><span data-stu-id="fbb07-164">string</span></span>| <span data-ttu-id="fbb07-165">A cadeia de caracteres do agente do usuário do navegador</span><span class="sxs-lookup"><span data-stu-id="fbb07-165">The browser's user agent string</span></span>|
|<span data-ttu-id="fbb07-166">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="fbb07-166">userDisplayName</span></span>|<span data-ttu-id="fbb07-167">string</span><span class="sxs-lookup"><span data-stu-id="fbb07-167">string</span></span>| <span data-ttu-id="fbb07-168">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="fbb07-168">The name of the user at risk</span></span>|
|<span data-ttu-id="fbb07-169">userId</span><span class="sxs-lookup"><span data-stu-id="fbb07-169">userId</span></span>|<span data-ttu-id="fbb07-170">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbb07-170">string</span></span>| <span data-ttu-id="fbb07-171">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="fbb07-171">The id of the user at risk</span></span>|
|<span data-ttu-id="fbb07-172">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fbb07-172">userPrincipalName</span></span>|<span data-ttu-id="fbb07-173">string</span><span class="sxs-lookup"><span data-stu-id="fbb07-173">string</span></span>| <span data-ttu-id="fbb07-174">O nome principal de usuário do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="fbb07-174">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbb07-175">Relações</span><span class="sxs-lookup"><span data-stu-id="fbb07-175">Relationships</span></span>
| <span data-ttu-id="fbb07-176">Relação</span><span class="sxs-lookup"><span data-stu-id="fbb07-176">Relationship</span></span> | <span data-ttu-id="fbb07-177">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbb07-177">Type</span></span>   |<span data-ttu-id="fbb07-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbb07-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbb07-179">impactedUser</span><span class="sxs-lookup"><span data-stu-id="fbb07-179">impactedUser</span></span>|[<span data-ttu-id="fbb07-180">user</span><span class="sxs-lookup"><span data-stu-id="fbb07-180">user</span></span>](user.md)| <span data-ttu-id="fbb07-p103">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="fbb07-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fbb07-183">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fbb07-183">JSON representation</span></span>

<span data-ttu-id="fbb07-184">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fbb07-184">Here is a JSON representation of the resource.</span></span>

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
