---
title: tipo de recurso unfamiliarLocationRiskEvent
description: Um evento de risco detectado pela Proteção de Identidade do Azure Active Directory em que uma conta de login é tentada a partir de um novo local para esse usuário. Informações completas sobre eventos de risco podem ser encontradas na documentação da Proteção de Identidade do Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: e2d34106de3e0b72303f103edcc6a798b5790b47
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442723"
---
# <a name="unfamiliarlocationriskevent-resource-type-deprecated"></a><span data-ttu-id="79df7-104">tipo de recurso unfamiliarLocationRiskEvent (preterido)</span><span class="sxs-lookup"><span data-stu-id="79df7-104">unfamiliarLocationRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="79df7-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79df7-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="79df7-106">A **API identityRiskEvents** está preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="79df7-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="79df7-107">Para obter detalhes, [consulte Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="79df7-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="79df7-108">Um evento de risco detectado pela Proteção de Identidade do [Azure Active Directory](/azure/active-directory/identity-protection/overview-identity-protection) em que uma conta de login é tentada a partir de um novo local para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="79df7-108">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) where an account sign-in is attempted from a new location for that user.</span></span> <span data-ttu-id="79df7-109">Informações completas sobre eventos de risco podem ser encontradas na documentação da Proteção de Identidade do [Azure AD.](/azure/active-directory/identity-protection/overview-identity-protection)</span><span class="sxs-lookup"><span data-stu-id="79df7-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="79df7-110">Methods</span><span class="sxs-lookup"><span data-stu-id="79df7-110">Methods</span></span>

| <span data-ttu-id="79df7-111">Método</span><span class="sxs-lookup"><span data-stu-id="79df7-111">Method</span></span>           | <span data-ttu-id="79df7-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="79df7-112">Return Type</span></span>    |<span data-ttu-id="79df7-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="79df7-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="79df7-114">Obter unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="79df7-114">Get unfamiliarLocationRiskEvent</span></span>](../api/unfamiliarlocationriskevent-get.md) | [<span data-ttu-id="79df7-115">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="79df7-115">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) |<span data-ttu-id="79df7-116">Leia propriedades e relações do objeto unfamiliarLocationRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="79df7-116">Read properties and relationships of unfamiliarLocationRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="79df7-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79df7-117">Properties</span></span>
| <span data-ttu-id="79df7-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79df7-118">Property</span></span>     | <span data-ttu-id="79df7-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="79df7-119">Type</span></span>   |<span data-ttu-id="79df7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="79df7-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79df7-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="79df7-121">closedDateTime</span></span>|<span data-ttu-id="79df7-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79df7-122">dateTimeOffset</span></span>| <span data-ttu-id="79df7-123">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="79df7-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="79df7-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79df7-124">createdDateTime</span></span>|<span data-ttu-id="79df7-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79df7-125">dateTimeOffset</span></span>| <span data-ttu-id="79df7-126">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="79df7-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="79df7-127">Isso é sempre maior ou igual ao tempo de data do evento de risco em si.</span><span class="sxs-lookup"><span data-stu-id="79df7-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="79df7-128">Essa é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="79df7-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="79df7-129">id</span><span class="sxs-lookup"><span data-stu-id="79df7-129">id</span></span>|<span data-ttu-id="79df7-130">string</span><span class="sxs-lookup"><span data-stu-id="79df7-130">string</span></span>| <span data-ttu-id="79df7-131">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="79df7-131">Read-only</span></span>|
|<span data-ttu-id="79df7-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="79df7-132">ipAddress</span></span>|<span data-ttu-id="79df7-133">string</span><span class="sxs-lookup"><span data-stu-id="79df7-133">string</span></span>| <span data-ttu-id="79df7-134">O endereço IP da assinatura</span><span class="sxs-lookup"><span data-stu-id="79df7-134">The IP address of the sign-in</span></span>|
|<span data-ttu-id="79df7-135">location</span><span class="sxs-lookup"><span data-stu-id="79df7-135">location</span></span>|<span data-ttu-id="79df7-136">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79df7-136">string</span></span>| <span data-ttu-id="79df7-137">O local anexado ao endereço IP da login</span><span class="sxs-lookup"><span data-stu-id="79df7-137">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="79df7-138">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="79df7-138">riskEventDateTime</span></span>|<span data-ttu-id="79df7-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79df7-139">dateTimeOffset</span></span>| <span data-ttu-id="79df7-140">A data e a hora em que o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="79df7-140">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="79df7-141">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="79df7-141">riskEventStatus</span></span>|<span data-ttu-id="79df7-142">string</span><span class="sxs-lookup"><span data-stu-id="79df7-142">string</span></span>| <span data-ttu-id="79df7-143">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="79df7-143">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="79df7-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="79df7-144">riskLevel</span></span>|<span data-ttu-id="79df7-145">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79df7-145">string</span></span>| <span data-ttu-id="79df7-146">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="79df7-146">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="79df7-147">riskEventType</span><span class="sxs-lookup"><span data-stu-id="79df7-147">riskEventType</span></span>|<span data-ttu-id="79df7-148">string</span><span class="sxs-lookup"><span data-stu-id="79df7-148">string</span></span>| <span data-ttu-id="79df7-149">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="79df7-149">The type of risk</span></span>|
|<span data-ttu-id="79df7-150">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="79df7-150">userDisplayName</span></span>|<span data-ttu-id="79df7-151">string</span><span class="sxs-lookup"><span data-stu-id="79df7-151">string</span></span>| <span data-ttu-id="79df7-152">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="79df7-152">The name of the user at risk</span></span>|
|<span data-ttu-id="79df7-153">userId</span><span class="sxs-lookup"><span data-stu-id="79df7-153">userId</span></span>|<span data-ttu-id="79df7-154">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79df7-154">string</span></span>| <span data-ttu-id="79df7-155">A id do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="79df7-155">The id of the user at risk</span></span>|
|<span data-ttu-id="79df7-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="79df7-156">userPrincipalName</span></span>|<span data-ttu-id="79df7-157">string</span><span class="sxs-lookup"><span data-stu-id="79df7-157">string</span></span>| <span data-ttu-id="79df7-158">O nome principal do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="79df7-158">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="79df7-159">Relações</span><span class="sxs-lookup"><span data-stu-id="79df7-159">Relationships</span></span>
| <span data-ttu-id="79df7-160">Relação</span><span class="sxs-lookup"><span data-stu-id="79df7-160">Relationship</span></span> | <span data-ttu-id="79df7-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="79df7-161">Type</span></span>   |<span data-ttu-id="79df7-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="79df7-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79df7-163">impactedUser</span><span class="sxs-lookup"><span data-stu-id="79df7-163">impactedUser</span></span>|[<span data-ttu-id="79df7-164">user</span><span class="sxs-lookup"><span data-stu-id="79df7-164">user</span></span>](user.md)| <span data-ttu-id="79df7-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="79df7-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="79df7-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79df7-167">JSON representation</span></span>

<span data-ttu-id="79df7-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79df7-168">Here is a JSON representation of the resource.</span></span>

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
