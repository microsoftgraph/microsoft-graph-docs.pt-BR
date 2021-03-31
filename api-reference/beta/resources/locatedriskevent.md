---
title: tipo de recurso locatedRiskEvent
description: 'Um evento de risco detectado pela Proteção de Identidade do Azure Active Directory que se baseia nos dados de localização. Os tipos de eventos de risco localizados incluem:'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: cloudhandler
ms.openlocfilehash: 902dc864ea16bd677d0499711faa078131ca015d
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469455"
---
# <a name="locatedriskevent-resource-type"></a><span data-ttu-id="58adf-104">tipo de recurso locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="58adf-104">locatedRiskEvent resource type</span></span>

<span data-ttu-id="58adf-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58adf-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58adf-106">Um evento de risco detectado pela Proteção de Identidade [do Azure Active Directory](/azure/active-directory/identity-protection/overview-identity-protection) que se baseia nos dados de localização.</span><span class="sxs-lookup"><span data-stu-id="58adf-106">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) that is based on location data.</span></span> <span data-ttu-id="58adf-107">Os tipos de eventos de risco localizados incluem:</span><span class="sxs-lookup"><span data-stu-id="58adf-107">Located risk event types include:</span></span>
* [<span data-ttu-id="58adf-108">entrar de endereços IP anônimos</span><span class="sxs-lookup"><span data-stu-id="58adf-108">sign-ins from anonymous IP addresses</span></span>](anonymousipriskevent.md)
* [<span data-ttu-id="58adf-109">entrar de dispositivos infectados por malware</span><span class="sxs-lookup"><span data-stu-id="58adf-109">sign-ins from malware-infected devices</span></span>](malwareriskevent.md)
* [<span data-ttu-id="58adf-110">viagem impossível para locais atípicos</span><span class="sxs-lookup"><span data-stu-id="58adf-110">impossible travel to atypical locations</span></span>](impossibletravelriskevent.md)
* [<span data-ttu-id="58adf-111">entrar de endereços IP suspeitos</span><span class="sxs-lookup"><span data-stu-id="58adf-111">sign-ins from suspicious IP addresses</span></span>](suspiciousipriskevent.md)
* <span data-ttu-id="58adf-112">[entrar de locais desconhecidos](unfamiliarlocationriskevent.md) Informações completas sobre eventos de risco podem ser encontradas na documentação da Proteção de Identidade do [Azure AD.](/azure/active-directory/identity-protection/overview-identity-protection)</span><span class="sxs-lookup"><span data-stu-id="58adf-112">[sign-ins from unfamiliar locations](unfamiliarlocationriskevent.md) Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="58adf-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="58adf-113">Methods</span></span>

