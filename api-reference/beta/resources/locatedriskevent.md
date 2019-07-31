---
title: tipo de recurso locatedRiskEvent
description: 'Um evento de risco detectado pela proteção de identidade do Azure Active Directory com base nos dados do local. Os tipos de eventos de risco localizados incluem:'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e024b5311d6385888e7ed8e53ba9e37e8b2d2ed5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966983"
---
# <a name="locatedriskevent-resource-type"></a><span data-ttu-id="2aea9-104">tipo de recurso locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="2aea9-104">locatedRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2aea9-105">Um evento de risco detectado pela [proteção de identidade do Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) com base nos dados do local.</span><span class="sxs-lookup"><span data-stu-id="2aea9-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) that is based on location data.</span></span> <span data-ttu-id="2aea9-106">Os tipos de eventos de risco localizados incluem:</span><span class="sxs-lookup"><span data-stu-id="2aea9-106">Located risk event types include:</span></span>
* [<span data-ttu-id="2aea9-107">entradas de endereços IP anônimos</span><span class="sxs-lookup"><span data-stu-id="2aea9-107">sign-ins from anonymous IP addresses</span></span>](anonymousipriskevent.md)
* [<span data-ttu-id="2aea9-108">entradas de dispositivos infectados por malware</span><span class="sxs-lookup"><span data-stu-id="2aea9-108">sign-ins from malware-infected devices</span></span>](malwareriskevent.md)
* [<span data-ttu-id="2aea9-109">impossível viajar para locais atypical</span><span class="sxs-lookup"><span data-stu-id="2aea9-109">impossible travel to atypical locations</span></span>](impossibletravelriskevent.md)
* [<span data-ttu-id="2aea9-110">entradas de endereços IP suspeitos</span><span class="sxs-lookup"><span data-stu-id="2aea9-110">sign-ins from suspicious IP addresses</span></span>](suspiciousipriskevent.md)
* <span data-ttu-id="2aea9-111">[entradas de locais](unfamiliarlocationriskevent.md) desconhecidos As informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Azure ad](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="2aea9-111">[sign-ins from unfamiliar locations](unfamiliarlocationriskevent.md) Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="2aea9-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="2aea9-112">Methods</span></span>

| <span data-ttu-id="2aea9-113">Método</span><span class="sxs-lookup"><span data-stu-id="2aea9-113">Method</span></span>           | <span data-ttu-id="2aea9-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2aea9-114">Return Type</span></span>    |<span data-ttu-id="2aea9-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="2aea9-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2aea9-116">Obter locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="2aea9-116">Get locatedRiskEvent</span></span>](../api/locatedriskevent-get.md) | [<span data-ttu-id="2aea9-117">locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="2aea9-117">locatedRiskEvent</span></span>](locatedriskevent.md) |<span data-ttu-id="2aea9-118">Leia as propriedades e os relacionamentos do objeto locatedRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="2aea9-118">Read properties and relationships of locatedRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2aea9-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2aea9-119">Properties</span></span>
| <span data-ttu-id="2aea9-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2aea9-120">Property</span></span>     | <span data-ttu-id="2aea9-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="2aea9-121">Type</span></span>   |<span data-ttu-id="2aea9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2aea9-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2aea9-123">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="2aea9-123">closedDateTime</span></span>|<span data-ttu-id="2aea9-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2aea9-124">dateTimeOffset</span></span>| <span data-ttu-id="2aea9-125">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="2aea9-125">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="2aea9-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2aea9-126">createdDateTime</span></span>|<span data-ttu-id="2aea9-127">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2aea9-127">dateTimeOffset</span></span>| <span data-ttu-id="2aea9-128">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="2aea9-128">The date and time that the risk event was created.</span></span> <span data-ttu-id="2aea9-129">Isso é sempre maior que ou igual ao DateTime do evento de risco propriamente dito.</span><span class="sxs-lookup"><span data-stu-id="2aea9-129">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="2aea9-130">Esta é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="2aea9-130">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="2aea9-131">id</span><span class="sxs-lookup"><span data-stu-id="2aea9-131">id</span></span>|<span data-ttu-id="2aea9-132">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2aea9-132">string</span></span>| <span data-ttu-id="2aea9-133">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="2aea9-133">Read-only</span></span>|
|<span data-ttu-id="2aea9-134">ipAddress</span><span class="sxs-lookup"><span data-stu-id="2aea9-134">ipAddress</span></span>|<span data-ttu-id="2aea9-135">string</span><span class="sxs-lookup"><span data-stu-id="2aea9-135">string</span></span>| <span data-ttu-id="2aea9-136">O endereço IP do logon</span><span class="sxs-lookup"><span data-stu-id="2aea9-136">The IP address of the sign-in</span></span>|
|<span data-ttu-id="2aea9-137">location</span><span class="sxs-lookup"><span data-stu-id="2aea9-137">location</span></span>|<span data-ttu-id="2aea9-138">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2aea9-138">string</span></span>| <span data-ttu-id="2aea9-139">O local anexado ao endereço IP do logon</span><span class="sxs-lookup"><span data-stu-id="2aea9-139">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="2aea9-140">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="2aea9-140">riskEventDateTime</span></span>|<span data-ttu-id="2aea9-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2aea9-141">dateTimeOffset</span></span>| <span data-ttu-id="2aea9-142">A data e a hora em que o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="2aea9-142">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="2aea9-143">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="2aea9-143">riskEventStatus</span></span>|<span data-ttu-id="2aea9-144">string</span><span class="sxs-lookup"><span data-stu-id="2aea9-144">string</span></span>| <span data-ttu-id="2aea9-145">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="2aea9-145">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="2aea9-146">riskLevel</span><span class="sxs-lookup"><span data-stu-id="2aea9-146">riskLevel</span></span>|<span data-ttu-id="2aea9-147">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2aea9-147">string</span></span>| <span data-ttu-id="2aea9-148">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="2aea9-148">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="2aea9-149">riskEventType</span><span class="sxs-lookup"><span data-stu-id="2aea9-149">riskEventType</span></span>|<span data-ttu-id="2aea9-150">string</span><span class="sxs-lookup"><span data-stu-id="2aea9-150">string</span></span>| <span data-ttu-id="2aea9-151">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="2aea9-151">The type of risk</span></span>|
|<span data-ttu-id="2aea9-152">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="2aea9-152">userDisplayName</span></span>|<span data-ttu-id="2aea9-153">string</span><span class="sxs-lookup"><span data-stu-id="2aea9-153">string</span></span>| <span data-ttu-id="2aea9-154">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="2aea9-154">The name of the user at risk</span></span>|
|<span data-ttu-id="2aea9-155">userId</span><span class="sxs-lookup"><span data-stu-id="2aea9-155">userId</span></span>|<span data-ttu-id="2aea9-156">string</span><span class="sxs-lookup"><span data-stu-id="2aea9-156">string</span></span>| <span data-ttu-id="2aea9-157">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="2aea9-157">The id of the user at risk</span></span>|
|<span data-ttu-id="2aea9-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2aea9-158">userPrincipalName</span></span>|<span data-ttu-id="2aea9-159">string</span><span class="sxs-lookup"><span data-stu-id="2aea9-159">string</span></span>| <span data-ttu-id="2aea9-160">O nome principal de usuário do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="2aea9-160">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="2aea9-161">Relações</span><span class="sxs-lookup"><span data-stu-id="2aea9-161">Relationships</span></span>
| <span data-ttu-id="2aea9-162">Relação</span><span class="sxs-lookup"><span data-stu-id="2aea9-162">Relationship</span></span> | <span data-ttu-id="2aea9-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="2aea9-163">Type</span></span>   |<span data-ttu-id="2aea9-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="2aea9-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2aea9-165">impactedUser</span><span class="sxs-lookup"><span data-stu-id="2aea9-165">impactedUser</span></span>|[<span data-ttu-id="2aea9-166">Usuário</span><span class="sxs-lookup"><span data-stu-id="2aea9-166">user</span></span>](user.md)| <span data-ttu-id="2aea9-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="2aea9-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2aea9-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2aea9-169">JSON representation</span></span>

<span data-ttu-id="2aea9-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2aea9-170">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
   "abstract": true,
   "keyProperty": "id",
   "baseType":"microsoft.graph.identityRiskEvent",
  "@odata.type": "microsoft.graph.locatedRiskEvent"
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
  "description": "locatedRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
