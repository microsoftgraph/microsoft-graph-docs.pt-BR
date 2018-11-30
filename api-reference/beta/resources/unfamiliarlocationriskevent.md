---
title: tipo de recurso de unfamiliarLocationRiskEvent
description: Um evento de risco detectado pelo Windows Azure Active Directory identidade proteção onde uma conta entrar é tentada de um novo local para esse usuário. Informações completas sobre eventos de risco podem ser encontradas na documentação de proteção de identidade do Windows Azure AD.
ms.openlocfilehash: 7fa75c28fcc6432a5f8e32bff695e32d76c5acdc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034390"
---
# <a name="unfamiliarlocationriskevent-resource-type"></a><span data-ttu-id="d249a-104">tipo de recurso de unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="d249a-104">unfamiliarLocationRiskEvent resource type</span></span>

> <span data-ttu-id="d249a-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d249a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d249a-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d249a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d249a-107">Um evento de risco detectado pelo [Proteção de identidade do Windows Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) onde uma conta entrar é tentada de um novo local para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="d249a-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from a new location for that user.</span></span> <span data-ttu-id="d249a-108">Informações completas sobre eventos de risco podem ser encontradas na [documentação de proteção de identidade do Windows Azure AD](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="d249a-108">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="d249a-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="d249a-109">Methods</span></span>

| <span data-ttu-id="d249a-110">Método</span><span class="sxs-lookup"><span data-stu-id="d249a-110">Method</span></span>           | <span data-ttu-id="d249a-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d249a-111">Return Type</span></span>    |<span data-ttu-id="d249a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d249a-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d249a-113">Obter unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="d249a-113">Get unfamiliarLocationRiskEvent</span></span>](../api/unfamiliarlocationriskevent-get.md) | [<span data-ttu-id="d249a-114">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="d249a-114">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) |<span data-ttu-id="d249a-115">Leia as propriedades e os relacionamentos do objeto unfamiliarLocationRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="d249a-115">Read properties and relationships of unfamiliarLocationRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d249a-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d249a-116">Properties</span></span>
| <span data-ttu-id="d249a-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d249a-117">Property</span></span>     | <span data-ttu-id="d249a-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="d249a-118">Type</span></span>   |<span data-ttu-id="d249a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d249a-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d249a-120">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="d249a-120">closedDateTime</span></span>|<span data-ttu-id="d249a-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d249a-121">dateTimeOffset</span></span>| <span data-ttu-id="d249a-122">A data e hora em que o evento de risco foi fechado</span><span class="sxs-lookup"><span data-stu-id="d249a-122">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="d249a-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d249a-123">createdDateTime</span></span>|<span data-ttu-id="d249a-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d249a-124">dateTimeOffset</span></span>| <span data-ttu-id="d249a-125">A data e hora em que o evento de risco foi criado.</span><span class="sxs-lookup"><span data-stu-id="d249a-125">The date and time that the risk event was created.</span></span> <span data-ttu-id="d249a-126">Sempre é maior ou igual ao datetime do evento risco em si.</span><span class="sxs-lookup"><span data-stu-id="d249a-126">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="d249a-127">Esta é a propriedade correta a ser usado como um filtro ao consultar eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="d249a-127">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="d249a-128">id</span><span class="sxs-lookup"><span data-stu-id="d249a-128">id</span></span>|<span data-ttu-id="d249a-129">string</span><span class="sxs-lookup"><span data-stu-id="d249a-129">string</span></span>| <span data-ttu-id="d249a-130">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="d249a-130">Read-only</span></span>|
|<span data-ttu-id="d249a-131">ipAddress</span><span class="sxs-lookup"><span data-stu-id="d249a-131">ipAddress</span></span>|<span data-ttu-id="d249a-132">string</span><span class="sxs-lookup"><span data-stu-id="d249a-132">string</span></span>| <span data-ttu-id="d249a-133">O endereço IP do sign-in</span><span class="sxs-lookup"><span data-stu-id="d249a-133">The IP address of the sign-in</span></span>|
|<span data-ttu-id="d249a-134">location</span><span class="sxs-lookup"><span data-stu-id="d249a-134">location</span></span>|<span data-ttu-id="d249a-135">string</span><span class="sxs-lookup"><span data-stu-id="d249a-135">string</span></span>| <span data-ttu-id="d249a-136">O local anexado ao endereço IP do sign-in</span><span class="sxs-lookup"><span data-stu-id="d249a-136">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="d249a-137">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="d249a-137">riskEventDateTime</span></span>|<span data-ttu-id="d249a-138">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d249a-138">dateTimeOffset</span></span>| <span data-ttu-id="d249a-139">A data e hora quando o evento de risco ocorreu</span><span class="sxs-lookup"><span data-stu-id="d249a-139">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="d249a-140">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="d249a-140">riskEventStatus</span></span>|<span data-ttu-id="d249a-141">string</span><span class="sxs-lookup"><span data-stu-id="d249a-141">string</span></span>| <span data-ttu-id="d249a-142">Os valores possíveis são: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="d249a-142">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="d249a-143">riskLevel</span><span class="sxs-lookup"><span data-stu-id="d249a-143">riskLevel</span></span>|<span data-ttu-id="d249a-144">string</span><span class="sxs-lookup"><span data-stu-id="d249a-144">string</span></span>| <span data-ttu-id="d249a-145">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="d249a-145">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="d249a-146">riskEventType</span><span class="sxs-lookup"><span data-stu-id="d249a-146">riskEventType</span></span>|<span data-ttu-id="d249a-147">string</span><span class="sxs-lookup"><span data-stu-id="d249a-147">string</span></span>| <span data-ttu-id="d249a-148">O tipo de risco</span><span class="sxs-lookup"><span data-stu-id="d249a-148">The type of risk</span></span>|
|<span data-ttu-id="d249a-149">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d249a-149">userDisplayName</span></span>|<span data-ttu-id="d249a-150">string</span><span class="sxs-lookup"><span data-stu-id="d249a-150">string</span></span>| <span data-ttu-id="d249a-151">O nome do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="d249a-151">The name of the user at risk</span></span>|
|<span data-ttu-id="d249a-152">userId</span><span class="sxs-lookup"><span data-stu-id="d249a-152">userId</span></span>|<span data-ttu-id="d249a-153">string</span><span class="sxs-lookup"><span data-stu-id="d249a-153">string</span></span>| <span data-ttu-id="d249a-154">A identificação do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="d249a-154">The id of the user at risk</span></span>|
|<span data-ttu-id="d249a-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d249a-155">userPrincipalName</span></span>|<span data-ttu-id="d249a-156">string</span><span class="sxs-lookup"><span data-stu-id="d249a-156">string</span></span>| <span data-ttu-id="d249a-157">O nome de usuário principal do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="d249a-157">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="d249a-158">Relações</span><span class="sxs-lookup"><span data-stu-id="d249a-158">Relationships</span></span>
| <span data-ttu-id="d249a-159">Relação</span><span class="sxs-lookup"><span data-stu-id="d249a-159">Relationship</span></span> | <span data-ttu-id="d249a-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="d249a-160">Type</span></span>   |<span data-ttu-id="d249a-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="d249a-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d249a-162">impactedUser</span><span class="sxs-lookup"><span data-stu-id="d249a-162">impactedUser</span></span>|[<span data-ttu-id="d249a-163">user</span><span class="sxs-lookup"><span data-stu-id="d249a-163">user</span></span>](user.md)| <span data-ttu-id="d249a-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="d249a-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d249a-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d249a-166">JSON representation</span></span>

<span data-ttu-id="d249a-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d249a-167">Here is a JSON representation of the resource.</span></span>

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