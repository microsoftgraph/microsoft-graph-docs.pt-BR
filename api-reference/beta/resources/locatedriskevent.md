---
title: tipo de recurso locatedRiskEvent
description: 'Um evento de risco detectado pela proteção de identidade do Azure Active Directory com base nos dados do local. Os tipos de eventos de risco localizados incluem:'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: 4fbad6d2b2cc736167f313ad6f70b8f0aea2e63b
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806545"
---
# <a name="locatedriskevent-resource-type"></a><span data-ttu-id="44be3-104">tipo de recurso locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="44be3-104">locatedRiskEvent resource type</span></span>

<span data-ttu-id="44be3-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44be3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44be3-106">Um evento de risco detectado pela [proteção de identidade do Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) com base nos dados do local.</span><span class="sxs-lookup"><span data-stu-id="44be3-106">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) that is based on location data.</span></span> <span data-ttu-id="44be3-107">Os tipos de eventos de risco localizados incluem:</span><span class="sxs-lookup"><span data-stu-id="44be3-107">Located risk event types include:</span></span>
* [<span data-ttu-id="44be3-108">entradas de endereços IP anônimos</span><span class="sxs-lookup"><span data-stu-id="44be3-108">sign-ins from anonymous IP addresses</span></span>](anonymousipriskevent.md)
* [<span data-ttu-id="44be3-109">entradas de dispositivos infectados por malware</span><span class="sxs-lookup"><span data-stu-id="44be3-109">sign-ins from malware-infected devices</span></span>](malwareriskevent.md)
* [<span data-ttu-id="44be3-110">impossível viajar para locais atypical</span><span class="sxs-lookup"><span data-stu-id="44be3-110">impossible travel to atypical locations</span></span>](impossibletravelriskevent.md)
* [<span data-ttu-id="44be3-111">entradas de endereços IP suspeitos</span><span class="sxs-lookup"><span data-stu-id="44be3-111">sign-ins from suspicious IP addresses</span></span>](suspiciousipriskevent.md)
* <span data-ttu-id="44be3-112">[entradas de locais desconhecidos](unfamiliarlocationriskevent.md) As informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Azure ad](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="44be3-112">[sign-ins from unfamiliar locations](unfamiliarlocationriskevent.md) Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="44be3-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="44be3-113">Methods</span></span>

| <span data-ttu-id="44be3-114">Método</span><span class="sxs-lookup"><span data-stu-id="44be3-114">Method</span></span>           | <span data-ttu-id="44be3-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="44be3-115">Return Type</span></span>    |<span data-ttu-id="44be3-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="44be3-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="44be3-117">Obter locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="44be3-117">Get locatedRiskEvent</span></span>](../api/locatedriskevent-get.md) | [<span data-ttu-id="44be3-118">locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="44be3-118">locatedRiskEvent</span></span>](locatedriskevent.md) |<span data-ttu-id="44be3-119">Leia as propriedades e os relacionamentos do objeto locatedRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="44be3-119">Read properties and relationships of locatedRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="44be3-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44be3-120">Properties</span></span>
| <span data-ttu-id="44be3-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44be3-121">Property</span></span>     | <span data-ttu-id="44be3-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="44be3-122">Type</span></span>   |<span data-ttu-id="44be3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="44be3-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44be3-124">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="44be3-124">closedDateTime</span></span>|<span data-ttu-id="44be3-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44be3-125">dateTimeOffset</span></span>| <span data-ttu-id="44be3-126">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="44be3-126">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="44be3-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44be3-127">createdDateTime</span></span>|<span data-ttu-id="44be3-128">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44be3-128">dateTimeOffset</span></span>| <span data-ttu-id="44be3-129">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="44be3-129">The date and time that the risk event was created.</span></span> <span data-ttu-id="44be3-130">Isso é sempre maior que ou igual ao DateTime do evento de risco propriamente dito.</span><span class="sxs-lookup"><span data-stu-id="44be3-130">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="44be3-131">Esta é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="44be3-131">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="44be3-132">id</span><span class="sxs-lookup"><span data-stu-id="44be3-132">id</span></span>|<span data-ttu-id="44be3-133">string</span><span class="sxs-lookup"><span data-stu-id="44be3-133">string</span></span>| <span data-ttu-id="44be3-134">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="44be3-134">Read-only</span></span>|
|<span data-ttu-id="44be3-135">ipAddress</span><span class="sxs-lookup"><span data-stu-id="44be3-135">ipAddress</span></span>|<span data-ttu-id="44be3-136">string</span><span class="sxs-lookup"><span data-stu-id="44be3-136">string</span></span>| <span data-ttu-id="44be3-137">O endereço IP do logon</span><span class="sxs-lookup"><span data-stu-id="44be3-137">The IP address of the sign-in</span></span>|
|<span data-ttu-id="44be3-138">location</span><span class="sxs-lookup"><span data-stu-id="44be3-138">location</span></span>|<span data-ttu-id="44be3-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44be3-139">string</span></span>| <span data-ttu-id="44be3-140">O local anexado ao endereço IP do logon</span><span class="sxs-lookup"><span data-stu-id="44be3-140">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="44be3-141">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="44be3-141">riskEventDateTime</span></span>|<span data-ttu-id="44be3-142">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44be3-142">dateTimeOffset</span></span>| <span data-ttu-id="44be3-143">A data e a hora em que o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="44be3-143">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="44be3-144">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="44be3-144">riskEventStatus</span></span>|<span data-ttu-id="44be3-145">string</span><span class="sxs-lookup"><span data-stu-id="44be3-145">string</span></span>| <span data-ttu-id="44be3-146">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="44be3-146">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="44be3-147">riskLevel</span><span class="sxs-lookup"><span data-stu-id="44be3-147">riskLevel</span></span>|<span data-ttu-id="44be3-148">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44be3-148">string</span></span>| <span data-ttu-id="44be3-149">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="44be3-149">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="44be3-150">riskEventType</span><span class="sxs-lookup"><span data-stu-id="44be3-150">riskEventType</span></span>|<span data-ttu-id="44be3-151">string</span><span class="sxs-lookup"><span data-stu-id="44be3-151">string</span></span>| <span data-ttu-id="44be3-152">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="44be3-152">The type of risk</span></span>|
|<span data-ttu-id="44be3-153">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="44be3-153">userDisplayName</span></span>|<span data-ttu-id="44be3-154">string</span><span class="sxs-lookup"><span data-stu-id="44be3-154">string</span></span>| <span data-ttu-id="44be3-155">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="44be3-155">The name of the user at risk</span></span>|
|<span data-ttu-id="44be3-156">userId</span><span class="sxs-lookup"><span data-stu-id="44be3-156">userId</span></span>|<span data-ttu-id="44be3-157">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44be3-157">string</span></span>| <span data-ttu-id="44be3-158">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="44be3-158">The id of the user at risk</span></span>|
|<span data-ttu-id="44be3-159">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="44be3-159">userPrincipalName</span></span>|<span data-ttu-id="44be3-160">string</span><span class="sxs-lookup"><span data-stu-id="44be3-160">string</span></span>| <span data-ttu-id="44be3-161">O nome principal de usuário do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="44be3-161">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="44be3-162">Relações</span><span class="sxs-lookup"><span data-stu-id="44be3-162">Relationships</span></span>
| <span data-ttu-id="44be3-163">Relação</span><span class="sxs-lookup"><span data-stu-id="44be3-163">Relationship</span></span> | <span data-ttu-id="44be3-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="44be3-164">Type</span></span>   |<span data-ttu-id="44be3-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="44be3-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44be3-166">impactedUser</span><span class="sxs-lookup"><span data-stu-id="44be3-166">impactedUser</span></span>|[<span data-ttu-id="44be3-167">user</span><span class="sxs-lookup"><span data-stu-id="44be3-167">user</span></span>](user.md)| <span data-ttu-id="44be3-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="44be3-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="44be3-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44be3-170">JSON representation</span></span>

<span data-ttu-id="44be3-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="44be3-171">Here is a JSON representation of the resource.</span></span>

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
