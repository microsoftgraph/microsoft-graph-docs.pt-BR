---
title: tipo de recurso de impossibleTravelRiskEvent
description: Um evento de risco detectado pelo Windows Azure Active Directory identidade proteção onde duas entradas do conta ocorrem de locais atípicos para o usuário e seria impossível viajam entre os locais em que a duração entre as informações completas de sign-ins. sobre eventos de risco podem ser encontrados na documentação de proteção de identidade do Windows Azure AD.
ms.openlocfilehash: 38e61927121f520e79fd1fec8b8e6443fa8b76e7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033449"
---
# <a name="impossibletravelriskevent-resource-type"></a><span data-ttu-id="9f09b-103">tipo de recurso de impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="9f09b-103">impossibleTravelRiskEvent resource type</span></span>

> <span data-ttu-id="9f09b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9f09b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f09b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9f09b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f09b-106">Um evento de risco detectado pelo [Proteção de identidade do Windows Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) na qual duas entradas do conta ocorrem de locais atípicos para o usuário e seria impossível viajam entre os locais na duração entre concluir sign-ins. informações sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Windows Azure AD](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="9f09b-106">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="9f09b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="9f09b-107">Methods</span></span>

| <span data-ttu-id="9f09b-108">Método</span><span class="sxs-lookup"><span data-stu-id="9f09b-108">Method</span></span>           | <span data-ttu-id="9f09b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9f09b-109">Return Type</span></span>    |<span data-ttu-id="9f09b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f09b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9f09b-111">Obter impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="9f09b-111">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="9f09b-112">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="9f09b-112">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="9f09b-113">Leia as propriedades e os relacionamentos do objeto impossibleTravelRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="9f09b-113">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9f09b-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9f09b-114">Properties</span></span>
| <span data-ttu-id="9f09b-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f09b-115">Property</span></span>     | <span data-ttu-id="9f09b-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f09b-116">Type</span></span>   |<span data-ttu-id="9f09b-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f09b-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f09b-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f09b-118">closedDateTime</span></span>|<span data-ttu-id="9f09b-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f09b-119">dateTimeOffset</span></span>| <span data-ttu-id="9f09b-120">A data e hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="9f09b-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="9f09b-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f09b-121">createdDateTime</span></span>|<span data-ttu-id="9f09b-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f09b-122">dateTimeOffset</span></span>| <span data-ttu-id="9f09b-123">A data e hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="9f09b-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="9f09b-124">Sempre é maior ou igual ao datetime do evento risco em si.</span><span class="sxs-lookup"><span data-stu-id="9f09b-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="9f09b-125">Esta é a propriedade correta a ser usado como um filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="9f09b-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="9f09b-126">deviceInformation</span><span class="sxs-lookup"><span data-stu-id="9f09b-126">deviceInformation</span></span>|<span data-ttu-id="9f09b-127">string</span><span class="sxs-lookup"><span data-stu-id="9f09b-127">string</span></span>| <span data-ttu-id="9f09b-128">Informações sobre o dispositivo</span><span class="sxs-lookup"><span data-stu-id="9f09b-128">Information about the device</span></span>|
|<span data-ttu-id="9f09b-129">id</span><span class="sxs-lookup"><span data-stu-id="9f09b-129">id</span></span>|<span data-ttu-id="9f09b-130">string</span><span class="sxs-lookup"><span data-stu-id="9f09b-130">string</span></span>| <span data-ttu-id="9f09b-131">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="9f09b-131">Read-only</span></span>|
|<span data-ttu-id="9f09b-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="9f09b-132">ipAddress</span></span>|<span data-ttu-id="9f09b-133">string</span><span class="sxs-lookup"><span data-stu-id="9f09b-133">string</span></span>| <span data-ttu-id="9f09b-134">O endereço IP do segundo sign-in</span><span class="sxs-lookup"><span data-stu-id="9f09b-134">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="9f09b-135">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="9f09b-135">isAtypicalLocation</span></span>|<span data-ttu-id="9f09b-136">booliano</span><span class="sxs-lookup"><span data-stu-id="9f09b-136">boolean</span></span>| <span data-ttu-id="9f09b-137">Se um dos locais for atípico para o usuário</span><span class="sxs-lookup"><span data-stu-id="9f09b-137">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="9f09b-138">location</span><span class="sxs-lookup"><span data-stu-id="9f09b-138">location</span></span>|<span data-ttu-id="9f09b-139">string</span><span class="sxs-lookup"><span data-stu-id="9f09b-139">string</span></span>| <span data-ttu-id="9f09b-140">O local anexado ao endereço IP do segundo sign-in</span><span class="sxs-lookup"><span data-stu-id="9f09b-140">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="9f09b-141">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="9f09b-141">previousIPAddress</span></span>|<span data-ttu-id="9f09b-142">string</span><span class="sxs-lookup"><span data-stu-id="9f09b-142">string</span></span>| <span data-ttu-id="9f09b-143">O endereço IP do primeiro sign-in</span><span class="sxs-lookup"><span data-stu-id="9f09b-143">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="9f09b-144">previousLocation</span><span class="sxs-lookup"><span data-stu-id="9f09b-144">previousLocation</span></span>|<span data-ttu-id="9f09b-145">string</span><span class="sxs-lookup"><span data-stu-id="9f09b-145">string</span></span>| <span data-ttu-id="9f09b-146">O local anexado ao endereço IP do primeiro sign-in</span><span class="sxs-lookup"><span data-stu-id="9f09b-146">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="9f09b-147">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="9f09b-147">previousSigninDateTime</span></span>|<span data-ttu-id="9f09b-148">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f09b-148">dateTimeOffset</span></span>| <span data-ttu-id="9f09b-149">A data e hora do primeiro sign-in</span><span class="sxs-lookup"><span data-stu-id="9f09b-149">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="9f09b-150">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="9f09b-150">riskEventDateTime</span></span>|<span data-ttu-id="9f09b-151">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f09b-151">dateTimeOffset</span></span>| <span data-ttu-id="9f09b-152">A data e hora do segundo sign-in</span><span class="sxs-lookup"><span data-stu-id="9f09b-152">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="9f09b-153">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="9f09b-153">riskEventStatus</span></span>|<span data-ttu-id="9f09b-154">string</span><span class="sxs-lookup"><span data-stu-id="9f09b-154">string</span></span>| <span data-ttu-id="9f09b-155">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="9f09b-155">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="9f09b-156">riskLevel</span><span class="sxs-lookup"><span data-stu-id="9f09b-156">riskLevel</span></span>|<span data-ttu-id="9f09b-157">string</span><span class="sxs-lookup"><span data-stu-id="9f09b-157">string</span></span>| <span data-ttu-id="9f09b-158">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="9f09b-158">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="9f09b-159">riskEventType</span><span class="sxs-lookup"><span data-stu-id="9f09b-159">riskEventType</span></span>|<span data-ttu-id="9f09b-160">string</span><span class="sxs-lookup"><span data-stu-id="9f09b-160">string</span></span>| <span data-ttu-id="9f09b-161">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="9f09b-161">The type of risk</span></span>|
|<span data-ttu-id="9f09b-162">userAgent</span><span class="sxs-lookup"><span data-stu-id="9f09b-162">userAgent</span></span>|<span data-ttu-id="9f09b-163">string</span><span class="sxs-lookup"><span data-stu-id="9f09b-163">string</span></span>| <span data-ttu-id="9f09b-164">Cadeia de caracteres de agente de usuário do navegador</span><span class="sxs-lookup"><span data-stu-id="9f09b-164">The browser's user agent string</span></span>|
|<span data-ttu-id="9f09b-165">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="9f09b-165">userDisplayName</span></span>|<span data-ttu-id="9f09b-166">string</span><span class="sxs-lookup"><span data-stu-id="9f09b-166">string</span></span>| <span data-ttu-id="9f09b-167">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="9f09b-167">The name of the user at risk</span></span>|
|<span data-ttu-id="9f09b-168">userId</span><span class="sxs-lookup"><span data-stu-id="9f09b-168">userId</span></span>|<span data-ttu-id="9f09b-169">string</span><span class="sxs-lookup"><span data-stu-id="9f09b-169">string</span></span>| <span data-ttu-id="9f09b-170">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="9f09b-170">The id of the user at risk</span></span>|
|<span data-ttu-id="9f09b-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9f09b-171">userPrincipalName</span></span>|<span data-ttu-id="9f09b-172">string</span><span class="sxs-lookup"><span data-stu-id="9f09b-172">string</span></span>| <span data-ttu-id="9f09b-173">O nome de usuário principal do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="9f09b-173">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f09b-174">Relações</span><span class="sxs-lookup"><span data-stu-id="9f09b-174">Relationships</span></span>
| <span data-ttu-id="9f09b-175">Relação</span><span class="sxs-lookup"><span data-stu-id="9f09b-175">Relationship</span></span> | <span data-ttu-id="9f09b-176">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f09b-176">Type</span></span>   |<span data-ttu-id="9f09b-177">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f09b-177">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f09b-178">impactedUser</span><span class="sxs-lookup"><span data-stu-id="9f09b-178">impactedUser</span></span>|[<span data-ttu-id="9f09b-179">user</span><span class="sxs-lookup"><span data-stu-id="9f09b-179">user</span></span>](user.md)| <span data-ttu-id="9f09b-p103">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="9f09b-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9f09b-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9f09b-182">JSON representation</span></span>

<span data-ttu-id="9f09b-183">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9f09b-183">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "impossibleTravelRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->