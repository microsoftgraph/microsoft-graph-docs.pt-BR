---
title: tipo de recurso leakedCredentialsRiskEvent
description: Um evento de risco detectado pela proteção de identidade do Azure Active Directory onde as credenciais de uma conta foram detectadas. As informações completas sobre eventos de risco podem ser encontradas na documentação de proteção de identidade do Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: c9c1efda0cb4c11899d5884da05a91f07e5a000d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029222"
---
# <a name="leakedcredentialsriskevent-resource-type-deprecated"></a><span data-ttu-id="abd16-104">tipo de recurso leakedCredentialsRiskEvent (preterido)</span><span class="sxs-lookup"><span data-stu-id="abd16-104">leakedCredentialsRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="abd16-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abd16-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="abd16-106">A API **identityRiskEvents** foi preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="abd16-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="abd16-107">Para obter detalhes, consulte [Preterition of the IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="abd16-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="abd16-108">Um evento de risco detectado pela [proteção de identidade do Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) onde as credenciais de uma conta foram detectadas.</span><span class="sxs-lookup"><span data-stu-id="abd16-108">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="abd16-109">As informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Azure ad](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="abd16-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="abd16-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="abd16-110">Methods</span></span>

| <span data-ttu-id="abd16-111">Método</span><span class="sxs-lookup"><span data-stu-id="abd16-111">Method</span></span>           | <span data-ttu-id="abd16-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="abd16-112">Return Type</span></span>    |<span data-ttu-id="abd16-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="abd16-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="abd16-114">Obter leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="abd16-114">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="abd16-115">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="abd16-115">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="abd16-116">Leia as propriedades e os relacionamentos do objeto leakedCredentialsRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="abd16-116">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="abd16-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="abd16-117">Properties</span></span>
| <span data-ttu-id="abd16-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="abd16-118">Property</span></span>     | <span data-ttu-id="abd16-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="abd16-119">Type</span></span>   |<span data-ttu-id="abd16-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="abd16-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="abd16-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="abd16-121">closedDateTime</span></span>|<span data-ttu-id="abd16-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abd16-122">dateTimeOffset</span></span>| <span data-ttu-id="abd16-123">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="abd16-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="abd16-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="abd16-124">createdDateTime</span></span>|<span data-ttu-id="abd16-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abd16-125">dateTimeOffset</span></span>| <span data-ttu-id="abd16-126">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="abd16-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="abd16-127">Isso é sempre maior que ou igual ao DateTime do evento de risco propriamente dito.</span><span class="sxs-lookup"><span data-stu-id="abd16-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="abd16-128">Esta é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="abd16-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="abd16-129">id</span><span class="sxs-lookup"><span data-stu-id="abd16-129">id</span></span>|<span data-ttu-id="abd16-130">string</span><span class="sxs-lookup"><span data-stu-id="abd16-130">string</span></span>| <span data-ttu-id="abd16-131">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="abd16-131">Read-only</span></span>|
|<span data-ttu-id="abd16-132">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="abd16-132">riskEventDateTime</span></span>|<span data-ttu-id="abd16-133">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abd16-133">dateTimeOffset</span></span>| <span data-ttu-id="abd16-134">A data e a hora em que o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="abd16-134">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="abd16-135">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="abd16-135">riskEventStatus</span></span>|<span data-ttu-id="abd16-136">string</span><span class="sxs-lookup"><span data-stu-id="abd16-136">string</span></span>| <span data-ttu-id="abd16-137">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="abd16-137">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="abd16-138">riskLevel</span><span class="sxs-lookup"><span data-stu-id="abd16-138">riskLevel</span></span>|<span data-ttu-id="abd16-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abd16-139">string</span></span>| <span data-ttu-id="abd16-140">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="abd16-140">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="abd16-141">riskEventType</span><span class="sxs-lookup"><span data-stu-id="abd16-141">riskEventType</span></span>|<span data-ttu-id="abd16-142">string</span><span class="sxs-lookup"><span data-stu-id="abd16-142">string</span></span>| <span data-ttu-id="abd16-143">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="abd16-143">The type of risk</span></span>|
|<span data-ttu-id="abd16-144">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="abd16-144">userDisplayName</span></span>|<span data-ttu-id="abd16-145">string</span><span class="sxs-lookup"><span data-stu-id="abd16-145">string</span></span>| <span data-ttu-id="abd16-146">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="abd16-146">The name of the user at risk</span></span>|
|<span data-ttu-id="abd16-147">userId</span><span class="sxs-lookup"><span data-stu-id="abd16-147">userId</span></span>|<span data-ttu-id="abd16-148">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abd16-148">string</span></span>| <span data-ttu-id="abd16-149">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="abd16-149">The id of the user at risk</span></span>|
|<span data-ttu-id="abd16-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="abd16-150">userPrincipalName</span></span>|<span data-ttu-id="abd16-151">string</span><span class="sxs-lookup"><span data-stu-id="abd16-151">string</span></span>| <span data-ttu-id="abd16-152">O nome principal de usuário do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="abd16-152">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="abd16-153">Relações</span><span class="sxs-lookup"><span data-stu-id="abd16-153">Relationships</span></span>
| <span data-ttu-id="abd16-154">Relação</span><span class="sxs-lookup"><span data-stu-id="abd16-154">Relationship</span></span> | <span data-ttu-id="abd16-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="abd16-155">Type</span></span>   |<span data-ttu-id="abd16-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="abd16-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="abd16-157">impactedUser</span><span class="sxs-lookup"><span data-stu-id="abd16-157">impactedUser</span></span>|[<span data-ttu-id="abd16-158">Usuário</span><span class="sxs-lookup"><span data-stu-id="abd16-158">user</span></span>](user.md)| <span data-ttu-id="abd16-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="abd16-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="abd16-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="abd16-161">JSON representation</span></span>

<span data-ttu-id="abd16-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="abd16-162">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent"
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
  "userPrincipalName": "string",
  "riskEventType": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "leakedCredentialsRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


