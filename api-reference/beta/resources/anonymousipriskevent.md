---
title: tipo de recurso anonymousIpRiskEvent
description: Um evento de risco detectado pela proteção de identidade do Azure Active Directory em que uma entrada de conta é tentada a partir de um endereço IP que parece ser anônimo. As informações completas sobre eventos de risco podem ser encontradas na documentação de proteção de identidade do Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 205659f4ebc301824798cd39506cd73853c167ca
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870395"
---
# <a name="anonymousipriskevent-resource-type"></a><span data-ttu-id="9a50b-104">tipo de recurso anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="9a50b-104">anonymousIpRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="9a50b-105">A API **identityRiskEvents** foi preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="9a50b-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="9a50b-106">Para obter detalhes, consulte [Preterition of the IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="9a50b-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="9a50b-107">Um evento de risco detectado pela [proteção de identidade do Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) em que uma entrada de conta é tentada a partir de um endereço IP que parece ser anônimo.</span><span class="sxs-lookup"><span data-stu-id="9a50b-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from an IP address that appears to be anonymous.</span></span> <span data-ttu-id="9a50b-108">As informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Azure ad](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="9a50b-108">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="9a50b-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="9a50b-109">Methods</span></span>

| <span data-ttu-id="9a50b-110">Método</span><span class="sxs-lookup"><span data-stu-id="9a50b-110">Method</span></span>           | <span data-ttu-id="9a50b-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9a50b-111">Return Type</span></span>    |<span data-ttu-id="9a50b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a50b-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9a50b-113">Obter anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="9a50b-113">Get anonymousIpRiskEvent</span></span>](../api/anonymousipriskevent-get.md) | [<span data-ttu-id="9a50b-114">anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="9a50b-114">anonymousIpRiskEvent</span></span>](anonymousipriskevent.md) |<span data-ttu-id="9a50b-115">Leia as propriedades e os relacionamentos do objeto anonymousIpRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="9a50b-115">Read properties and relationships of anonymousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9a50b-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9a50b-116">Properties</span></span>
| <span data-ttu-id="9a50b-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a50b-117">Property</span></span>     | <span data-ttu-id="9a50b-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a50b-118">Type</span></span>   |<span data-ttu-id="9a50b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a50b-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a50b-120">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a50b-120">closedDateTime</span></span>|<span data-ttu-id="9a50b-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a50b-121">dateTimeOffset</span></span>| <span data-ttu-id="9a50b-122">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="9a50b-122">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="9a50b-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a50b-123">createdDateTime</span></span>|<span data-ttu-id="9a50b-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a50b-124">dateTimeOffset</span></span>| <span data-ttu-id="9a50b-125">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="9a50b-125">The date and time that the risk event was created.</span></span> <span data-ttu-id="9a50b-126">Isso é sempre maior que ou igual ao DateTime do evento de risco propriamente dito.</span><span class="sxs-lookup"><span data-stu-id="9a50b-126">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="9a50b-127">Esta é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="9a50b-127">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="9a50b-128">id</span><span class="sxs-lookup"><span data-stu-id="9a50b-128">id</span></span>|<span data-ttu-id="9a50b-129">string</span><span class="sxs-lookup"><span data-stu-id="9a50b-129">string</span></span>| <span data-ttu-id="9a50b-130">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="9a50b-130">Read-only</span></span>|
|<span data-ttu-id="9a50b-131">ipAddress</span><span class="sxs-lookup"><span data-stu-id="9a50b-131">ipAddress</span></span>|<span data-ttu-id="9a50b-132">string</span><span class="sxs-lookup"><span data-stu-id="9a50b-132">string</span></span>| <span data-ttu-id="9a50b-133">O endereço IP do logon</span><span class="sxs-lookup"><span data-stu-id="9a50b-133">The IP address of the sign-in</span></span>|
|<span data-ttu-id="9a50b-134">location</span><span class="sxs-lookup"><span data-stu-id="9a50b-134">location</span></span>|<span data-ttu-id="9a50b-135">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a50b-135">string</span></span>| <span data-ttu-id="9a50b-136">O local anexado ao endereço IP do logon</span><span class="sxs-lookup"><span data-stu-id="9a50b-136">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="9a50b-137">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="9a50b-137">riskEventDateTime</span></span>|<span data-ttu-id="9a50b-138">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a50b-138">dateTimeOffset</span></span>| <span data-ttu-id="9a50b-139">A data e a hora em que o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="9a50b-139">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="9a50b-140">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="9a50b-140">riskEventStatus</span></span>|<span data-ttu-id="9a50b-141">string</span><span class="sxs-lookup"><span data-stu-id="9a50b-141">string</span></span>| <span data-ttu-id="9a50b-142">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="9a50b-142">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="9a50b-143">riskLevel</span><span class="sxs-lookup"><span data-stu-id="9a50b-143">riskLevel</span></span>|<span data-ttu-id="9a50b-144">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a50b-144">string</span></span>| <span data-ttu-id="9a50b-145">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="9a50b-145">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="9a50b-146">riskEventType</span><span class="sxs-lookup"><span data-stu-id="9a50b-146">riskEventType</span></span>|<span data-ttu-id="9a50b-147">string</span><span class="sxs-lookup"><span data-stu-id="9a50b-147">string</span></span>| <span data-ttu-id="9a50b-148">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="9a50b-148">The type of risk</span></span>|
|<span data-ttu-id="9a50b-149">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="9a50b-149">userDisplayName</span></span>|<span data-ttu-id="9a50b-150">string</span><span class="sxs-lookup"><span data-stu-id="9a50b-150">string</span></span>| <span data-ttu-id="9a50b-151">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="9a50b-151">The name of the user at risk</span></span>|
|<span data-ttu-id="9a50b-152">userId</span><span class="sxs-lookup"><span data-stu-id="9a50b-152">userId</span></span>|<span data-ttu-id="9a50b-153">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a50b-153">string</span></span>| <span data-ttu-id="9a50b-154">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="9a50b-154">The id of the user at risk</span></span>|
|<span data-ttu-id="9a50b-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9a50b-155">userPrincipalName</span></span>|<span data-ttu-id="9a50b-156">string</span><span class="sxs-lookup"><span data-stu-id="9a50b-156">string</span></span>| <span data-ttu-id="9a50b-157">O nome principal de usuário do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="9a50b-157">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a50b-158">Relações</span><span class="sxs-lookup"><span data-stu-id="9a50b-158">Relationships</span></span>
| <span data-ttu-id="9a50b-159">Relação</span><span class="sxs-lookup"><span data-stu-id="9a50b-159">Relationship</span></span> | <span data-ttu-id="9a50b-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a50b-160">Type</span></span>   |<span data-ttu-id="9a50b-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a50b-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a50b-162">impactedUser</span><span class="sxs-lookup"><span data-stu-id="9a50b-162">impactedUser</span></span>|[<span data-ttu-id="9a50b-163">Usuário</span><span class="sxs-lookup"><span data-stu-id="9a50b-163">user</span></span>](user.md)| <span data-ttu-id="9a50b-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="9a50b-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9a50b-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9a50b-166">JSON representation</span></span>

<span data-ttu-id="9a50b-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9a50b-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
   "baseType":"microsoft.graph.locatedRiskEvent",
  "@odata.type": "microsoft.graph.anonymousIpRiskEvent"
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
  "description": "anonymousIpRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
