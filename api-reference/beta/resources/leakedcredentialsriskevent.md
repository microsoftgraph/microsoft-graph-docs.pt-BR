---
title: tipo de recurso de leakedCredentialsRiskEvent
description: Um evento de risco detectado pelo Windows Azure Active Directory identidade proteção onde credenciais da conta foram detectadas à solta. Informações completas sobre eventos de risco podem ser encontradas na documentação de proteção de identidade do Windows Azure AD.
localization_priority: Normal
ms.openlocfilehash: 7a8f2a8cf72b713fab30887fcc4d81b8a88e71ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815978"
---
# <a name="leakedcredentialsriskevent-resource-type"></a><span data-ttu-id="9bf75-104">tipo de recurso de leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="9bf75-104">leakedCredentialsRiskEvent resource type</span></span>

> <span data-ttu-id="9bf75-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9bf75-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9bf75-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9bf75-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9bf75-107">Um evento de risco detectado pelo [Proteção de identidade do Windows Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) onde credenciais da conta foram detectadas à solta.</span><span class="sxs-lookup"><span data-stu-id="9bf75-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="9bf75-108">Informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Windows Azure AD](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="9bf75-108">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="9bf75-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="9bf75-109">Methods</span></span>

| <span data-ttu-id="9bf75-110">Método</span><span class="sxs-lookup"><span data-stu-id="9bf75-110">Method</span></span>           | <span data-ttu-id="9bf75-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9bf75-111">Return Type</span></span>    |<span data-ttu-id="9bf75-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bf75-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9bf75-113">Obter leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="9bf75-113">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="9bf75-114">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="9bf75-114">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="9bf75-115">Leia as propriedades e os relacionamentos do objeto leakedCredentialsRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="9bf75-115">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9bf75-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9bf75-116">Properties</span></span>
| <span data-ttu-id="9bf75-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9bf75-117">Property</span></span>     | <span data-ttu-id="9bf75-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bf75-118">Type</span></span>   |<span data-ttu-id="9bf75-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bf75-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9bf75-120">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="9bf75-120">closedDateTime</span></span>|<span data-ttu-id="9bf75-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bf75-121">dateTimeOffset</span></span>| <span data-ttu-id="9bf75-122">A data e hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="9bf75-122">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="9bf75-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9bf75-123">createdDateTime</span></span>|<span data-ttu-id="9bf75-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bf75-124">dateTimeOffset</span></span>| <span data-ttu-id="9bf75-125">A data e hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="9bf75-125">The date and time that the risk event was created.</span></span> <span data-ttu-id="9bf75-126">Sempre é maior ou igual ao datetime do evento risco em si.</span><span class="sxs-lookup"><span data-stu-id="9bf75-126">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="9bf75-127">Esta é a propriedade correta a ser usado como um filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="9bf75-127">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="9bf75-128">id</span><span class="sxs-lookup"><span data-stu-id="9bf75-128">id</span></span>|<span data-ttu-id="9bf75-129">string</span><span class="sxs-lookup"><span data-stu-id="9bf75-129">string</span></span>| <span data-ttu-id="9bf75-130">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="9bf75-130">Read-only</span></span>|
|<span data-ttu-id="9bf75-131">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="9bf75-131">riskEventDateTime</span></span>|<span data-ttu-id="9bf75-132">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bf75-132">dateTimeOffset</span></span>| <span data-ttu-id="9bf75-133">A data e hora quando o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="9bf75-133">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="9bf75-134">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="9bf75-134">riskEventStatus</span></span>|<span data-ttu-id="9bf75-135">string</span><span class="sxs-lookup"><span data-stu-id="9bf75-135">string</span></span>| <span data-ttu-id="9bf75-136">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="9bf75-136">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="9bf75-137">riskLevel</span><span class="sxs-lookup"><span data-stu-id="9bf75-137">riskLevel</span></span>|<span data-ttu-id="9bf75-138">string</span><span class="sxs-lookup"><span data-stu-id="9bf75-138">string</span></span>| <span data-ttu-id="9bf75-139">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="9bf75-139">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="9bf75-140">riskEventType</span><span class="sxs-lookup"><span data-stu-id="9bf75-140">riskEventType</span></span>|<span data-ttu-id="9bf75-141">string</span><span class="sxs-lookup"><span data-stu-id="9bf75-141">string</span></span>| <span data-ttu-id="9bf75-142">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="9bf75-142">The type of risk</span></span>|
|<span data-ttu-id="9bf75-143">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="9bf75-143">userDisplayName</span></span>|<span data-ttu-id="9bf75-144">string</span><span class="sxs-lookup"><span data-stu-id="9bf75-144">string</span></span>| <span data-ttu-id="9bf75-145">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="9bf75-145">The name of the user at risk</span></span>|
|<span data-ttu-id="9bf75-146">userId</span><span class="sxs-lookup"><span data-stu-id="9bf75-146">userId</span></span>|<span data-ttu-id="9bf75-147">string</span><span class="sxs-lookup"><span data-stu-id="9bf75-147">string</span></span>| <span data-ttu-id="9bf75-148">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="9bf75-148">The id of the user at risk</span></span>|
|<span data-ttu-id="9bf75-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9bf75-149">userPrincipalName</span></span>|<span data-ttu-id="9bf75-150">string</span><span class="sxs-lookup"><span data-stu-id="9bf75-150">string</span></span>| <span data-ttu-id="9bf75-151">O nome de usuário principal do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="9bf75-151">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="9bf75-152">Relações</span><span class="sxs-lookup"><span data-stu-id="9bf75-152">Relationships</span></span>
| <span data-ttu-id="9bf75-153">Relação</span><span class="sxs-lookup"><span data-stu-id="9bf75-153">Relationship</span></span> | <span data-ttu-id="9bf75-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bf75-154">Type</span></span>   |<span data-ttu-id="9bf75-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bf75-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9bf75-156">impactedUser</span><span class="sxs-lookup"><span data-stu-id="9bf75-156">impactedUser</span></span>|[<span data-ttu-id="9bf75-157">user</span><span class="sxs-lookup"><span data-stu-id="9bf75-157">user</span></span>](user.md)| <span data-ttu-id="9bf75-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="9bf75-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9bf75-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9bf75-160">JSON representation</span></span>

<span data-ttu-id="9bf75-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9bf75-161">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "leakedCredentialsRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
