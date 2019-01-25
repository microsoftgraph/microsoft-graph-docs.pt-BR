---
title: tipo de recurso de impossibleTravelRiskEvent
description: Um evento de risco detectado pelo Windows Azure Active Directory identidade proteção onde duas entradas do conta ocorrem de locais atípicos para o usuário e seria impossível viajam entre os locais em que a duração entre as informações completas de sign-ins. sobre eventos de risco podem ser encontrados na documentação de proteção de identidade do Windows Azure AD.
localization_priority: Normal
ms.openlocfilehash: 517a09963570ce2c4a9e58edf7b73babaaff0426
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529380"
---
# <a name="impossibletravelriskevent-resource-type"></a><span data-ttu-id="8cda1-103">tipo de recurso de impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="8cda1-103">impossibleTravelRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cda1-104">Um evento de risco detectado pelo [Proteção de identidade do Windows Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) na qual duas entradas do conta ocorrem de locais atípicos para o usuário e seria impossível viajam entre os locais na duração entre concluir sign-ins. informações sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Windows Azure AD](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="8cda1-104">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="8cda1-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="8cda1-105">Methods</span></span>

| <span data-ttu-id="8cda1-106">Método</span><span class="sxs-lookup"><span data-stu-id="8cda1-106">Method</span></span>           | <span data-ttu-id="8cda1-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8cda1-107">Return Type</span></span>    |<span data-ttu-id="8cda1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cda1-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8cda1-109">Obter impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="8cda1-109">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="8cda1-110">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="8cda1-110">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="8cda1-111">Leia as propriedades e os relacionamentos do objeto impossibleTravelRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="8cda1-111">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8cda1-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8cda1-112">Properties</span></span>
| <span data-ttu-id="8cda1-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8cda1-113">Property</span></span>     | <span data-ttu-id="8cda1-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cda1-114">Type</span></span>   |<span data-ttu-id="8cda1-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cda1-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cda1-116">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="8cda1-116">closedDateTime</span></span>|<span data-ttu-id="8cda1-117">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cda1-117">dateTimeOffset</span></span>| <span data-ttu-id="8cda1-118">A data e hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="8cda1-118">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="8cda1-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8cda1-119">createdDateTime</span></span>|<span data-ttu-id="8cda1-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cda1-120">dateTimeOffset</span></span>| <span data-ttu-id="8cda1-121">A data e hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="8cda1-121">The date and time that the risk event was created.</span></span> <span data-ttu-id="8cda1-122">Sempre é maior ou igual ao datetime do evento risco em si.</span><span class="sxs-lookup"><span data-stu-id="8cda1-122">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="8cda1-123">Esta é a propriedade correta a ser usado como um filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="8cda1-123">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="8cda1-124">deviceInformation</span><span class="sxs-lookup"><span data-stu-id="8cda1-124">deviceInformation</span></span>|<span data-ttu-id="8cda1-125">string</span><span class="sxs-lookup"><span data-stu-id="8cda1-125">string</span></span>| <span data-ttu-id="8cda1-126">Informações sobre o dispositivo</span><span class="sxs-lookup"><span data-stu-id="8cda1-126">Information about the device</span></span>|
|<span data-ttu-id="8cda1-127">id</span><span class="sxs-lookup"><span data-stu-id="8cda1-127">id</span></span>|<span data-ttu-id="8cda1-128">string</span><span class="sxs-lookup"><span data-stu-id="8cda1-128">string</span></span>| <span data-ttu-id="8cda1-129">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="8cda1-129">Read-only</span></span>|
|<span data-ttu-id="8cda1-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="8cda1-130">ipAddress</span></span>|<span data-ttu-id="8cda1-131">string</span><span class="sxs-lookup"><span data-stu-id="8cda1-131">string</span></span>| <span data-ttu-id="8cda1-132">O endereço IP do segundo sign-in</span><span class="sxs-lookup"><span data-stu-id="8cda1-132">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="8cda1-133">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="8cda1-133">isAtypicalLocation</span></span>|<span data-ttu-id="8cda1-134">booliano</span><span class="sxs-lookup"><span data-stu-id="8cda1-134">boolean</span></span>| <span data-ttu-id="8cda1-135">Se um dos locais for atípico para o usuário</span><span class="sxs-lookup"><span data-stu-id="8cda1-135">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="8cda1-136">location</span><span class="sxs-lookup"><span data-stu-id="8cda1-136">location</span></span>|<span data-ttu-id="8cda1-137">string</span><span class="sxs-lookup"><span data-stu-id="8cda1-137">string</span></span>| <span data-ttu-id="8cda1-138">O local anexado ao endereço IP do segundo sign-in</span><span class="sxs-lookup"><span data-stu-id="8cda1-138">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="8cda1-139">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="8cda1-139">previousIPAddress</span></span>|<span data-ttu-id="8cda1-140">string</span><span class="sxs-lookup"><span data-stu-id="8cda1-140">string</span></span>| <span data-ttu-id="8cda1-141">O endereço IP do primeiro sign-in</span><span class="sxs-lookup"><span data-stu-id="8cda1-141">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="8cda1-142">previousLocation</span><span class="sxs-lookup"><span data-stu-id="8cda1-142">previousLocation</span></span>|<span data-ttu-id="8cda1-143">string</span><span class="sxs-lookup"><span data-stu-id="8cda1-143">string</span></span>| <span data-ttu-id="8cda1-144">O local anexado ao endereço IP do primeiro sign-in</span><span class="sxs-lookup"><span data-stu-id="8cda1-144">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="8cda1-145">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="8cda1-145">previousSigninDateTime</span></span>|<span data-ttu-id="8cda1-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cda1-146">dateTimeOffset</span></span>| <span data-ttu-id="8cda1-147">A data e hora do primeiro sign-in</span><span class="sxs-lookup"><span data-stu-id="8cda1-147">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="8cda1-148">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="8cda1-148">riskEventDateTime</span></span>|<span data-ttu-id="8cda1-149">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cda1-149">dateTimeOffset</span></span>| <span data-ttu-id="8cda1-150">A data e hora do segundo sign-in</span><span class="sxs-lookup"><span data-stu-id="8cda1-150">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="8cda1-151">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="8cda1-151">riskEventStatus</span></span>|<span data-ttu-id="8cda1-152">string</span><span class="sxs-lookup"><span data-stu-id="8cda1-152">string</span></span>| <span data-ttu-id="8cda1-153">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="8cda1-153">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="8cda1-154">riskLevel</span><span class="sxs-lookup"><span data-stu-id="8cda1-154">riskLevel</span></span>|<span data-ttu-id="8cda1-155">string</span><span class="sxs-lookup"><span data-stu-id="8cda1-155">string</span></span>| <span data-ttu-id="8cda1-156">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="8cda1-156">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="8cda1-157">riskEventType</span><span class="sxs-lookup"><span data-stu-id="8cda1-157">riskEventType</span></span>|<span data-ttu-id="8cda1-158">string</span><span class="sxs-lookup"><span data-stu-id="8cda1-158">string</span></span>| <span data-ttu-id="8cda1-159">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="8cda1-159">The type of risk</span></span>|
|<span data-ttu-id="8cda1-160">UserAgent</span><span class="sxs-lookup"><span data-stu-id="8cda1-160">userAgent</span></span>|<span data-ttu-id="8cda1-161">string</span><span class="sxs-lookup"><span data-stu-id="8cda1-161">string</span></span>| <span data-ttu-id="8cda1-162">Cadeia de caracteres de agente de usuário do navegador</span><span class="sxs-lookup"><span data-stu-id="8cda1-162">The browser's user agent string</span></span>|
|<span data-ttu-id="8cda1-163">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="8cda1-163">userDisplayName</span></span>|<span data-ttu-id="8cda1-164">string</span><span class="sxs-lookup"><span data-stu-id="8cda1-164">string</span></span>| <span data-ttu-id="8cda1-165">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="8cda1-165">The name of the user at risk</span></span>|
|<span data-ttu-id="8cda1-166">userId</span><span class="sxs-lookup"><span data-stu-id="8cda1-166">userId</span></span>|<span data-ttu-id="8cda1-167">string</span><span class="sxs-lookup"><span data-stu-id="8cda1-167">string</span></span>| <span data-ttu-id="8cda1-168">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="8cda1-168">The id of the user at risk</span></span>|
|<span data-ttu-id="8cda1-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8cda1-169">userPrincipalName</span></span>|<span data-ttu-id="8cda1-170">string</span><span class="sxs-lookup"><span data-stu-id="8cda1-170">string</span></span>| <span data-ttu-id="8cda1-171">O nome de usuário principal do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="8cda1-171">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cda1-172">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="8cda1-172">Relationships</span></span>
| <span data-ttu-id="8cda1-173">Relação</span><span class="sxs-lookup"><span data-stu-id="8cda1-173">Relationship</span></span> | <span data-ttu-id="8cda1-174">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cda1-174">Type</span></span>   |<span data-ttu-id="8cda1-175">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cda1-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cda1-176">impactedUser</span><span class="sxs-lookup"><span data-stu-id="8cda1-176">impactedUser</span></span>|[<span data-ttu-id="8cda1-177">user</span><span class="sxs-lookup"><span data-stu-id="8cda1-177">user</span></span>](user.md)| <span data-ttu-id="8cda1-p102">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="8cda1-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8cda1-180">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8cda1-180">JSON representation</span></span>

<span data-ttu-id="8cda1-181">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8cda1-181">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
  "userPrincipalName": "string"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/impossibletravelriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
