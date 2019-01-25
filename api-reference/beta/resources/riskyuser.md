---
title: tipo de recurso de riskyUsers
description: Representa os usuários do Windows Azure AD que estão em risco. Azure AD continuamente avalia o risco de usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários em risco em sua Azure AD.
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 27c189a81d6ba4e088c1242acfd2cf0d0f5c56c5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515710"
---
# <a name="riskyusers-resource-type"></a><span data-ttu-id="98233-105">tipo de recurso de riskyUsers</span><span class="sxs-lookup"><span data-stu-id="98233-105">riskyUsers resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98233-106">Representa os usuários do Windows Azure AD que estão em risco.</span><span class="sxs-lookup"><span data-stu-id="98233-106">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="98233-107">Azure AD continuamente avalia o risco de usuário com base em vários sinais e aprendizado de máquina.</span><span class="sxs-lookup"><span data-stu-id="98233-107">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="98233-108">Essa API fornece acesso programático a todos os usuários em risco em sua Azure AD.</span><span class="sxs-lookup"><span data-stu-id="98233-108">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

> <span data-ttu-id="98233-109">**Observação:** Esta API requer uma licença de P2 Premium do Windows Azure AD.</span><span class="sxs-lookup"><span data-stu-id="98233-109">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="98233-110">Para obter mais informações sobre eventos de risco, consulte [Proteção de identidade do Windows Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="98233-110">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

## <a name="methods"></a><span data-ttu-id="98233-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="98233-111">Methods</span></span>

| <span data-ttu-id="98233-112">Método</span><span class="sxs-lookup"><span data-stu-id="98233-112">Method</span></span>   | <span data-ttu-id="98233-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="98233-113">Return Type</span></span>|<span data-ttu-id="98233-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="98233-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="98233-115">Lista riskyUsers</span><span class="sxs-lookup"><span data-stu-id="98233-115">List riskyUsers</span></span>](../api/riskyusers-list.md) | [<span data-ttu-id="98233-116">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="98233-116">riskyUsers</span></span>](riskyuser.md) |<span data-ttu-id="98233-117">Listar usuários riscados e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="98233-117">List risky users and their properties.</span></span>|
|[<span data-ttu-id="98233-118">Obter riskyUsers</span><span class="sxs-lookup"><span data-stu-id="98233-118">Get riskyUsers</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="98233-119">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="98233-119">riskyUsers</span></span>](riskyuser.md)|<span data-ttu-id="98233-120">Obtenha um usuário riscado específico e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="98233-120">Get a specific risky user and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="98233-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="98233-121">Properties</span></span>

| <span data-ttu-id="98233-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98233-122">Property</span></span>   | <span data-ttu-id="98233-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="98233-123">Type</span></span>|<span data-ttu-id="98233-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="98233-124">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="98233-125">Id exclusiva do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="98233-125">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="98233-126">Indica se o usuário é excluído.</span><span class="sxs-lookup"><span data-stu-id="98233-126">Indicates whether the user is deleted.</span></span> <span data-ttu-id="98233-127">Os valores possíveis são: `true`,`false`</span><span class="sxs-lookup"><span data-stu-id="98233-127">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="98233-128">Indica se o usuário é um usuário convidado.</span><span class="sxs-lookup"><span data-stu-id="98233-128">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="98233-129">Os valores possíveis são: `true` e `false`.</span><span class="sxs-lookup"><span data-stu-id="98233-129">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="98233-130">True se a identidade do usuário encontra-se fora do locatário em consideração.</span><span class="sxs-lookup"><span data-stu-id="98233-130">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="98233-131">Esse usuário pode ser uma B2B ou um usuário B2C com identidade no Azure AD, MSA ou 3º provedor de identidade de terceiros.</span><span class="sxs-lookup"><span data-stu-id="98233-131">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="98233-132">False se a identidade do usuário estiver dentro do locatário em consideração</span><span class="sxs-lookup"><span data-stu-id="98233-132">False if user’s identity lies inside the tenant in consideration</span></span>|
|`riskDetail`|`riskDetail`|<span data-ttu-id="98233-133">Fornece o motivo por trás de um estado específico de um usuário riscado, entrar ou um evento de risco.</span><span class="sxs-lookup"><span data-stu-id="98233-133">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="98233-134">Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="98233-134">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="98233-135">O valor `none` significa que nenhuma ação foi realizada no usuário ou entrar até o momento.</span><span class="sxs-lookup"><span data-stu-id="98233-135">The value `none` means that no action has been performed on the user or sign-in so far.</span></span>|
|`riskLevel`|`riskLevel`|<span data-ttu-id="98233-136">Fornece o nível de risco geral de um usuário riscado, entrar ou um evento de risco.</span><span class="sxs-lookup"><span data-stu-id="98233-136">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="98233-137">Os valores possíveis são: `none`, `low`, `medium`, `high`, `hidden`, e `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="98233-137">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="98233-138">O valor `hidden` significa que o usuário ou entrar não foi habilitada para a proteção de identidade do Windows Azure AD.</span><span class="sxs-lookup"><span data-stu-id="98233-138">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskState`|`riskState`|<span data-ttu-id="98233-139">Fornece o 'estado de risco' de um usuário riscado, entrar ou um evento de risco.</span><span class="sxs-lookup"><span data-stu-id="98233-139">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="98233-140">Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="98233-140">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="98233-141">A data e hora em que o usuário riscado foi atualizada pela última vez</span><span class="sxs-lookup"><span data-stu-id="98233-141">The date and time that the risky user was last updated</span></span>|
|`userDisplayName`|`string`|<span data-ttu-id="98233-142">Nome de exibição do usuário riscado</span><span class="sxs-lookup"><span data-stu-id="98233-142">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="98233-143">Nome principal de usuário riscado</span><span class="sxs-lookup"><span data-stu-id="98233-143">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="98233-144">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="98233-144">Relationships</span></span>

| <span data-ttu-id="98233-145">Relação</span><span class="sxs-lookup"><span data-stu-id="98233-145">Relationship</span></span> | <span data-ttu-id="98233-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="98233-146">Type</span></span> |<span data-ttu-id="98233-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="98233-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98233-148">id</span><span class="sxs-lookup"><span data-stu-id="98233-148">id</span></span>|<span data-ttu-id="98233-149">UserObjectId</span><span class="sxs-lookup"><span data-stu-id="98233-149">UserObjectId</span></span>| <span data-ttu-id="98233-150">O identificador exclusivo do usuário com a qual um evento de determinado risco está associado.</span><span class="sxs-lookup"><span data-stu-id="98233-150">The unique identifier of the user with which a given risk event is associated with.</span></span>|
|<span data-ttu-id="98233-151">isGuest</span><span class="sxs-lookup"><span data-stu-id="98233-151">isGuest</span></span>|<span data-ttu-id="98233-152">isGuest</span><span class="sxs-lookup"><span data-stu-id="98233-152">isGuest</span></span>| <span data-ttu-id="98233-153">Um usuário riscado poderia ser um usuário Home (B2E) ou um usuário convidado (B2B, B2C).</span><span class="sxs-lookup"><span data-stu-id="98233-153">A risky user could be either a Home user (B2E) or a Guest user (B2B, B2C).</span></span>|
|<span data-ttu-id="98233-154">isDeleted</span><span class="sxs-lookup"><span data-stu-id="98233-154">isDeleted</span></span>|<span data-ttu-id="98233-155">isDeleted</span><span class="sxs-lookup"><span data-stu-id="98233-155">isDeleted</span></span>| <span data-ttu-id="98233-156">Um usuário pode ou não pode ser excluído.</span><span class="sxs-lookup"><span data-stu-id="98233-156">A user may or may not be deleted.</span></span> |
|<span data-ttu-id="98233-157">riskState</span><span class="sxs-lookup"><span data-stu-id="98233-157">riskState</span></span>|<span data-ttu-id="98233-158">riskState</span><span class="sxs-lookup"><span data-stu-id="98233-158">riskState</span></span>| <span data-ttu-id="98233-159">Um usuário riscado pode existir em um dos vários estados.</span><span class="sxs-lookup"><span data-stu-id="98233-159">A risky user could exist in one of multiple states.</span></span> |
|<span data-ttu-id="98233-160">riskDetail</span><span class="sxs-lookup"><span data-stu-id="98233-160">riskDetail</span></span>|<span data-ttu-id="98233-161">riskDetail</span><span class="sxs-lookup"><span data-stu-id="98233-161">riskDetail</span></span>| <span data-ttu-id="98233-162">Um usuário riscado poderia ser em um determinado estado por vários motivos.</span><span class="sxs-lookup"><span data-stu-id="98233-162">A risky user could be in a certain state because of multiple reasons.</span></span> |
|<span data-ttu-id="98233-163">riskLevel</span><span class="sxs-lookup"><span data-stu-id="98233-163">riskLevel</span></span>|<span data-ttu-id="98233-164">riskLevel</span><span class="sxs-lookup"><span data-stu-id="98233-164">riskLevel</span></span>| <span data-ttu-id="98233-165">Um usuário riscado poderia ser considerado um dos vários níveis de risco.</span><span class="sxs-lookup"><span data-stu-id="98233-165">A risky user could be considered one of multiple risk levels.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="98233-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="98233-166">JSON representation</span></span>

<span data-ttu-id="98233-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="98233-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskyusers"
}-->

```json
{
"id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isGuest": "boolean",
"isDeleted": "boolean",
"riskDetail":  {"@odata.type": "microsoft.graph.riskDetail"},
"riskLevel":  {"@odata.type": "microsoft.graph.riskLevel"},
"riskState":  {"@odata.type": "microsoft.graph.riskState"},
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/riskyuser.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
