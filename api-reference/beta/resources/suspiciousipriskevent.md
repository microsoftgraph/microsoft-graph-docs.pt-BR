---
title: tipo de recurso de suspiciousIpRiskEvent
description: Um evento de risco detectado pelo Windows Azure Active Directory identidade proteção onde uma conta entrar é tentada de um endereço IP suspeito. Informações completas sobre eventos de risco podem ser encontradas na documentação de proteção de identidade do Windows Azure AD.
localization_priority: Normal
ms.openlocfilehash: e144e1f631941076b5cee7cee20d90062564012a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515808"
---
# <a name="suspiciousipriskevent-resource-type"></a><span data-ttu-id="d7e30-104">tipo de recurso de suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="d7e30-104">suspiciousIpRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7e30-105">Um evento de risco detectado pelo [Proteção de identidade do Windows Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) onde uma conta entrar é tentada de um endereço IP suspeito.</span><span class="sxs-lookup"><span data-stu-id="d7e30-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from a suspicious IP address.</span></span> <span data-ttu-id="d7e30-106">Informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Windows Azure AD](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="d7e30-106">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="d7e30-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d7e30-107">Methods</span></span>

| <span data-ttu-id="d7e30-108">Método</span><span class="sxs-lookup"><span data-stu-id="d7e30-108">Method</span></span>           | <span data-ttu-id="d7e30-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d7e30-109">Return Type</span></span>    |<span data-ttu-id="d7e30-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7e30-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d7e30-111">Obter suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="d7e30-111">Get suspiciousIpRiskEvent</span></span>](../api/suspiciousipriskevent-get.md) | [<span data-ttu-id="d7e30-112">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="d7e30-112">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) |<span data-ttu-id="d7e30-113">Leia as propriedades e os relacionamentos do objeto suspiciousIpRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="d7e30-113">Read properties and relationships of suspiciousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d7e30-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d7e30-114">Properties</span></span>
| <span data-ttu-id="d7e30-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7e30-115">Property</span></span>     | <span data-ttu-id="d7e30-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7e30-116">Type</span></span>   |<span data-ttu-id="d7e30-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7e30-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7e30-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7e30-118">closedDateTime</span></span>|<span data-ttu-id="d7e30-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7e30-119">dateTimeOffset</span></span>| <span data-ttu-id="d7e30-120">A data e hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="d7e30-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="d7e30-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d7e30-121">createdDateTime</span></span>|<span data-ttu-id="d7e30-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7e30-122">dateTimeOffset</span></span>| <span data-ttu-id="d7e30-123">A data e hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="d7e30-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="d7e30-124">Sempre é maior ou igual ao datetime do evento risco em si.</span><span class="sxs-lookup"><span data-stu-id="d7e30-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="d7e30-125">Esta é a propriedade correta a ser usado como um filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="d7e30-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="d7e30-126">id</span><span class="sxs-lookup"><span data-stu-id="d7e30-126">id</span></span>|<span data-ttu-id="d7e30-127">string</span><span class="sxs-lookup"><span data-stu-id="d7e30-127">string</span></span>| <span data-ttu-id="d7e30-128">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="d7e30-128">Read-only</span></span>|
|<span data-ttu-id="d7e30-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="d7e30-129">ipAddress</span></span>|<span data-ttu-id="d7e30-130">string</span><span class="sxs-lookup"><span data-stu-id="d7e30-130">string</span></span>| <span data-ttu-id="d7e30-131">O endereço IP do sign-in</span><span class="sxs-lookup"><span data-stu-id="d7e30-131">The IP address of the sign-in</span></span>|
|<span data-ttu-id="d7e30-132">location</span><span class="sxs-lookup"><span data-stu-id="d7e30-132">location</span></span>|<span data-ttu-id="d7e30-133">string</span><span class="sxs-lookup"><span data-stu-id="d7e30-133">string</span></span>| <span data-ttu-id="d7e30-134">O local anexado ao endereço IP do sign-in</span><span class="sxs-lookup"><span data-stu-id="d7e30-134">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="d7e30-135">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="d7e30-135">riskEventDateTime</span></span>|<span data-ttu-id="d7e30-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7e30-136">dateTimeOffset</span></span>| <span data-ttu-id="d7e30-137">A data e hora quando o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="d7e30-137">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="d7e30-138">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="d7e30-138">riskEventStatus</span></span>|<span data-ttu-id="d7e30-139">string</span><span class="sxs-lookup"><span data-stu-id="d7e30-139">string</span></span>| <span data-ttu-id="d7e30-140">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="d7e30-140">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="d7e30-141">riskLevel</span><span class="sxs-lookup"><span data-stu-id="d7e30-141">riskLevel</span></span>|<span data-ttu-id="d7e30-142">string</span><span class="sxs-lookup"><span data-stu-id="d7e30-142">string</span></span>| <span data-ttu-id="d7e30-143">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="d7e30-143">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="d7e30-144">riskEventType</span><span class="sxs-lookup"><span data-stu-id="d7e30-144">riskEventType</span></span>|<span data-ttu-id="d7e30-145">string</span><span class="sxs-lookup"><span data-stu-id="d7e30-145">string</span></span>| <span data-ttu-id="d7e30-146">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="d7e30-146">The type of risk</span></span>|
|<span data-ttu-id="d7e30-147">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d7e30-147">userDisplayName</span></span>|<span data-ttu-id="d7e30-148">string</span><span class="sxs-lookup"><span data-stu-id="d7e30-148">string</span></span>| <span data-ttu-id="d7e30-149">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="d7e30-149">The name of the user at risk</span></span>|
|<span data-ttu-id="d7e30-150">userId</span><span class="sxs-lookup"><span data-stu-id="d7e30-150">userId</span></span>|<span data-ttu-id="d7e30-151">string</span><span class="sxs-lookup"><span data-stu-id="d7e30-151">string</span></span>| <span data-ttu-id="d7e30-152">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="d7e30-152">The id of the user at risk</span></span>|
|<span data-ttu-id="d7e30-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d7e30-153">userPrincipalName</span></span>|<span data-ttu-id="d7e30-154">string</span><span class="sxs-lookup"><span data-stu-id="d7e30-154">string</span></span>| <span data-ttu-id="d7e30-155">O nome de usuário principal do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="d7e30-155">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7e30-156">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="d7e30-156">Relationships</span></span>
| <span data-ttu-id="d7e30-157">Relação</span><span class="sxs-lookup"><span data-stu-id="d7e30-157">Relationship</span></span> | <span data-ttu-id="d7e30-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7e30-158">Type</span></span>   |<span data-ttu-id="d7e30-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7e30-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7e30-160">impactedUser</span><span class="sxs-lookup"><span data-stu-id="d7e30-160">impactedUser</span></span>|[<span data-ttu-id="d7e30-161">user</span><span class="sxs-lookup"><span data-stu-id="d7e30-161">user</span></span>](user.md)| <span data-ttu-id="d7e30-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="d7e30-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d7e30-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d7e30-164">JSON representation</span></span>

<span data-ttu-id="d7e30-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d7e30-165">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "suspiciousIpRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/suspiciousipriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
