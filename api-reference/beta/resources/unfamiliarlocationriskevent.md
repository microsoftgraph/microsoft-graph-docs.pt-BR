---
title: tipo de recurso de unfamiliarLocationRiskEvent
description: Um evento de risco detectado pelo Windows Azure Active Directory identidade proteção onde uma conta entrar é tentada de um novo local para esse usuário. Informações completas sobre eventos de risco podem ser encontradas na documentação de proteção de identidade do Windows Azure AD.
localization_priority: Normal
ms.openlocfilehash: 130d68bfb23bdb23b6a9de81fa988d38db1d8c10
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868737"
---
# <a name="unfamiliarlocationriskevent-resource-type"></a><span data-ttu-id="5ae19-104">tipo de recurso de unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="5ae19-104">unfamiliarLocationRiskEvent resource type</span></span>

> <span data-ttu-id="5ae19-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5ae19-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5ae19-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5ae19-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5ae19-107">Um evento de risco detectado pelo [Proteção de identidade do Windows Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) onde uma conta entrar é tentada de um novo local para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="5ae19-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from a new location for that user.</span></span> <span data-ttu-id="5ae19-108">Informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Windows Azure AD](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="5ae19-108">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="5ae19-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="5ae19-109">Methods</span></span>

| <span data-ttu-id="5ae19-110">Método</span><span class="sxs-lookup"><span data-stu-id="5ae19-110">Method</span></span>           | <span data-ttu-id="5ae19-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5ae19-111">Return Type</span></span>    |<span data-ttu-id="5ae19-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ae19-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5ae19-113">Obter unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="5ae19-113">Get unfamiliarLocationRiskEvent</span></span>](../api/unfamiliarlocationriskevent-get.md) | [<span data-ttu-id="5ae19-114">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="5ae19-114">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) |<span data-ttu-id="5ae19-115">Leia as propriedades e os relacionamentos do objeto unfamiliarLocationRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="5ae19-115">Read properties and relationships of unfamiliarLocationRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5ae19-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5ae19-116">Properties</span></span>
| <span data-ttu-id="5ae19-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ae19-117">Property</span></span>     | <span data-ttu-id="5ae19-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ae19-118">Type</span></span>   |<span data-ttu-id="5ae19-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ae19-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ae19-120">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ae19-120">closedDateTime</span></span>|<span data-ttu-id="5ae19-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ae19-121">dateTimeOffset</span></span>| <span data-ttu-id="5ae19-122">A data e hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="5ae19-122">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="5ae19-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ae19-123">createdDateTime</span></span>|<span data-ttu-id="5ae19-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ae19-124">dateTimeOffset</span></span>| <span data-ttu-id="5ae19-125">A data e hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="5ae19-125">The date and time that the risk event was created.</span></span> <span data-ttu-id="5ae19-126">Sempre é maior ou igual ao datetime do evento risco em si.</span><span class="sxs-lookup"><span data-stu-id="5ae19-126">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="5ae19-127">Esta é a propriedade correta a ser usado como um filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="5ae19-127">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="5ae19-128">id</span><span class="sxs-lookup"><span data-stu-id="5ae19-128">id</span></span>|<span data-ttu-id="5ae19-129">string</span><span class="sxs-lookup"><span data-stu-id="5ae19-129">string</span></span>| <span data-ttu-id="5ae19-130">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="5ae19-130">Read-only</span></span>|
|<span data-ttu-id="5ae19-131">ipAddress</span><span class="sxs-lookup"><span data-stu-id="5ae19-131">ipAddress</span></span>|<span data-ttu-id="5ae19-132">string</span><span class="sxs-lookup"><span data-stu-id="5ae19-132">string</span></span>| <span data-ttu-id="5ae19-133">O endereço IP do sign-in</span><span class="sxs-lookup"><span data-stu-id="5ae19-133">The IP address of the sign-in</span></span>|
|<span data-ttu-id="5ae19-134">location</span><span class="sxs-lookup"><span data-stu-id="5ae19-134">location</span></span>|<span data-ttu-id="5ae19-135">string</span><span class="sxs-lookup"><span data-stu-id="5ae19-135">string</span></span>| <span data-ttu-id="5ae19-136">O local anexado ao endereço IP do sign-in</span><span class="sxs-lookup"><span data-stu-id="5ae19-136">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="5ae19-137">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="5ae19-137">riskEventDateTime</span></span>|<span data-ttu-id="5ae19-138">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ae19-138">dateTimeOffset</span></span>| <span data-ttu-id="5ae19-139">A data e hora quando o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="5ae19-139">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="5ae19-140">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="5ae19-140">riskEventStatus</span></span>|<span data-ttu-id="5ae19-141">string</span><span class="sxs-lookup"><span data-stu-id="5ae19-141">string</span></span>| <span data-ttu-id="5ae19-142">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="5ae19-142">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="5ae19-143">riskLevel</span><span class="sxs-lookup"><span data-stu-id="5ae19-143">riskLevel</span></span>|<span data-ttu-id="5ae19-144">string</span><span class="sxs-lookup"><span data-stu-id="5ae19-144">string</span></span>| <span data-ttu-id="5ae19-145">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="5ae19-145">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="5ae19-146">riskEventType</span><span class="sxs-lookup"><span data-stu-id="5ae19-146">riskEventType</span></span>|<span data-ttu-id="5ae19-147">string</span><span class="sxs-lookup"><span data-stu-id="5ae19-147">string</span></span>| <span data-ttu-id="5ae19-148">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="5ae19-148">The type of risk</span></span>|
|<span data-ttu-id="5ae19-149">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="5ae19-149">userDisplayName</span></span>|<span data-ttu-id="5ae19-150">string</span><span class="sxs-lookup"><span data-stu-id="5ae19-150">string</span></span>| <span data-ttu-id="5ae19-151">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="5ae19-151">The name of the user at risk</span></span>|
|<span data-ttu-id="5ae19-152">userId</span><span class="sxs-lookup"><span data-stu-id="5ae19-152">userId</span></span>|<span data-ttu-id="5ae19-153">string</span><span class="sxs-lookup"><span data-stu-id="5ae19-153">string</span></span>| <span data-ttu-id="5ae19-154">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="5ae19-154">The id of the user at risk</span></span>|
|<span data-ttu-id="5ae19-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5ae19-155">userPrincipalName</span></span>|<span data-ttu-id="5ae19-156">string</span><span class="sxs-lookup"><span data-stu-id="5ae19-156">string</span></span>| <span data-ttu-id="5ae19-157">O nome de usuário principal do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="5ae19-157">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ae19-158">Relações</span><span class="sxs-lookup"><span data-stu-id="5ae19-158">Relationships</span></span>
| <span data-ttu-id="5ae19-159">Relação</span><span class="sxs-lookup"><span data-stu-id="5ae19-159">Relationship</span></span> | <span data-ttu-id="5ae19-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ae19-160">Type</span></span>   |<span data-ttu-id="5ae19-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ae19-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ae19-162">impactedUser</span><span class="sxs-lookup"><span data-stu-id="5ae19-162">impactedUser</span></span>|[<span data-ttu-id="5ae19-163">user</span><span class="sxs-lookup"><span data-stu-id="5ae19-163">user</span></span>](user.md)| <span data-ttu-id="5ae19-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="5ae19-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5ae19-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5ae19-166">JSON representation</span></span>

<span data-ttu-id="5ae19-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5ae19-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unfamiliarLocationRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
