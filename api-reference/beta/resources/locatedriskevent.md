---
title: tipo de recurso locatedRiskEvent
description: 'Um evento de risco detectado pela proteção de identidade do Azure Active Directory com base nos dados do local. Os tipos de eventos de risco localizados incluem:'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: 461f20233e92edca48b9dd51fa417b33ab9f386c
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48404669"
---
# <a name="locatedriskevent-resource-type"></a><span data-ttu-id="5e6d5-104">tipo de recurso locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="5e6d5-104">locatedRiskEvent resource type</span></span>

<span data-ttu-id="5e6d5-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e6d5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e6d5-106">Um evento de risco detectado pela [proteção de identidade do Azure Active Directory](/azure/active-directory/identity-protection/overview-identity-protection) com base nos dados do local.</span><span class="sxs-lookup"><span data-stu-id="5e6d5-106">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) that is based on location data.</span></span> <span data-ttu-id="5e6d5-107">Os tipos de eventos de risco localizados incluem:</span><span class="sxs-lookup"><span data-stu-id="5e6d5-107">Located risk event types include:</span></span>
* [<span data-ttu-id="5e6d5-108">entradas de endereços IP anônimos</span><span class="sxs-lookup"><span data-stu-id="5e6d5-108">sign-ins from anonymous IP addresses</span></span>](anonymousipriskevent.md)
* [<span data-ttu-id="5e6d5-109">entradas de dispositivos infectados por malware</span><span class="sxs-lookup"><span data-stu-id="5e6d5-109">sign-ins from malware-infected devices</span></span>](malwareriskevent.md)
* [<span data-ttu-id="5e6d5-110">impossível viajar para locais atypical</span><span class="sxs-lookup"><span data-stu-id="5e6d5-110">impossible travel to atypical locations</span></span>](impossibletravelriskevent.md)
* [<span data-ttu-id="5e6d5-111">entradas de endereços IP suspeitos</span><span class="sxs-lookup"><span data-stu-id="5e6d5-111">sign-ins from suspicious IP addresses</span></span>](suspiciousipriskevent.md)
* <span data-ttu-id="5e6d5-112">[entradas de locais desconhecidos](unfamiliarlocationriskevent.md) As informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Azure ad](/azure/active-directory/identity-protection/overview-identity-protection).</span><span class="sxs-lookup"><span data-stu-id="5e6d5-112">[sign-ins from unfamiliar locations](unfamiliarlocationriskevent.md) Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="5e6d5-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="5e6d5-113">Methods</span></span>

