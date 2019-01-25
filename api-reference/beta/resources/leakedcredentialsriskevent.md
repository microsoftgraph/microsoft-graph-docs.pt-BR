---
title: tipo de recurso de leakedCredentialsRiskEvent
description: Um evento de risco detectado pelo Windows Azure Active Directory identidade proteção onde credenciais da conta foram detectadas à solta. Informações completas sobre eventos de risco podem ser encontradas na documentação de proteção de identidade do Windows Azure AD.
localization_priority: Normal
ms.openlocfilehash: 0884da08195ffa2bee38c943d27b1d25aef02e49
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510985"
---
# <a name="leakedcredentialsriskevent-resource-type"></a><span data-ttu-id="51399-104">tipo de recurso de leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="51399-104">leakedCredentialsRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51399-105">Um evento de risco detectado pelo [Proteção de identidade do Windows Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) onde credenciais da conta foram detectadas à solta.</span><span class="sxs-lookup"><span data-stu-id="51399-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="51399-106">Informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Windows Azure AD](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="51399-106">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="51399-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="51399-107">Methods</span></span>

| <span data-ttu-id="51399-108">Método</span><span class="sxs-lookup"><span data-stu-id="51399-108">Method</span></span>           | <span data-ttu-id="51399-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="51399-109">Return Type</span></span>    |<span data-ttu-id="51399-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="51399-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="51399-111">Obter leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="51399-111">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="51399-112">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="51399-112">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="51399-113">Leia as propriedades e os relacionamentos do objeto leakedCredentialsRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="51399-113">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="51399-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51399-114">Properties</span></span>
| <span data-ttu-id="51399-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51399-115">Property</span></span>     | <span data-ttu-id="51399-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="51399-116">Type</span></span>   |<span data-ttu-id="51399-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="51399-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51399-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="51399-118">closedDateTime</span></span>|<span data-ttu-id="51399-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51399-119">dateTimeOffset</span></span>| <span data-ttu-id="51399-120">A data e hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="51399-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="51399-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51399-121">createdDateTime</span></span>|<span data-ttu-id="51399-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51399-122">dateTimeOffset</span></span>| <span data-ttu-id="51399-123">A data e hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="51399-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="51399-124">Sempre é maior ou igual ao datetime do evento risco em si.</span><span class="sxs-lookup"><span data-stu-id="51399-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="51399-125">Esta é a propriedade correta a ser usado como um filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="51399-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="51399-126">id</span><span class="sxs-lookup"><span data-stu-id="51399-126">id</span></span>|<span data-ttu-id="51399-127">string</span><span class="sxs-lookup"><span data-stu-id="51399-127">string</span></span>| <span data-ttu-id="51399-128">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="51399-128">Read-only</span></span>|
|<span data-ttu-id="51399-129">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="51399-129">riskEventDateTime</span></span>|<span data-ttu-id="51399-130">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51399-130">dateTimeOffset</span></span>| <span data-ttu-id="51399-131">A data e hora quando o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="51399-131">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="51399-132">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="51399-132">riskEventStatus</span></span>|<span data-ttu-id="51399-133">string</span><span class="sxs-lookup"><span data-stu-id="51399-133">string</span></span>| <span data-ttu-id="51399-134">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="51399-134">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="51399-135">riskLevel</span><span class="sxs-lookup"><span data-stu-id="51399-135">riskLevel</span></span>|<span data-ttu-id="51399-136">string</span><span class="sxs-lookup"><span data-stu-id="51399-136">string</span></span>| <span data-ttu-id="51399-137">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="51399-137">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="51399-138">riskEventType</span><span class="sxs-lookup"><span data-stu-id="51399-138">riskEventType</span></span>|<span data-ttu-id="51399-139">string</span><span class="sxs-lookup"><span data-stu-id="51399-139">string</span></span>| <span data-ttu-id="51399-140">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="51399-140">The type of risk</span></span>|
|<span data-ttu-id="51399-141">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="51399-141">userDisplayName</span></span>|<span data-ttu-id="51399-142">string</span><span class="sxs-lookup"><span data-stu-id="51399-142">string</span></span>| <span data-ttu-id="51399-143">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="51399-143">The name of the user at risk</span></span>|
|<span data-ttu-id="51399-144">userId</span><span class="sxs-lookup"><span data-stu-id="51399-144">userId</span></span>|<span data-ttu-id="51399-145">string</span><span class="sxs-lookup"><span data-stu-id="51399-145">string</span></span>| <span data-ttu-id="51399-146">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="51399-146">The id of the user at risk</span></span>|
|<span data-ttu-id="51399-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="51399-147">userPrincipalName</span></span>|<span data-ttu-id="51399-148">string</span><span class="sxs-lookup"><span data-stu-id="51399-148">string</span></span>| <span data-ttu-id="51399-149">O nome de usuário principal do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="51399-149">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="51399-150">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="51399-150">Relationships</span></span>
| <span data-ttu-id="51399-151">Relação</span><span class="sxs-lookup"><span data-stu-id="51399-151">Relationship</span></span> | <span data-ttu-id="51399-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="51399-152">Type</span></span>   |<span data-ttu-id="51399-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="51399-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51399-154">impactedUser</span><span class="sxs-lookup"><span data-stu-id="51399-154">impactedUser</span></span>|[<span data-ttu-id="51399-155">user</span><span class="sxs-lookup"><span data-stu-id="51399-155">user</span></span>](user.md)| <span data-ttu-id="51399-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="51399-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="51399-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51399-158">JSON representation</span></span>

<span data-ttu-id="51399-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="51399-159">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
  "userPrincipalName": "string"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/leakedcredentialsriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
