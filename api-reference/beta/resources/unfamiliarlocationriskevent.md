---
title: tipo de recurso unfamiliarLocationRiskEvent
description: Um evento de risco detectado pela proteção de identidade do Azure Active Directory na qual é feita uma tentativa de entrada de uma conta a partir de um novo local para esse usuário. As informações completas sobre eventos de risco podem ser encontradas na documentação de proteção de identidade do Azure AD.
localization_priority: Normal
ms.openlocfilehash: 984f11f7e47a251d49acd315d29504216b7995f6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345469"
---
# <a name="unfamiliarlocationriskevent-resource-type"></a><span data-ttu-id="12705-104">tipo de recurso unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="12705-104">unfamiliarLocationRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12705-105">Um evento de risco detectado pela [proteção de identidade do Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) na qual é feita uma tentativa de entrada de uma conta a partir de um novo local para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="12705-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from a new location for that user.</span></span> <span data-ttu-id="12705-106">As informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Azure ad](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="12705-106">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="12705-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="12705-107">Methods</span></span>

| <span data-ttu-id="12705-108">Método</span><span class="sxs-lookup"><span data-stu-id="12705-108">Method</span></span>           | <span data-ttu-id="12705-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="12705-109">Return Type</span></span>    |<span data-ttu-id="12705-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="12705-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="12705-111">Obter unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="12705-111">Get unfamiliarLocationRiskEvent</span></span>](../api/unfamiliarlocationriskevent-get.md) | [<span data-ttu-id="12705-112">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="12705-112">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) |<span data-ttu-id="12705-113">Leia as propriedades e os relacionamentos do objeto unfamiliarLocationRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="12705-113">Read properties and relationships of unfamiliarLocationRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="12705-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12705-114">Properties</span></span>
| <span data-ttu-id="12705-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12705-115">Property</span></span>     | <span data-ttu-id="12705-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="12705-116">Type</span></span>   |<span data-ttu-id="12705-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="12705-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12705-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="12705-118">closedDateTime</span></span>|<span data-ttu-id="12705-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12705-119">dateTimeOffset</span></span>| <span data-ttu-id="12705-120">A data e a hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="12705-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="12705-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12705-121">createdDateTime</span></span>|<span data-ttu-id="12705-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12705-122">dateTimeOffset</span></span>| <span data-ttu-id="12705-123">A data e a hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="12705-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="12705-124">Isso é sempre maior que ou igual ao DateTime do evento de risco propriamente dito.</span><span class="sxs-lookup"><span data-stu-id="12705-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="12705-125">Esta é a propriedade correta a ser usada como filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="12705-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="12705-126">id</span><span class="sxs-lookup"><span data-stu-id="12705-126">id</span></span>|<span data-ttu-id="12705-127">string</span><span class="sxs-lookup"><span data-stu-id="12705-127">string</span></span>| <span data-ttu-id="12705-128">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="12705-128">Read-only</span></span>|
|<span data-ttu-id="12705-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="12705-129">ipAddress</span></span>|<span data-ttu-id="12705-130">string</span><span class="sxs-lookup"><span data-stu-id="12705-130">string</span></span>| <span data-ttu-id="12705-131">O endereço IP do logon</span><span class="sxs-lookup"><span data-stu-id="12705-131">The IP address of the sign-in</span></span>|
|<span data-ttu-id="12705-132">location</span><span class="sxs-lookup"><span data-stu-id="12705-132">location</span></span>|<span data-ttu-id="12705-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12705-133">string</span></span>| <span data-ttu-id="12705-134">O local anexado ao endereço IP do logon</span><span class="sxs-lookup"><span data-stu-id="12705-134">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="12705-135">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="12705-135">riskEventDateTime</span></span>|<span data-ttu-id="12705-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12705-136">dateTimeOffset</span></span>| <span data-ttu-id="12705-137">A data e a hora em que o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="12705-137">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="12705-138">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="12705-138">riskEventStatus</span></span>|<span data-ttu-id="12705-139">string</span><span class="sxs-lookup"><span data-stu-id="12705-139">string</span></span>| <span data-ttu-id="12705-140">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="12705-140">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="12705-141">riskLevel</span><span class="sxs-lookup"><span data-stu-id="12705-141">riskLevel</span></span>|<span data-ttu-id="12705-142">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12705-142">string</span></span>| <span data-ttu-id="12705-143">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="12705-143">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="12705-144">riskEventType</span><span class="sxs-lookup"><span data-stu-id="12705-144">riskEventType</span></span>|<span data-ttu-id="12705-145">string</span><span class="sxs-lookup"><span data-stu-id="12705-145">string</span></span>| <span data-ttu-id="12705-146">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="12705-146">The type of risk</span></span>|
|<span data-ttu-id="12705-147">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="12705-147">userDisplayName</span></span>|<span data-ttu-id="12705-148">string</span><span class="sxs-lookup"><span data-stu-id="12705-148">string</span></span>| <span data-ttu-id="12705-149">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="12705-149">The name of the user at risk</span></span>|
|<span data-ttu-id="12705-150">userId</span><span class="sxs-lookup"><span data-stu-id="12705-150">userId</span></span>|<span data-ttu-id="12705-151">string</span><span class="sxs-lookup"><span data-stu-id="12705-151">string</span></span>| <span data-ttu-id="12705-152">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="12705-152">The id of the user at risk</span></span>|
|<span data-ttu-id="12705-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="12705-153">userPrincipalName</span></span>|<span data-ttu-id="12705-154">string</span><span class="sxs-lookup"><span data-stu-id="12705-154">string</span></span>| <span data-ttu-id="12705-155">O nome principal de usuário do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="12705-155">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="12705-156">Relações</span><span class="sxs-lookup"><span data-stu-id="12705-156">Relationships</span></span>
| <span data-ttu-id="12705-157">Relação</span><span class="sxs-lookup"><span data-stu-id="12705-157">Relationship</span></span> | <span data-ttu-id="12705-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="12705-158">Type</span></span>   |<span data-ttu-id="12705-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="12705-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12705-160">impactedUser</span><span class="sxs-lookup"><span data-stu-id="12705-160">impactedUser</span></span>|[<span data-ttu-id="12705-161">user</span><span class="sxs-lookup"><span data-stu-id="12705-161">user</span></span>](user.md)| <span data-ttu-id="12705-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="12705-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12705-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12705-164">JSON representation</span></span>

<span data-ttu-id="12705-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="12705-165">Here is a JSON representation of the resource.</span></span>

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
