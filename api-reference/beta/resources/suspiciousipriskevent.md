---
title: tipo de recurso de suspiciousIpRiskEvent
description: Um evento de risco detectado pelo Windows Azure Active Directory identidade proteção onde uma conta entrar é tentada de um endereço IP suspeito. Informações completas sobre eventos de risco podem ser encontradas na documentação de proteção de identidade do Windows Azure AD.
localization_priority: Normal
ms.openlocfilehash: fff23d3034267adc56f3611f22a181ac415499cb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822117"
---
# <a name="suspiciousipriskevent-resource-type"></a><span data-ttu-id="2a851-104">tipo de recurso de suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="2a851-104">suspiciousIpRiskEvent resource type</span></span>

> <span data-ttu-id="2a851-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2a851-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2a851-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2a851-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2a851-107">Um evento de risco detectado pelo [Proteção de identidade do Windows Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) onde uma conta entrar é tentada de um endereço IP suspeito.</span><span class="sxs-lookup"><span data-stu-id="2a851-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from a suspicious IP address.</span></span> <span data-ttu-id="2a851-108">Informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Windows Azure AD](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="2a851-108">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="2a851-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="2a851-109">Methods</span></span>

| <span data-ttu-id="2a851-110">Método</span><span class="sxs-lookup"><span data-stu-id="2a851-110">Method</span></span>           | <span data-ttu-id="2a851-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2a851-111">Return Type</span></span>    |<span data-ttu-id="2a851-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a851-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2a851-113">Obter suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="2a851-113">Get suspiciousIpRiskEvent</span></span>](../api/suspiciousipriskevent-get.md) | [<span data-ttu-id="2a851-114">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="2a851-114">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) |<span data-ttu-id="2a851-115">Leia as propriedades e os relacionamentos do objeto suspiciousIpRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="2a851-115">Read properties and relationships of suspiciousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2a851-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2a851-116">Properties</span></span>
| <span data-ttu-id="2a851-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2a851-117">Property</span></span>     | <span data-ttu-id="2a851-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a851-118">Type</span></span>   |<span data-ttu-id="2a851-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a851-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a851-120">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a851-120">closedDateTime</span></span>|<span data-ttu-id="2a851-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a851-121">dateTimeOffset</span></span>| <span data-ttu-id="2a851-122">A data e hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="2a851-122">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="2a851-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2a851-123">createdDateTime</span></span>|<span data-ttu-id="2a851-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a851-124">dateTimeOffset</span></span>| <span data-ttu-id="2a851-125">A data e hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="2a851-125">The date and time that the risk event was created.</span></span> <span data-ttu-id="2a851-126">Sempre é maior ou igual ao datetime do evento risco em si.</span><span class="sxs-lookup"><span data-stu-id="2a851-126">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="2a851-127">Esta é a propriedade correta a ser usado como um filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="2a851-127">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="2a851-128">id</span><span class="sxs-lookup"><span data-stu-id="2a851-128">id</span></span>|<span data-ttu-id="2a851-129">string</span><span class="sxs-lookup"><span data-stu-id="2a851-129">string</span></span>| <span data-ttu-id="2a851-130">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="2a851-130">Read-only</span></span>|
|<span data-ttu-id="2a851-131">ipAddress</span><span class="sxs-lookup"><span data-stu-id="2a851-131">ipAddress</span></span>|<span data-ttu-id="2a851-132">string</span><span class="sxs-lookup"><span data-stu-id="2a851-132">string</span></span>| <span data-ttu-id="2a851-133">O endereço IP do sign-in</span><span class="sxs-lookup"><span data-stu-id="2a851-133">The IP address of the sign-in</span></span>|
|<span data-ttu-id="2a851-134">location</span><span class="sxs-lookup"><span data-stu-id="2a851-134">location</span></span>|<span data-ttu-id="2a851-135">string</span><span class="sxs-lookup"><span data-stu-id="2a851-135">string</span></span>| <span data-ttu-id="2a851-136">O local anexado ao endereço IP do sign-in</span><span class="sxs-lookup"><span data-stu-id="2a851-136">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="2a851-137">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="2a851-137">riskEventDateTime</span></span>|<span data-ttu-id="2a851-138">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a851-138">dateTimeOffset</span></span>| <span data-ttu-id="2a851-139">A data e hora quando o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="2a851-139">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="2a851-140">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="2a851-140">riskEventStatus</span></span>|<span data-ttu-id="2a851-141">string</span><span class="sxs-lookup"><span data-stu-id="2a851-141">string</span></span>| <span data-ttu-id="2a851-142">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="2a851-142">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="2a851-143">riskLevel</span><span class="sxs-lookup"><span data-stu-id="2a851-143">riskLevel</span></span>|<span data-ttu-id="2a851-144">string</span><span class="sxs-lookup"><span data-stu-id="2a851-144">string</span></span>| <span data-ttu-id="2a851-145">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="2a851-145">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="2a851-146">riskEventType</span><span class="sxs-lookup"><span data-stu-id="2a851-146">riskEventType</span></span>|<span data-ttu-id="2a851-147">string</span><span class="sxs-lookup"><span data-stu-id="2a851-147">string</span></span>| <span data-ttu-id="2a851-148">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="2a851-148">The type of risk</span></span>|
|<span data-ttu-id="2a851-149">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="2a851-149">userDisplayName</span></span>|<span data-ttu-id="2a851-150">string</span><span class="sxs-lookup"><span data-stu-id="2a851-150">string</span></span>| <span data-ttu-id="2a851-151">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="2a851-151">The name of the user at risk</span></span>|
|<span data-ttu-id="2a851-152">userId</span><span class="sxs-lookup"><span data-stu-id="2a851-152">userId</span></span>|<span data-ttu-id="2a851-153">string</span><span class="sxs-lookup"><span data-stu-id="2a851-153">string</span></span>| <span data-ttu-id="2a851-154">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="2a851-154">The id of the user at risk</span></span>|
|<span data-ttu-id="2a851-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2a851-155">userPrincipalName</span></span>|<span data-ttu-id="2a851-156">string</span><span class="sxs-lookup"><span data-stu-id="2a851-156">string</span></span>| <span data-ttu-id="2a851-157">O nome de usuário principal do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="2a851-157">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a851-158">Relações</span><span class="sxs-lookup"><span data-stu-id="2a851-158">Relationships</span></span>
| <span data-ttu-id="2a851-159">Relação</span><span class="sxs-lookup"><span data-stu-id="2a851-159">Relationship</span></span> | <span data-ttu-id="2a851-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a851-160">Type</span></span>   |<span data-ttu-id="2a851-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a851-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a851-162">impactedUser</span><span class="sxs-lookup"><span data-stu-id="2a851-162">impactedUser</span></span>|[<span data-ttu-id="2a851-163">user</span><span class="sxs-lookup"><span data-stu-id="2a851-163">user</span></span>](user.md)| <span data-ttu-id="2a851-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="2a851-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2a851-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2a851-166">JSON representation</span></span>

<span data-ttu-id="2a851-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2a851-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.suspiciousIpRiskEvent"
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
  "description": "suspiciousIpRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
