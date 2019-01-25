---
title: tipo de recurso de locatedRiskEvent
description: 'Um evento de risco detectado pelo Windows Azure Active Directory identidade proteção baseado nos dados de local. Os tipos de evento de risco localizado incluem:'
localization_priority: Normal
ms.openlocfilehash: 20fe76099c511483144b42e33fc260910debb5ed
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510257"
---
# <a name="locatedriskevent-resource-type"></a><span data-ttu-id="f9122-104">tipo de recurso de locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f9122-104">locatedRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9122-105">Um evento de risco detectado pelo [Windows Azure Active Directory proteção de identidade](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) que é baseado em dados de local.</span><span class="sxs-lookup"><span data-stu-id="f9122-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) that is based on location data.</span></span> <span data-ttu-id="f9122-106">Os tipos de evento de risco localizado incluem:</span><span class="sxs-lookup"><span data-stu-id="f9122-106">Located risk event types include:</span></span>
* [<span data-ttu-id="f9122-107">entradas de endereços IP anônimos</span><span class="sxs-lookup"><span data-stu-id="f9122-107">sign-ins from anonymous IP addresses</span></span>](anonymousipriskevent.md)
* [<span data-ttu-id="f9122-108">entradas de dispositivos infectados por malware</span><span class="sxs-lookup"><span data-stu-id="f9122-108">sign-ins from malware-infected devices</span></span>](malwareriskevent.md)
* [<span data-ttu-id="f9122-109">Impossível viajar para locais atípicos</span><span class="sxs-lookup"><span data-stu-id="f9122-109">impossible travel to atypical locations</span></span>](impossibletravelriskevent.md)
* [<span data-ttu-id="f9122-110">entradas de endereços IP suspeitos</span><span class="sxs-lookup"><span data-stu-id="f9122-110">sign-ins from suspicious IP addresses</span></span>](suspiciousipriskevent.md)
* <span data-ttu-id="f9122-111">[entradas de familiarizado locais](unfamiliarlocationriskevent.md) Informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Windows Azure AD](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="f9122-111">[sign-ins from unfamiliar locations](unfamiliarlocationriskevent.md) Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="f9122-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="f9122-112">Methods</span></span>

| <span data-ttu-id="f9122-113">Método</span><span class="sxs-lookup"><span data-stu-id="f9122-113">Method</span></span>           | <span data-ttu-id="f9122-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f9122-114">Return Type</span></span>    |<span data-ttu-id="f9122-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9122-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f9122-116">Obter locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f9122-116">Get locatedRiskEvent</span></span>](../api/locatedriskevent-get.md) | [<span data-ttu-id="f9122-117">locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f9122-117">locatedRiskEvent</span></span>](locatedriskevent.md) |<span data-ttu-id="f9122-118">Leia as propriedades e os relacionamentos do objeto locatedRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="f9122-118">Read properties and relationships of locatedRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f9122-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f9122-119">Properties</span></span>
| <span data-ttu-id="f9122-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9122-120">Property</span></span>     | <span data-ttu-id="f9122-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9122-121">Type</span></span>   |<span data-ttu-id="f9122-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9122-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9122-123">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9122-123">closedDateTime</span></span>|<span data-ttu-id="f9122-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9122-124">dateTimeOffset</span></span>| <span data-ttu-id="f9122-125">A data e hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="f9122-125">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="f9122-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f9122-126">createdDateTime</span></span>|<span data-ttu-id="f9122-127">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9122-127">dateTimeOffset</span></span>| <span data-ttu-id="f9122-128">A data e hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="f9122-128">The date and time that the risk event was created.</span></span> <span data-ttu-id="f9122-129">Sempre é maior ou igual ao datetime do evento risco em si.</span><span class="sxs-lookup"><span data-stu-id="f9122-129">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="f9122-130">Esta é a propriedade correta a ser usado como um filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="f9122-130">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="f9122-131">id</span><span class="sxs-lookup"><span data-stu-id="f9122-131">id</span></span>|<span data-ttu-id="f9122-132">string</span><span class="sxs-lookup"><span data-stu-id="f9122-132">string</span></span>| <span data-ttu-id="f9122-133">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="f9122-133">Read-only</span></span>|
|<span data-ttu-id="f9122-134">ipAddress</span><span class="sxs-lookup"><span data-stu-id="f9122-134">ipAddress</span></span>|<span data-ttu-id="f9122-135">string</span><span class="sxs-lookup"><span data-stu-id="f9122-135">string</span></span>| <span data-ttu-id="f9122-136">O endereço IP do sign-in</span><span class="sxs-lookup"><span data-stu-id="f9122-136">The IP address of the sign-in</span></span>|
|<span data-ttu-id="f9122-137">location</span><span class="sxs-lookup"><span data-stu-id="f9122-137">location</span></span>|<span data-ttu-id="f9122-138">string</span><span class="sxs-lookup"><span data-stu-id="f9122-138">string</span></span>| <span data-ttu-id="f9122-139">O local anexado ao endereço IP do sign-in</span><span class="sxs-lookup"><span data-stu-id="f9122-139">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="f9122-140">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="f9122-140">riskEventDateTime</span></span>|<span data-ttu-id="f9122-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9122-141">dateTimeOffset</span></span>| <span data-ttu-id="f9122-142">A data e hora quando o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="f9122-142">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="f9122-143">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="f9122-143">riskEventStatus</span></span>|<span data-ttu-id="f9122-144">string</span><span class="sxs-lookup"><span data-stu-id="f9122-144">string</span></span>| <span data-ttu-id="f9122-145">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="f9122-145">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="f9122-146">riskLevel</span><span class="sxs-lookup"><span data-stu-id="f9122-146">riskLevel</span></span>|<span data-ttu-id="f9122-147">string</span><span class="sxs-lookup"><span data-stu-id="f9122-147">string</span></span>| <span data-ttu-id="f9122-148">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="f9122-148">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="f9122-149">riskEventType</span><span class="sxs-lookup"><span data-stu-id="f9122-149">riskEventType</span></span>|<span data-ttu-id="f9122-150">string</span><span class="sxs-lookup"><span data-stu-id="f9122-150">string</span></span>| <span data-ttu-id="f9122-151">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="f9122-151">The type of risk</span></span>|
|<span data-ttu-id="f9122-152">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f9122-152">userDisplayName</span></span>|<span data-ttu-id="f9122-153">string</span><span class="sxs-lookup"><span data-stu-id="f9122-153">string</span></span>| <span data-ttu-id="f9122-154">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="f9122-154">The name of the user at risk</span></span>|
|<span data-ttu-id="f9122-155">userId</span><span class="sxs-lookup"><span data-stu-id="f9122-155">userId</span></span>|<span data-ttu-id="f9122-156">string</span><span class="sxs-lookup"><span data-stu-id="f9122-156">string</span></span>| <span data-ttu-id="f9122-157">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="f9122-157">The id of the user at risk</span></span>|
|<span data-ttu-id="f9122-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f9122-158">userPrincipalName</span></span>|<span data-ttu-id="f9122-159">string</span><span class="sxs-lookup"><span data-stu-id="f9122-159">string</span></span>| <span data-ttu-id="f9122-160">O nome de usuário principal do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="f9122-160">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9122-161">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="f9122-161">Relationships</span></span>
| <span data-ttu-id="f9122-162">Relação</span><span class="sxs-lookup"><span data-stu-id="f9122-162">Relationship</span></span> | <span data-ttu-id="f9122-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9122-163">Type</span></span>   |<span data-ttu-id="f9122-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9122-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9122-165">impactedUser</span><span class="sxs-lookup"><span data-stu-id="f9122-165">impactedUser</span></span>|[<span data-ttu-id="f9122-166">user</span><span class="sxs-lookup"><span data-stu-id="f9122-166">user</span></span>](user.md)| <span data-ttu-id="f9122-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="f9122-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f9122-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f9122-169">JSON representation</span></span>

<span data-ttu-id="f9122-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f9122-170">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "userPrincipalName": "string"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/locatedriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
