---
title: tipo de recurso leakedCredentialsRiskEvent
description: Um evento de risco detectado pela proteção de identidade do Azure Active Directory onde as credenciais de uma conta foram detectadas. As informações completas sobre eventos de risco podem ser encontradas na documentação de proteção de identidade do Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4f12131d1dafcd8bc33d026ef4c56d220eae2799
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870212"
---
# <a name="leakedcredentialsriskevent-resource-type"></a><span data-ttu-id="1505e-104">tipo de recurso leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="1505e-104">leakedCredentialsRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="1505e-105">A API **identityRiskEvents** foi preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="1505e-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="1505e-106">Para obter detalhes, consulte [Preterition of the IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="1505e-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="1505e-107">Um evento de risco detectado pela [proteção de identidade do Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) onde as credenciais de uma conta foram detectadas.</span><span class="sxs-lookup"><span data-stu-id="1505e-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="1505e-108">As informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Azure ad](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="1505e-108">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="1505e-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="1505e-109">Methods</span></span>

| <span data-ttu-id="1505e-110">Método</span><span class="sxs-lookup"><span data-stu-id="1505e-110">Method</span></span>           | <span data-ttu-id="1505e-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1505e-111">Return Type</span></span>    |<span data-ttu-id="1505e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1505e-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1505e-113">Obter leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="1505e-113">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="1505e-114">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="1505e-114">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="1505e-115">Leia as propriedades e os relacionamentos do objeto leakedCredentialsRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="1505e-115">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1505e-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1505e-116">Properties</span></span>
| <span data-ttu-id="1505e-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1505e-117">Property</span></span>     | <span data-ttu-id="1505e-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="1505e-118">Type</span></span>   |<span data-ttu-id="1505e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="1505e-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1505e-120">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="1505e-120">closedDateTime</span></span>|<span data-ttu-id="1505e-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1505e-121">dateTimeOffset</span></span>| <span data-ttu-id="1505e-122">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="1505e-122">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="1505e-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1505e-123">createdDateTime</span></span>|<span data-ttu-id="1505e-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1505e-124">dateTimeOffset</span></span>| <span data-ttu-id="1505e-125">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="1505e-125">The date and time that the risk event was created.</span></span> <span data-ttu-id="1505e-126">Isso é sempre maior que ou igual ao DateTime do evento de risco propriamente dito.</span><span class="sxs-lookup"><span data-stu-id="1505e-126">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="1505e-127">Esta é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="1505e-127">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="1505e-128">id</span><span class="sxs-lookup"><span data-stu-id="1505e-128">id</span></span>|<span data-ttu-id="1505e-129">string</span><span class="sxs-lookup"><span data-stu-id="1505e-129">string</span></span>| <span data-ttu-id="1505e-130">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="1505e-130">Read-only</span></span>|
|<span data-ttu-id="1505e-131">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="1505e-131">riskEventDateTime</span></span>|<span data-ttu-id="1505e-132">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1505e-132">dateTimeOffset</span></span>| <span data-ttu-id="1505e-133">A data e a hora em que o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="1505e-133">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="1505e-134">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="1505e-134">riskEventStatus</span></span>|<span data-ttu-id="1505e-135">string</span><span class="sxs-lookup"><span data-stu-id="1505e-135">string</span></span>| <span data-ttu-id="1505e-136">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="1505e-136">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="1505e-137">riskLevel</span><span class="sxs-lookup"><span data-stu-id="1505e-137">riskLevel</span></span>|<span data-ttu-id="1505e-138">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1505e-138">string</span></span>| <span data-ttu-id="1505e-139">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="1505e-139">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="1505e-140">riskEventType</span><span class="sxs-lookup"><span data-stu-id="1505e-140">riskEventType</span></span>|<span data-ttu-id="1505e-141">string</span><span class="sxs-lookup"><span data-stu-id="1505e-141">string</span></span>| <span data-ttu-id="1505e-142">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="1505e-142">The type of risk</span></span>|
|<span data-ttu-id="1505e-143">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="1505e-143">userDisplayName</span></span>|<span data-ttu-id="1505e-144">string</span><span class="sxs-lookup"><span data-stu-id="1505e-144">string</span></span>| <span data-ttu-id="1505e-145">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="1505e-145">The name of the user at risk</span></span>|
|<span data-ttu-id="1505e-146">userId</span><span class="sxs-lookup"><span data-stu-id="1505e-146">userId</span></span>|<span data-ttu-id="1505e-147">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1505e-147">string</span></span>| <span data-ttu-id="1505e-148">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="1505e-148">The id of the user at risk</span></span>|
|<span data-ttu-id="1505e-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1505e-149">userPrincipalName</span></span>|<span data-ttu-id="1505e-150">string</span><span class="sxs-lookup"><span data-stu-id="1505e-150">string</span></span>| <span data-ttu-id="1505e-151">O nome principal de usuário do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="1505e-151">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="1505e-152">Relações</span><span class="sxs-lookup"><span data-stu-id="1505e-152">Relationships</span></span>
| <span data-ttu-id="1505e-153">Relação</span><span class="sxs-lookup"><span data-stu-id="1505e-153">Relationship</span></span> | <span data-ttu-id="1505e-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="1505e-154">Type</span></span>   |<span data-ttu-id="1505e-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="1505e-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1505e-156">impactedUser</span><span class="sxs-lookup"><span data-stu-id="1505e-156">impactedUser</span></span>|[<span data-ttu-id="1505e-157">Usuário</span><span class="sxs-lookup"><span data-stu-id="1505e-157">user</span></span>](user.md)| <span data-ttu-id="1505e-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="1505e-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1505e-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1505e-160">JSON representation</span></span>

<span data-ttu-id="1505e-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1505e-161">Here is a JSON representation of the resource.</span></span>

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
