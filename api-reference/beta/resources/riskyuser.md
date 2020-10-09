---
title: tipo de recurso riskyUser
description: Representa usuários do Azure AD que estão em risco. O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários de risco em seu Azure AD.
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 77b3a483c8993b421348bb052c66d66a1558beb0
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48400708"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="4e758-105">tipo de recurso riskyUser</span><span class="sxs-lookup"><span data-stu-id="4e758-105">riskyUser resource type</span></span>

<span data-ttu-id="4e758-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e758-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e758-107">Representa usuários do Azure AD que estão em risco.</span><span class="sxs-lookup"><span data-stu-id="4e758-107">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="4e758-108">O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina.</span><span class="sxs-lookup"><span data-stu-id="4e758-108">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="4e758-109">Essa API fornece acesso programático a todos os usuários de risco em seu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4e758-109">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="4e758-110">Para obter mais informações sobre eventos de risco, consulte [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span><span class="sxs-lookup"><span data-stu-id="4e758-110">For more information about risk events, see [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>

><span data-ttu-id="4e758-111">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="4e758-111">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="4e758-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="4e758-112">Methods</span></span>

| <span data-ttu-id="4e758-113">Método</span><span class="sxs-lookup"><span data-stu-id="4e758-113">Method</span></span>   | <span data-ttu-id="4e758-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4e758-114">Return Type</span></span>|<span data-ttu-id="4e758-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e758-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4e758-116">Listar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="4e758-116">List riskyUsers</span></span>](../api/riskyusers-list.md) | <span data-ttu-id="4e758-117">coleção [riskyUser](riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="4e758-117">[riskyUser](riskyuser.md) collection</span></span>|<span data-ttu-id="4e758-118">Listar usuários arriscados e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="4e758-118">List risky users and their properties.</span></span>|
|[<span data-ttu-id="4e758-119">Obter riskyUser</span><span class="sxs-lookup"><span data-stu-id="4e758-119">Get riskyUser</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="4e758-120">riskyUser</span><span class="sxs-lookup"><span data-stu-id="4e758-120">riskyUser</span></span>](riskyuser.md)|<span data-ttu-id="4e758-121">Obtenha um usuário arriscado específico e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="4e758-121">Get a specific risky user and its properties.</span></span>|
|[<span data-ttu-id="4e758-122">Histórico de lista</span><span class="sxs-lookup"><span data-stu-id="4e758-122">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="4e758-123">coleção [riskyUserHistoryItem](riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="4e758-123">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="4e758-124">Obter o histórico de riscos de um usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4e758-124">Get the risk history of an Azure AD user.</span></span>|
|[<span data-ttu-id="4e758-125">Confirmar riskyUsers comprometido</span><span class="sxs-lookup"><span data-stu-id="4e758-125">Confirm riskyUsers compromised</span></span>](../api/riskyusers-confirmcompromised.md)|<span data-ttu-id="4e758-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4e758-126">None</span></span> |<span data-ttu-id="4e758-127">Confirmar um usuário arriscado como comprometido.</span><span class="sxs-lookup"><span data-stu-id="4e758-127">Confirm a risky user as compromised.</span></span>|
|[<span data-ttu-id="4e758-128">Ignorar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="4e758-128">Dismiss riskyUsers</span></span>](../api/riskyusers-dismiss.md)|<span data-ttu-id="4e758-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4e758-129">None</span></span> | <span data-ttu-id="4e758-130">Descartar o risco de um usuário arriscado.</span><span class="sxs-lookup"><span data-stu-id="4e758-130">Dismiss the risk of a risky user.</span></span>|

## <a name="properties"></a><span data-ttu-id="4e758-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4e758-131">Properties</span></span>

| <span data-ttu-id="4e758-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e758-132">Property</span></span>   | <span data-ttu-id="4e758-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e758-133">Type</span></span>|<span data-ttu-id="4e758-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e758-134">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="4e758-135">ID exclusiva do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="4e758-135">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="4e758-136">Indica se o usuário é excluído.</span><span class="sxs-lookup"><span data-stu-id="4e758-136">Indicates whether the user is deleted.</span></span> <span data-ttu-id="4e758-137">Os valores possíveis são: `true` , `false`</span><span class="sxs-lookup"><span data-stu-id="4e758-137">Possible values are: `true`, `false`</span></span>|
|`isProcessing`|`bool`|<span data-ttu-id="4e758-138">Indica wehther que o estado arriscado de um usuário está sendo processado pelo backend</span><span class="sxs-lookup"><span data-stu-id="4e758-138">Indicates wehther a user's risky state is being processed by the backend</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="4e758-139">A data e a hora em que o usuário arriscado foi atualizado pela última vez</span><span class="sxs-lookup"><span data-stu-id="4e758-139">The date and time that the risky user was last updated</span></span>|
|`riskLevel`|`riskLevel`| <span data-ttu-id="4e758-140">Os valores possíveis são baixo, médio, alto, oculto, nenhum, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="4e758-140">The possible values are low, medium, high, hidden, none, unknownFutureValue.</span></span>  |
|`riskState`|`riskState`| <span data-ttu-id="4e758-141">Os valores possíveis são None, confirmedSafe, remediated, atRisk, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="4e758-141">The possible values are none, confirmedSafe, remediated, atRisk, unknownFutureValue.</span></span>  |
|`riskDetail`|`riskDetail`| <span data-ttu-id="4e758-142">Os valores possíveis são None, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, Hidden, adminConfirmedUserCompromised, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="4e758-142">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |
|`userDisplayName`|`string`|<span data-ttu-id="4e758-143">Nome de exibição do usuário arriscado</span><span class="sxs-lookup"><span data-stu-id="4e758-143">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="4e758-144">Nome UPN de usuário arriscado</span><span class="sxs-lookup"><span data-stu-id="4e758-144">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e758-145">Relações</span><span class="sxs-lookup"><span data-stu-id="4e758-145">Relationships</span></span>

<span data-ttu-id="4e758-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4e758-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e758-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4e758-147">JSON representation</span></span>

<span data-ttu-id="4e758-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4e758-148">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUser"
}-->

```json
{
"id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isProcessing": "boolean",
"isDeleted": "boolean",
"riskDetail":  "string",
"riskLevel":  "string",
"riskState":  "string",
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->