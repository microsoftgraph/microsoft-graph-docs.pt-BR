---
title: tipo de recurso leakedCredentialsRiskEvent
description: Um evento de risco detectado pela proteção de identidade do Azure Active Directory onde as credenciais de uma conta foram detectadas. As informações completas sobre eventos de risco podem ser encontradas na documentação de proteção de identidade do Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: 90b062fa0e7f6d577accabf6d8b458174d2f696c
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810556"
---
# <a name="leakedcredentialsriskevent-resource-type"></a><span data-ttu-id="ed513-104">tipo de recurso leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="ed513-104">leakedCredentialsRiskEvent resource type</span></span>

<span data-ttu-id="ed513-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed513-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="ed513-106">A API **identityRiskEvents** foi preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="ed513-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="ed513-107">Para obter detalhes, consulte [Preterition of the IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="ed513-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="ed513-108">Um evento de risco detectado pela [proteção de identidade do Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) onde as credenciais de uma conta foram detectadas.</span><span class="sxs-lookup"><span data-stu-id="ed513-108">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="ed513-109">As informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Azure ad](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="ed513-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="ed513-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="ed513-110">Methods</span></span>

| <span data-ttu-id="ed513-111">Método</span><span class="sxs-lookup"><span data-stu-id="ed513-111">Method</span></span>           | <span data-ttu-id="ed513-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ed513-112">Return Type</span></span>    |<span data-ttu-id="ed513-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed513-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ed513-114">Obter leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="ed513-114">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="ed513-115">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="ed513-115">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="ed513-116">Leia as propriedades e os relacionamentos do objeto leakedCredentialsRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="ed513-116">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ed513-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed513-117">Properties</span></span>
| <span data-ttu-id="ed513-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed513-118">Property</span></span>     | <span data-ttu-id="ed513-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed513-119">Type</span></span>   |<span data-ttu-id="ed513-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed513-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed513-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed513-121">closedDateTime</span></span>|<span data-ttu-id="ed513-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed513-122">dateTimeOffset</span></span>| <span data-ttu-id="ed513-123">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="ed513-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="ed513-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ed513-124">createdDateTime</span></span>|<span data-ttu-id="ed513-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed513-125">dateTimeOffset</span></span>| <span data-ttu-id="ed513-126">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="ed513-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="ed513-127">Isso é sempre maior que ou igual ao DateTime do evento de risco propriamente dito.</span><span class="sxs-lookup"><span data-stu-id="ed513-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="ed513-128">Esta é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="ed513-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="ed513-129">id</span><span class="sxs-lookup"><span data-stu-id="ed513-129">id</span></span>|<span data-ttu-id="ed513-130">string</span><span class="sxs-lookup"><span data-stu-id="ed513-130">string</span></span>| <span data-ttu-id="ed513-131">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="ed513-131">Read-only</span></span>|
|<span data-ttu-id="ed513-132">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="ed513-132">riskEventDateTime</span></span>|<span data-ttu-id="ed513-133">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed513-133">dateTimeOffset</span></span>| <span data-ttu-id="ed513-134">A data e a hora em que o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="ed513-134">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="ed513-135">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="ed513-135">riskEventStatus</span></span>|<span data-ttu-id="ed513-136">string</span><span class="sxs-lookup"><span data-stu-id="ed513-136">string</span></span>| <span data-ttu-id="ed513-137">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="ed513-137">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="ed513-138">riskLevel</span><span class="sxs-lookup"><span data-stu-id="ed513-138">riskLevel</span></span>|<span data-ttu-id="ed513-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed513-139">string</span></span>| <span data-ttu-id="ed513-140">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="ed513-140">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="ed513-141">riskEventType</span><span class="sxs-lookup"><span data-stu-id="ed513-141">riskEventType</span></span>|<span data-ttu-id="ed513-142">string</span><span class="sxs-lookup"><span data-stu-id="ed513-142">string</span></span>| <span data-ttu-id="ed513-143">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="ed513-143">The type of risk</span></span>|
|<span data-ttu-id="ed513-144">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ed513-144">userDisplayName</span></span>|<span data-ttu-id="ed513-145">string</span><span class="sxs-lookup"><span data-stu-id="ed513-145">string</span></span>| <span data-ttu-id="ed513-146">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="ed513-146">The name of the user at risk</span></span>|
|<span data-ttu-id="ed513-147">userId</span><span class="sxs-lookup"><span data-stu-id="ed513-147">userId</span></span>|<span data-ttu-id="ed513-148">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed513-148">string</span></span>| <span data-ttu-id="ed513-149">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="ed513-149">The id of the user at risk</span></span>|
|<span data-ttu-id="ed513-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ed513-150">userPrincipalName</span></span>|<span data-ttu-id="ed513-151">string</span><span class="sxs-lookup"><span data-stu-id="ed513-151">string</span></span>| <span data-ttu-id="ed513-152">O nome principal de usuário do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="ed513-152">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed513-153">Relações</span><span class="sxs-lookup"><span data-stu-id="ed513-153">Relationships</span></span>
| <span data-ttu-id="ed513-154">Relação</span><span class="sxs-lookup"><span data-stu-id="ed513-154">Relationship</span></span> | <span data-ttu-id="ed513-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed513-155">Type</span></span>   |<span data-ttu-id="ed513-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed513-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed513-157">impactedUser</span><span class="sxs-lookup"><span data-stu-id="ed513-157">impactedUser</span></span>|[<span data-ttu-id="ed513-158">user</span><span class="sxs-lookup"><span data-stu-id="ed513-158">user</span></span>](user.md)| <span data-ttu-id="ed513-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="ed513-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ed513-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed513-161">JSON representation</span></span>

<span data-ttu-id="ed513-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed513-162">Here is a JSON representation of the resource.</span></span>

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
