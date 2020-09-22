---
title: tipo de recurso unfamiliarLocationRiskEvent
description: Um evento de risco detectado pela proteção de identidade do Azure Active Directory na qual é feita uma tentativa de entrada de uma conta a partir de um novo local para esse usuário. As informações completas sobre eventos de risco podem ser encontradas na documentação de proteção de identidade do Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: ec1b9a0921326f9ebd8ff6f72b9ec584b1080462
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075391"
---
# <a name="unfamiliarlocationriskevent-resource-type-deprecated"></a><span data-ttu-id="8ee6b-104">tipo de recurso unfamiliarLocationRiskEvent (preterido)</span><span class="sxs-lookup"><span data-stu-id="8ee6b-104">unfamiliarLocationRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="8ee6b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ee6b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="8ee6b-106">A API **identityRiskEvents** foi preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="8ee6b-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="8ee6b-107">Para obter detalhes, consulte [Preterition of the IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="8ee6b-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="8ee6b-108">Um evento de risco detectado pela [proteção de identidade do Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) na qual é feita uma tentativa de entrada de uma conta a partir de um novo local para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="8ee6b-108">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from a new location for that user.</span></span> <span data-ttu-id="8ee6b-109">As informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Azure ad](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="8ee6b-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="8ee6b-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="8ee6b-110">Methods</span></span>

| <span data-ttu-id="8ee6b-111">Método</span><span class="sxs-lookup"><span data-stu-id="8ee6b-111">Method</span></span>           | <span data-ttu-id="8ee6b-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8ee6b-112">Return Type</span></span>    |<span data-ttu-id="8ee6b-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ee6b-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8ee6b-114">Obter unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="8ee6b-114">Get unfamiliarLocationRiskEvent</span></span>](../api/unfamiliarlocationriskevent-get.md) | [<span data-ttu-id="8ee6b-115">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="8ee6b-115">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) |<span data-ttu-id="8ee6b-116">Leia as propriedades e os relacionamentos do objeto unfamiliarLocationRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="8ee6b-116">Read properties and relationships of unfamiliarLocationRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8ee6b-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ee6b-117">Properties</span></span>
| <span data-ttu-id="8ee6b-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ee6b-118">Property</span></span>     | <span data-ttu-id="8ee6b-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ee6b-119">Type</span></span>   |<span data-ttu-id="8ee6b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ee6b-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ee6b-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ee6b-121">closedDateTime</span></span>|<span data-ttu-id="8ee6b-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ee6b-122">dateTimeOffset</span></span>| <span data-ttu-id="8ee6b-123">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="8ee6b-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="8ee6b-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ee6b-124">createdDateTime</span></span>|<span data-ttu-id="8ee6b-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ee6b-125">dateTimeOffset</span></span>| <span data-ttu-id="8ee6b-126">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="8ee6b-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="8ee6b-127">Isso é sempre maior que ou igual ao DateTime do evento de risco propriamente dito.</span><span class="sxs-lookup"><span data-stu-id="8ee6b-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="8ee6b-128">Esta é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="8ee6b-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="8ee6b-129">id</span><span class="sxs-lookup"><span data-stu-id="8ee6b-129">id</span></span>|<span data-ttu-id="8ee6b-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ee6b-130">string</span></span>| <span data-ttu-id="8ee6b-131">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="8ee6b-131">Read-only</span></span>|
|<span data-ttu-id="8ee6b-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="8ee6b-132">ipAddress</span></span>|<span data-ttu-id="8ee6b-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ee6b-133">string</span></span>| <span data-ttu-id="8ee6b-134">O endereço IP do logon</span><span class="sxs-lookup"><span data-stu-id="8ee6b-134">The IP address of the sign-in</span></span>|
|<span data-ttu-id="8ee6b-135">location</span><span class="sxs-lookup"><span data-stu-id="8ee6b-135">location</span></span>|<span data-ttu-id="8ee6b-136">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ee6b-136">string</span></span>| <span data-ttu-id="8ee6b-137">O local anexado ao endereço IP do logon</span><span class="sxs-lookup"><span data-stu-id="8ee6b-137">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="8ee6b-138">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="8ee6b-138">riskEventDateTime</span></span>|<span data-ttu-id="8ee6b-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ee6b-139">dateTimeOffset</span></span>| <span data-ttu-id="8ee6b-140">A data e a hora em que o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="8ee6b-140">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="8ee6b-141">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="8ee6b-141">riskEventStatus</span></span>|<span data-ttu-id="8ee6b-142">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ee6b-142">string</span></span>| <span data-ttu-id="8ee6b-143">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="8ee6b-143">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="8ee6b-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="8ee6b-144">riskLevel</span></span>|<span data-ttu-id="8ee6b-145">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ee6b-145">string</span></span>| <span data-ttu-id="8ee6b-146">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="8ee6b-146">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="8ee6b-147">riskEventType</span><span class="sxs-lookup"><span data-stu-id="8ee6b-147">riskEventType</span></span>|<span data-ttu-id="8ee6b-148">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ee6b-148">string</span></span>| <span data-ttu-id="8ee6b-149">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="8ee6b-149">The type of risk</span></span>|
|<span data-ttu-id="8ee6b-150">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="8ee6b-150">userDisplayName</span></span>|<span data-ttu-id="8ee6b-151">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ee6b-151">string</span></span>| <span data-ttu-id="8ee6b-152">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="8ee6b-152">The name of the user at risk</span></span>|
|<span data-ttu-id="8ee6b-153">userId</span><span class="sxs-lookup"><span data-stu-id="8ee6b-153">userId</span></span>|<span data-ttu-id="8ee6b-154">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ee6b-154">string</span></span>| <span data-ttu-id="8ee6b-155">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="8ee6b-155">The id of the user at risk</span></span>|
|<span data-ttu-id="8ee6b-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8ee6b-156">userPrincipalName</span></span>|<span data-ttu-id="8ee6b-157">string</span><span class="sxs-lookup"><span data-stu-id="8ee6b-157">string</span></span>| <span data-ttu-id="8ee6b-158">O nome principal de usuário do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="8ee6b-158">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ee6b-159">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="8ee6b-159">Relationships</span></span>
| <span data-ttu-id="8ee6b-160">Relação</span><span class="sxs-lookup"><span data-stu-id="8ee6b-160">Relationship</span></span> | <span data-ttu-id="8ee6b-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ee6b-161">Type</span></span>   |<span data-ttu-id="8ee6b-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ee6b-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ee6b-163">impactedUser</span><span class="sxs-lookup"><span data-stu-id="8ee6b-163">impactedUser</span></span>|[<span data-ttu-id="8ee6b-164">usuário</span><span class="sxs-lookup"><span data-stu-id="8ee6b-164">user</span></span>](user.md)| <span data-ttu-id="8ee6b-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="8ee6b-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ee6b-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ee6b-167">JSON representation</span></span>

<span data-ttu-id="8ee6b-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ee6b-168">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.locatedRiskEvent",
  "@odata.type": "microsoft.graph.unfamiliarLocationRiskEvent"
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
  "description": "unfamiliarLocationRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


