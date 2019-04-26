---
title: tipo de recurso locatedRiskEvent
description: 'Um evento de risco detectado pela proteção de identidade do Azure Active Directory com base nos dados do local. Os tipos de eventos de risco localizados incluem:'
localization_priority: Normal
ms.openlocfilehash: 2c7503c08700a0d7c2d2ad67e8868901bdb008e2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345354"
---
# <a name="locatedriskevent-resource-type"></a><span data-ttu-id="070cb-104">tipo de recurso locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="070cb-104">locatedRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="070cb-105">Um evento de risco detectado pela [proteção de identidade do Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) com base nos dados do local.</span><span class="sxs-lookup"><span data-stu-id="070cb-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) that is based on location data.</span></span> <span data-ttu-id="070cb-106">Os tipos de eventos de risco localizados incluem:</span><span class="sxs-lookup"><span data-stu-id="070cb-106">Located risk event types include:</span></span>
* [<span data-ttu-id="070cb-107">entradas de endereços IP anônimos</span><span class="sxs-lookup"><span data-stu-id="070cb-107">sign-ins from anonymous IP addresses</span></span>](anonymousipriskevent.md)
* [<span data-ttu-id="070cb-108">entradas de dispositivos infectados por malware</span><span class="sxs-lookup"><span data-stu-id="070cb-108">sign-ins from malware-infected devices</span></span>](malwareriskevent.md)
* [<span data-ttu-id="070cb-109">impossível viajar para locais atypical</span><span class="sxs-lookup"><span data-stu-id="070cb-109">impossible travel to atypical locations</span></span>](impossibletravelriskevent.md)
* [<span data-ttu-id="070cb-110">entradas de endereços IP suspeitos</span><span class="sxs-lookup"><span data-stu-id="070cb-110">sign-ins from suspicious IP addresses</span></span>](suspiciousipriskevent.md)
* <span data-ttu-id="070cb-111">[entradas de locais](unfamiliarlocationriskevent.md) desconhecidos As informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Azure ad](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="070cb-111">[sign-ins from unfamiliar locations](unfamiliarlocationriskevent.md) Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="070cb-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="070cb-112">Methods</span></span>

| <span data-ttu-id="070cb-113">Método</span><span class="sxs-lookup"><span data-stu-id="070cb-113">Method</span></span>           | <span data-ttu-id="070cb-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="070cb-114">Return Type</span></span>    |<span data-ttu-id="070cb-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="070cb-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="070cb-116">Obter locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="070cb-116">Get locatedRiskEvent</span></span>](../api/locatedriskevent-get.md) | [<span data-ttu-id="070cb-117">locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="070cb-117">locatedRiskEvent</span></span>](locatedriskevent.md) |<span data-ttu-id="070cb-118">Leia as propriedades e os relacionamentos do objeto locatedRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="070cb-118">Read properties and relationships of locatedRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="070cb-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="070cb-119">Properties</span></span>
| <span data-ttu-id="070cb-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="070cb-120">Property</span></span>     | <span data-ttu-id="070cb-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="070cb-121">Type</span></span>   |<span data-ttu-id="070cb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="070cb-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="070cb-123">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="070cb-123">closedDateTime</span></span>|<span data-ttu-id="070cb-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="070cb-124">dateTimeOffset</span></span>| <span data-ttu-id="070cb-125">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="070cb-125">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="070cb-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="070cb-126">createdDateTime</span></span>|<span data-ttu-id="070cb-127">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="070cb-127">dateTimeOffset</span></span>| <span data-ttu-id="070cb-128">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="070cb-128">The date and time that the risk event was created.</span></span> <span data-ttu-id="070cb-129">Isso é sempre maior que ou igual ao DateTime do evento de risco propriamente dito.</span><span class="sxs-lookup"><span data-stu-id="070cb-129">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="070cb-130">Esta é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="070cb-130">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="070cb-131">id</span><span class="sxs-lookup"><span data-stu-id="070cb-131">id</span></span>|<span data-ttu-id="070cb-132">string</span><span class="sxs-lookup"><span data-stu-id="070cb-132">string</span></span>| <span data-ttu-id="070cb-133">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="070cb-133">Read-only</span></span>|
|<span data-ttu-id="070cb-134">ipAddress</span><span class="sxs-lookup"><span data-stu-id="070cb-134">ipAddress</span></span>|<span data-ttu-id="070cb-135">string</span><span class="sxs-lookup"><span data-stu-id="070cb-135">string</span></span>| <span data-ttu-id="070cb-136">O endereço IP do logon</span><span class="sxs-lookup"><span data-stu-id="070cb-136">The IP address of the sign-in</span></span>|
|<span data-ttu-id="070cb-137">location</span><span class="sxs-lookup"><span data-stu-id="070cb-137">location</span></span>|<span data-ttu-id="070cb-138">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="070cb-138">string</span></span>| <span data-ttu-id="070cb-139">O local anexado ao endereço IP do logon</span><span class="sxs-lookup"><span data-stu-id="070cb-139">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="070cb-140">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="070cb-140">riskEventDateTime</span></span>|<span data-ttu-id="070cb-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="070cb-141">dateTimeOffset</span></span>| <span data-ttu-id="070cb-142">A data e a hora em que o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="070cb-142">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="070cb-143">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="070cb-143">riskEventStatus</span></span>|<span data-ttu-id="070cb-144">string</span><span class="sxs-lookup"><span data-stu-id="070cb-144">string</span></span>| <span data-ttu-id="070cb-145">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="070cb-145">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="070cb-146">riskLevel</span><span class="sxs-lookup"><span data-stu-id="070cb-146">riskLevel</span></span>|<span data-ttu-id="070cb-147">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="070cb-147">string</span></span>| <span data-ttu-id="070cb-148">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="070cb-148">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="070cb-149">riskEventType</span><span class="sxs-lookup"><span data-stu-id="070cb-149">riskEventType</span></span>|<span data-ttu-id="070cb-150">string</span><span class="sxs-lookup"><span data-stu-id="070cb-150">string</span></span>| <span data-ttu-id="070cb-151">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="070cb-151">The type of risk</span></span>|
|<span data-ttu-id="070cb-152">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="070cb-152">userDisplayName</span></span>|<span data-ttu-id="070cb-153">string</span><span class="sxs-lookup"><span data-stu-id="070cb-153">string</span></span>| <span data-ttu-id="070cb-154">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="070cb-154">The name of the user at risk</span></span>|
|<span data-ttu-id="070cb-155">userId</span><span class="sxs-lookup"><span data-stu-id="070cb-155">userId</span></span>|<span data-ttu-id="070cb-156">string</span><span class="sxs-lookup"><span data-stu-id="070cb-156">string</span></span>| <span data-ttu-id="070cb-157">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="070cb-157">The id of the user at risk</span></span>|
|<span data-ttu-id="070cb-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="070cb-158">userPrincipalName</span></span>|<span data-ttu-id="070cb-159">string</span><span class="sxs-lookup"><span data-stu-id="070cb-159">string</span></span>| <span data-ttu-id="070cb-160">O nome principal de usuário do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="070cb-160">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="070cb-161">Relações</span><span class="sxs-lookup"><span data-stu-id="070cb-161">Relationships</span></span>
| <span data-ttu-id="070cb-162">Relação</span><span class="sxs-lookup"><span data-stu-id="070cb-162">Relationship</span></span> | <span data-ttu-id="070cb-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="070cb-163">Type</span></span>   |<span data-ttu-id="070cb-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="070cb-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="070cb-165">impactedUser</span><span class="sxs-lookup"><span data-stu-id="070cb-165">impactedUser</span></span>|[<span data-ttu-id="070cb-166">user</span><span class="sxs-lookup"><span data-stu-id="070cb-166">user</span></span>](user.md)| <span data-ttu-id="070cb-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="070cb-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="070cb-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="070cb-169">JSON representation</span></span>

<span data-ttu-id="070cb-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="070cb-170">Here is a JSON representation of the resource.</span></span>

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
