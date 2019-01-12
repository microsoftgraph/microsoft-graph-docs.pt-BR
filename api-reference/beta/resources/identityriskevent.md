---
title: tipo de recurso de identityRiskEvent
description: 'Um evento de risco detectado pelo Windows Azure Active Directory proteção de identidade. É o tipo de base para cada tipo de evento de risco específico:'
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: be5e4afaa5bf85581c904ed94f07433243651ee9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953642"
---
# <a name="identityriskevent-resource-type"></a><span data-ttu-id="c7efb-104">tipo de recurso de identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c7efb-104">identityRiskEvent resource type</span></span>

> <span data-ttu-id="c7efb-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c7efb-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7efb-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c7efb-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c7efb-107">Um evento de risco detectado pelo [Windows Azure Active Directory proteção de identidade](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="c7efb-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span> <span data-ttu-id="c7efb-108">É o tipo de base para cada tipo de evento de risco específico:</span><span class="sxs-lookup"><span data-stu-id="c7efb-108">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="c7efb-109">Tipo de evento</span><span class="sxs-lookup"><span data-stu-id="c7efb-109">Event type</span></span>         | <span data-ttu-id="c7efb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7efb-110">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="c7efb-111">anonymousipRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c7efb-111">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="c7efb-112">Entradas de endereços IP anônimos.</span><span class="sxs-lookup"><span data-stu-id="c7efb-112">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="c7efb-113">malwareRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c7efb-113">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="c7efb-114">Entradas de dispositivos infectados por malware.</span><span class="sxs-lookup"><span data-stu-id="c7efb-114">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="c7efb-115">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c7efb-115">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="c7efb-116">Impossível viagens para atípicos locais.</span><span class="sxs-lookup"><span data-stu-id="c7efb-116">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="c7efb-117">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c7efb-117">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="c7efb-118">Usuários com credenciais perdidas.</span><span class="sxs-lookup"><span data-stu-id="c7efb-118">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="c7efb-119">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c7efb-119">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="c7efb-120">Entradas de endereços IP suspeitos.</span><span class="sxs-lookup"><span data-stu-id="c7efb-120">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="c7efb-121">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c7efb-121">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="c7efb-122">Entradas de familiarizado locais.</span><span class="sxs-lookup"><span data-stu-id="c7efb-122">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="c7efb-123">Informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Windows Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span><span class="sxs-lookup"><span data-stu-id="c7efb-123">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="c7efb-124">Métodos</span><span class="sxs-lookup"><span data-stu-id="c7efb-124">Methods</span></span>

| <span data-ttu-id="c7efb-125">Método</span><span class="sxs-lookup"><span data-stu-id="c7efb-125">Method</span></span>           | <span data-ttu-id="c7efb-126">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c7efb-126">Return Type</span></span>    |<span data-ttu-id="c7efb-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7efb-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c7efb-128">Obter identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c7efb-128">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="c7efb-129">identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c7efb-129">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="c7efb-130">Leia as propriedades e os relacionamentos do objeto identityRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="c7efb-130">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c7efb-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7efb-131">Properties</span></span>
| <span data-ttu-id="c7efb-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7efb-132">Property</span></span>     | <span data-ttu-id="c7efb-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7efb-133">Type</span></span>   |<span data-ttu-id="c7efb-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7efb-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7efb-135">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7efb-135">closedDateTime</span></span>|<span data-ttu-id="c7efb-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7efb-136">dateTimeOffset</span></span>| <span data-ttu-id="c7efb-137">A data e hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="c7efb-137">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="c7efb-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7efb-138">createdDateTime</span></span>|<span data-ttu-id="c7efb-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7efb-139">dateTimeOffset</span></span>| <span data-ttu-id="c7efb-140">A data e hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="c7efb-140">The date and time that the risk event was created.</span></span> <span data-ttu-id="c7efb-141">Sempre é maior ou igual ao datetime do evento risco em si.</span><span class="sxs-lookup"><span data-stu-id="c7efb-141">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="c7efb-142">Esta é a propriedade correta a ser usado como um filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="c7efb-142">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="c7efb-143">id</span><span class="sxs-lookup"><span data-stu-id="c7efb-143">id</span></span>|<span data-ttu-id="c7efb-144">string</span><span class="sxs-lookup"><span data-stu-id="c7efb-144">string</span></span>| <span data-ttu-id="c7efb-145">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="c7efb-145">Read-only</span></span>|
|<span data-ttu-id="c7efb-146">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="c7efb-146">riskEventDateTime</span></span>|<span data-ttu-id="c7efb-147">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7efb-147">dateTimeOffset</span></span>| <span data-ttu-id="c7efb-148">A data e hora quando o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="c7efb-148">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="c7efb-149">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="c7efb-149">riskEventStatus</span></span>|<span data-ttu-id="c7efb-150">string</span><span class="sxs-lookup"><span data-stu-id="c7efb-150">string</span></span>| <span data-ttu-id="c7efb-151">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="c7efb-151">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="c7efb-152">riskLevel</span><span class="sxs-lookup"><span data-stu-id="c7efb-152">riskLevel</span></span>|<span data-ttu-id="c7efb-153">string</span><span class="sxs-lookup"><span data-stu-id="c7efb-153">string</span></span>| <span data-ttu-id="c7efb-154">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="c7efb-154">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="c7efb-155">riskEventType</span><span class="sxs-lookup"><span data-stu-id="c7efb-155">riskEventType</span></span>|<span data-ttu-id="c7efb-156">string</span><span class="sxs-lookup"><span data-stu-id="c7efb-156">string</span></span>| <span data-ttu-id="c7efb-157">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="c7efb-157">The type of risk</span></span>|
|<span data-ttu-id="c7efb-158">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c7efb-158">userDisplayName</span></span>|<span data-ttu-id="c7efb-159">string</span><span class="sxs-lookup"><span data-stu-id="c7efb-159">string</span></span>| <span data-ttu-id="c7efb-160">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="c7efb-160">The name of the user at risk</span></span>|
|<span data-ttu-id="c7efb-161">userId</span><span class="sxs-lookup"><span data-stu-id="c7efb-161">userId</span></span>|<span data-ttu-id="c7efb-162">string</span><span class="sxs-lookup"><span data-stu-id="c7efb-162">string</span></span>| <span data-ttu-id="c7efb-163">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="c7efb-163">The id of the user at risk</span></span>|
|<span data-ttu-id="c7efb-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c7efb-164">userPrincipalName</span></span>|<span data-ttu-id="c7efb-165">string</span><span class="sxs-lookup"><span data-stu-id="c7efb-165">string</span></span>| <span data-ttu-id="c7efb-166">O nome de usuário principal do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="c7efb-166">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7efb-167">Relações</span><span class="sxs-lookup"><span data-stu-id="c7efb-167">Relationships</span></span>
| <span data-ttu-id="c7efb-168">Relação</span><span class="sxs-lookup"><span data-stu-id="c7efb-168">Relationship</span></span> | <span data-ttu-id="c7efb-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7efb-169">Type</span></span>   |<span data-ttu-id="c7efb-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7efb-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7efb-171">impactedUser</span><span class="sxs-lookup"><span data-stu-id="c7efb-171">impactedUser</span></span>|[<span data-ttu-id="c7efb-172">user</span><span class="sxs-lookup"><span data-stu-id="c7efb-172">user</span></span>](user.md)| <span data-ttu-id="c7efb-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="c7efb-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7efb-175">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7efb-175">JSON representation</span></span>

<span data-ttu-id="c7efb-176">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7efb-176">Here is a JSON representation of the resource.</span></span> 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identityRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
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
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
