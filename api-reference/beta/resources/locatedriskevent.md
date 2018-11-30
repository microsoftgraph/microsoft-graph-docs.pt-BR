---
title: tipo de recurso de locatedRiskEvent
description: 'Um evento de risco detectado pelo Windows Azure Active Directory identidade proteção baseado nos dados de local. Os tipos de evento de risco localizado incluem:'
ms.openlocfilehash: e84cff5985905977b6b1eeb75a9ef9703a2a2078
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036062"
---
# <a name="locatedriskevent-resource-type"></a><span data-ttu-id="27806-104">tipo de recurso de locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="27806-104">locatedRiskEvent resource type</span></span>

> <span data-ttu-id="27806-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="27806-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27806-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="27806-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="27806-107">Um evento de risco detectado pelo [Windows Azure Active Directory proteção de identidade](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) que é baseado em dados de local.</span><span class="sxs-lookup"><span data-stu-id="27806-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) that is based on location data.</span></span> <span data-ttu-id="27806-108">Os tipos de evento de risco localizado incluem:</span><span class="sxs-lookup"><span data-stu-id="27806-108">Located risk event types include:</span></span>
* [<span data-ttu-id="27806-109">entradas de endereços IP anônimos</span><span class="sxs-lookup"><span data-stu-id="27806-109">sign-ins from anonymous IP addresses</span></span>](anonymousipriskevent.md)
* [<span data-ttu-id="27806-110">entradas de dispositivos infectados por malware</span><span class="sxs-lookup"><span data-stu-id="27806-110">sign-ins from malware-infected devices</span></span>](malwareriskevent.md)
* [<span data-ttu-id="27806-111">Impossível viajar para locais atípicos</span><span class="sxs-lookup"><span data-stu-id="27806-111">impossible travel to atypical locations</span></span>](impossibletravelriskevent.md)
* [<span data-ttu-id="27806-112">entradas de endereços IP suspeitos</span><span class="sxs-lookup"><span data-stu-id="27806-112">sign-ins from suspicious IP addresses</span></span>](suspiciousipriskevent.md)
* <span data-ttu-id="27806-113">[entradas de familiarizado locais](unfamiliarlocationriskevent.md) Informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Windows Azure AD](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="27806-113">[sign-ins from unfamiliar locations](unfamiliarlocationriskevent.md) Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="27806-114">Métodos</span><span class="sxs-lookup"><span data-stu-id="27806-114">Methods</span></span>

| <span data-ttu-id="27806-115">Método</span><span class="sxs-lookup"><span data-stu-id="27806-115">Method</span></span>           | <span data-ttu-id="27806-116">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="27806-116">Return Type</span></span>    |<span data-ttu-id="27806-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="27806-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="27806-118">Obter locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="27806-118">Get locatedRiskEvent</span></span>](../api/locatedriskevent-get.md) | [<span data-ttu-id="27806-119">locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="27806-119">locatedRiskEvent</span></span>](locatedriskevent.md) |<span data-ttu-id="27806-120">Leia as propriedades e os relacionamentos do objeto locatedRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="27806-120">Read properties and relationships of locatedRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="27806-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="27806-121">Properties</span></span>
| <span data-ttu-id="27806-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27806-122">Property</span></span>     | <span data-ttu-id="27806-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="27806-123">Type</span></span>   |<span data-ttu-id="27806-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="27806-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27806-125">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="27806-125">closedDateTime</span></span>|<span data-ttu-id="27806-126">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27806-126">dateTimeOffset</span></span>| <span data-ttu-id="27806-127">A data e hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="27806-127">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="27806-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27806-128">createdDateTime</span></span>|<span data-ttu-id="27806-129">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27806-129">dateTimeOffset</span></span>| <span data-ttu-id="27806-130">A data e hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="27806-130">The date and time that the risk event was created.</span></span> <span data-ttu-id="27806-131">Sempre é maior ou igual ao datetime do evento risco em si.</span><span class="sxs-lookup"><span data-stu-id="27806-131">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="27806-132">Esta é a propriedade correta a ser usado como um filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="27806-132">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="27806-133">id</span><span class="sxs-lookup"><span data-stu-id="27806-133">id</span></span>|<span data-ttu-id="27806-134">string</span><span class="sxs-lookup"><span data-stu-id="27806-134">string</span></span>| <span data-ttu-id="27806-135">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="27806-135">Read-only</span></span>|
|<span data-ttu-id="27806-136">ipAddress</span><span class="sxs-lookup"><span data-stu-id="27806-136">ipAddress</span></span>|<span data-ttu-id="27806-137">string</span><span class="sxs-lookup"><span data-stu-id="27806-137">string</span></span>| <span data-ttu-id="27806-138">O endereço IP do sign-in</span><span class="sxs-lookup"><span data-stu-id="27806-138">The IP address of the sign-in</span></span>|
|<span data-ttu-id="27806-139">location</span><span class="sxs-lookup"><span data-stu-id="27806-139">location</span></span>|<span data-ttu-id="27806-140">string</span><span class="sxs-lookup"><span data-stu-id="27806-140">string</span></span>| <span data-ttu-id="27806-141">O local anexado ao endereço IP do sign-in</span><span class="sxs-lookup"><span data-stu-id="27806-141">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="27806-142">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="27806-142">riskEventDateTime</span></span>|<span data-ttu-id="27806-143">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27806-143">dateTimeOffset</span></span>| <span data-ttu-id="27806-144">A data e hora quando o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="27806-144">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="27806-145">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="27806-145">riskEventStatus</span></span>|<span data-ttu-id="27806-146">string</span><span class="sxs-lookup"><span data-stu-id="27806-146">string</span></span>| <span data-ttu-id="27806-147">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="27806-147">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="27806-148">riskLevel</span><span class="sxs-lookup"><span data-stu-id="27806-148">riskLevel</span></span>|<span data-ttu-id="27806-149">string</span><span class="sxs-lookup"><span data-stu-id="27806-149">string</span></span>| <span data-ttu-id="27806-150">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="27806-150">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="27806-151">riskEventType</span><span class="sxs-lookup"><span data-stu-id="27806-151">riskEventType</span></span>|<span data-ttu-id="27806-152">string</span><span class="sxs-lookup"><span data-stu-id="27806-152">string</span></span>| <span data-ttu-id="27806-153">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="27806-153">The type of risk</span></span>|
|<span data-ttu-id="27806-154">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="27806-154">userDisplayName</span></span>|<span data-ttu-id="27806-155">string</span><span class="sxs-lookup"><span data-stu-id="27806-155">string</span></span>| <span data-ttu-id="27806-156">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="27806-156">The name of the user at risk</span></span>|
|<span data-ttu-id="27806-157">userId</span><span class="sxs-lookup"><span data-stu-id="27806-157">userId</span></span>|<span data-ttu-id="27806-158">string</span><span class="sxs-lookup"><span data-stu-id="27806-158">string</span></span>| <span data-ttu-id="27806-159">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="27806-159">The id of the user at risk</span></span>|
|<span data-ttu-id="27806-160">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="27806-160">userPrincipalName</span></span>|<span data-ttu-id="27806-161">string</span><span class="sxs-lookup"><span data-stu-id="27806-161">string</span></span>| <span data-ttu-id="27806-162">O nome de usuário principal do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="27806-162">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="27806-163">Relações</span><span class="sxs-lookup"><span data-stu-id="27806-163">Relationships</span></span>
| <span data-ttu-id="27806-164">Relação</span><span class="sxs-lookup"><span data-stu-id="27806-164">Relationship</span></span> | <span data-ttu-id="27806-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="27806-165">Type</span></span>   |<span data-ttu-id="27806-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="27806-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27806-167">impactedUser</span><span class="sxs-lookup"><span data-stu-id="27806-167">impactedUser</span></span>|[<span data-ttu-id="27806-168">user</span><span class="sxs-lookup"><span data-stu-id="27806-168">user</span></span>](user.md)| <span data-ttu-id="27806-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="27806-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27806-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="27806-171">JSON representation</span></span>

<span data-ttu-id="27806-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="27806-172">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "locatedRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->