| <span data-ttu-id="58adf-114">Método</span><span class="sxs-lookup"><span data-stu-id="58adf-114">Method</span></span>           | <span data-ttu-id="58adf-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="58adf-115">Return Type</span></span>    |<span data-ttu-id="58adf-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="58adf-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="58adf-117">Obter locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="58adf-117">Get locatedRiskEvent</span></span>](../api/locatedriskevent-get.md) | [<span data-ttu-id="58adf-118">locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="58adf-118">locatedRiskEvent</span></span>](locatedriskevent.md) |<span data-ttu-id="58adf-119">Leia propriedades e relações do objeto locatedRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="58adf-119">Read properties and relationships of locatedRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="58adf-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="58adf-120">Properties</span></span>
| <span data-ttu-id="58adf-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58adf-121">Property</span></span>     | <span data-ttu-id="58adf-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="58adf-122">Type</span></span>   |<span data-ttu-id="58adf-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="58adf-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58adf-124">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="58adf-124">closedDateTime</span></span>|<span data-ttu-id="58adf-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58adf-125">dateTimeOffset</span></span>| <span data-ttu-id="58adf-126">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="58adf-126">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="58adf-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="58adf-127">createdDateTime</span></span>|<span data-ttu-id="58adf-128">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58adf-128">dateTimeOffset</span></span>| <span data-ttu-id="58adf-129">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="58adf-129">The date and time that the risk event was created.</span></span> <span data-ttu-id="58adf-130">Isso é sempre maior ou igual ao tempo de data do evento de risco em si.</span><span class="sxs-lookup"><span data-stu-id="58adf-130">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="58adf-131">Essa é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="58adf-131">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="58adf-132">id</span><span class="sxs-lookup"><span data-stu-id="58adf-132">id</span></span>|<span data-ttu-id="58adf-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58adf-133">string</span></span>| <span data-ttu-id="58adf-134">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="58adf-134">Read-only</span></span>|
|<span data-ttu-id="58adf-135">ipAddress</span><span class="sxs-lookup"><span data-stu-id="58adf-135">ipAddress</span></span>|<span data-ttu-id="58adf-136">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58adf-136">string</span></span>| <span data-ttu-id="58adf-137">O endereço IP da assinatura</span><span class="sxs-lookup"><span data-stu-id="58adf-137">The IP address of the sign-in</span></span>|
|<span data-ttu-id="58adf-138">location</span><span class="sxs-lookup"><span data-stu-id="58adf-138">location</span></span>|<span data-ttu-id="58adf-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58adf-139">string</span></span>| <span data-ttu-id="58adf-140">O local anexado ao endereço IP da login</span><span class="sxs-lookup"><span data-stu-id="58adf-140">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="58adf-141">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="58adf-141">riskEventDateTime</span></span>|<span data-ttu-id="58adf-142">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58adf-142">dateTimeOffset</span></span>| <span data-ttu-id="58adf-143">A data e a hora em que o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="58adf-143">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="58adf-144">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="58adf-144">riskEventStatus</span></span>|<span data-ttu-id="58adf-145">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58adf-145">string</span></span>| <span data-ttu-id="58adf-146">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="58adf-146">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="58adf-147">riskLevel</span><span class="sxs-lookup"><span data-stu-id="58adf-147">riskLevel</span></span>|<span data-ttu-id="58adf-148">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58adf-148">string</span></span>| <span data-ttu-id="58adf-149">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="58adf-149">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="58adf-150">riskEventType</span><span class="sxs-lookup"><span data-stu-id="58adf-150">riskEventType</span></span>|<span data-ttu-id="58adf-151">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58adf-151">string</span></span>| <span data-ttu-id="58adf-152">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="58adf-152">The type of risk</span></span>|
|<span data-ttu-id="58adf-153">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="58adf-153">userDisplayName</span></span>|<span data-ttu-id="58adf-154">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58adf-154">string</span></span>| <span data-ttu-id="58adf-155">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="58adf-155">The name of the user at risk</span></span>|
|<span data-ttu-id="58adf-156">userId</span><span class="sxs-lookup"><span data-stu-id="58adf-156">userId</span></span>|<span data-ttu-id="58adf-157">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58adf-157">string</span></span>| <span data-ttu-id="58adf-158">A id do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="58adf-158">The id of the user at risk</span></span>|
|<span data-ttu-id="58adf-159">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="58adf-159">userPrincipalName</span></span>|<span data-ttu-id="58adf-160">string</span><span class="sxs-lookup"><span data-stu-id="58adf-160">string</span></span>| <span data-ttu-id="58adf-161">O nome principal do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="58adf-161">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="58adf-162">Relações</span><span class="sxs-lookup"><span data-stu-id="58adf-162">Relationships</span></span>
| <span data-ttu-id="58adf-163">Relação</span><span class="sxs-lookup"><span data-stu-id="58adf-163">Relationship</span></span> | <span data-ttu-id="58adf-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="58adf-164">Type</span></span>   |<span data-ttu-id="58adf-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="58adf-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58adf-166">impactedUser</span><span class="sxs-lookup"><span data-stu-id="58adf-166">impactedUser</span></span>|[<span data-ttu-id="58adf-167">user</span><span class="sxs-lookup"><span data-stu-id="58adf-167">user</span></span>](user.md)| <span data-ttu-id="58adf-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="58adf-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="58adf-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="58adf-170">JSON representation</span></span>

<span data-ttu-id="58adf-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="58adf-171">Here is a JSON representation of the resource.</span></span>

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