| <span data-ttu-id="5e6d5-114">Método</span><span class="sxs-lookup"><span data-stu-id="5e6d5-114">Method</span></span>           | <span data-ttu-id="5e6d5-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5e6d5-115">Return Type</span></span>    |<span data-ttu-id="5e6d5-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e6d5-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5e6d5-117">Obter locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="5e6d5-117">Get locatedRiskEvent</span></span>](../api/locatedriskevent-get.md) | [<span data-ttu-id="5e6d5-118">locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="5e6d5-118">locatedRiskEvent</span></span>](locatedriskevent.md) |<span data-ttu-id="5e6d5-119">Leia as propriedades e os relacionamentos do objeto locatedRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="5e6d5-119">Read properties and relationships of locatedRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5e6d5-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5e6d5-120">Properties</span></span>
| <span data-ttu-id="5e6d5-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e6d5-121">Property</span></span>     | <span data-ttu-id="5e6d5-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e6d5-122">Type</span></span>   |<span data-ttu-id="5e6d5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e6d5-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e6d5-124">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e6d5-124">closedDateTime</span></span>|<span data-ttu-id="5e6d5-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e6d5-125">dateTimeOffset</span></span>| <span data-ttu-id="5e6d5-126">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="5e6d5-126">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="5e6d5-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5e6d5-127">createdDateTime</span></span>|<span data-ttu-id="5e6d5-128">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e6d5-128">dateTimeOffset</span></span>| <span data-ttu-id="5e6d5-129">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="5e6d5-129">The date and time that the risk event was created.</span></span> <span data-ttu-id="5e6d5-130">Isso é sempre maior que ou igual ao DateTime do evento de risco propriamente dito.</span><span class="sxs-lookup"><span data-stu-id="5e6d5-130">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="5e6d5-131">Esta é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="5e6d5-131">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="5e6d5-132">id</span><span class="sxs-lookup"><span data-stu-id="5e6d5-132">id</span></span>|<span data-ttu-id="5e6d5-133">string</span><span class="sxs-lookup"><span data-stu-id="5e6d5-133">string</span></span>| <span data-ttu-id="5e6d5-134">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="5e6d5-134">Read-only</span></span>|
|<span data-ttu-id="5e6d5-135">ipAddress</span><span class="sxs-lookup"><span data-stu-id="5e6d5-135">ipAddress</span></span>|<span data-ttu-id="5e6d5-136">string</span><span class="sxs-lookup"><span data-stu-id="5e6d5-136">string</span></span>| <span data-ttu-id="5e6d5-137">O endereço IP do logon</span><span class="sxs-lookup"><span data-stu-id="5e6d5-137">The IP address of the sign-in</span></span>|
|<span data-ttu-id="5e6d5-138">location</span><span class="sxs-lookup"><span data-stu-id="5e6d5-138">location</span></span>|<span data-ttu-id="5e6d5-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e6d5-139">string</span></span>| <span data-ttu-id="5e6d5-140">O local anexado ao endereço IP do logon</span><span class="sxs-lookup"><span data-stu-id="5e6d5-140">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="5e6d5-141">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="5e6d5-141">riskEventDateTime</span></span>|<span data-ttu-id="5e6d5-142">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e6d5-142">dateTimeOffset</span></span>| <span data-ttu-id="5e6d5-143">A data e a hora em que o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="5e6d5-143">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="5e6d5-144">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="5e6d5-144">riskEventStatus</span></span>|<span data-ttu-id="5e6d5-145">string</span><span class="sxs-lookup"><span data-stu-id="5e6d5-145">string</span></span>| <span data-ttu-id="5e6d5-146">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="5e6d5-146">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="5e6d5-147">riskLevel</span><span class="sxs-lookup"><span data-stu-id="5e6d5-147">riskLevel</span></span>|<span data-ttu-id="5e6d5-148">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e6d5-148">string</span></span>| <span data-ttu-id="5e6d5-149">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="5e6d5-149">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="5e6d5-150">riskEventType</span><span class="sxs-lookup"><span data-stu-id="5e6d5-150">riskEventType</span></span>|<span data-ttu-id="5e6d5-151">string</span><span class="sxs-lookup"><span data-stu-id="5e6d5-151">string</span></span>| <span data-ttu-id="5e6d5-152">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="5e6d5-152">The type of risk</span></span>|
|<span data-ttu-id="5e6d5-153">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="5e6d5-153">userDisplayName</span></span>|<span data-ttu-id="5e6d5-154">string</span><span class="sxs-lookup"><span data-stu-id="5e6d5-154">string</span></span>| <span data-ttu-id="5e6d5-155">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="5e6d5-155">The name of the user at risk</span></span>|
|<span data-ttu-id="5e6d5-156">userId</span><span class="sxs-lookup"><span data-stu-id="5e6d5-156">userId</span></span>|<span data-ttu-id="5e6d5-157">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e6d5-157">string</span></span>| <span data-ttu-id="5e6d5-158">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="5e6d5-158">The id of the user at risk</span></span>|
|<span data-ttu-id="5e6d5-159">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5e6d5-159">userPrincipalName</span></span>|<span data-ttu-id="5e6d5-160">string</span><span class="sxs-lookup"><span data-stu-id="5e6d5-160">string</span></span>| <span data-ttu-id="5e6d5-161">O nome principal de usuário do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="5e6d5-161">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e6d5-162">Relações</span><span class="sxs-lookup"><span data-stu-id="5e6d5-162">Relationships</span></span>
| <span data-ttu-id="5e6d5-163">Relação</span><span class="sxs-lookup"><span data-stu-id="5e6d5-163">Relationship</span></span> | <span data-ttu-id="5e6d5-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e6d5-164">Type</span></span>   |<span data-ttu-id="5e6d5-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e6d5-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e6d5-166">impactedUser</span><span class="sxs-lookup"><span data-stu-id="5e6d5-166">impactedUser</span></span>|[<span data-ttu-id="5e6d5-167">user</span><span class="sxs-lookup"><span data-stu-id="5e6d5-167">user</span></span>](user.md)| <span data-ttu-id="5e6d5-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="5e6d5-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e6d5-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5e6d5-170">JSON representation</span></span>

<span data-ttu-id="5e6d5-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5e6d5-171">Here is a JSON representation of the resource.</span></span>

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