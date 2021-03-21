---
title: tipo de recurso riskyUser
description: Representa os usuários do Azure AD que estão em risco. O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários em risco no Azure AD.
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
ms.openlocfilehash: d2e0942e92b1dcd648812503a923dac51a640be1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960317"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="2bb54-105">tipo de recurso riskyUser</span><span class="sxs-lookup"><span data-stu-id="2bb54-105">riskyUser resource type</span></span>

<span data-ttu-id="2bb54-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bb54-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bb54-107">Representa os usuários do Azure AD que estão em risco.</span><span class="sxs-lookup"><span data-stu-id="2bb54-107">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="2bb54-108">O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina.</span><span class="sxs-lookup"><span data-stu-id="2bb54-108">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="2bb54-109">Essa API fornece acesso programático a todos os usuários em risco no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2bb54-109">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="2bb54-110">Para obter mais informações sobre eventos de risco, consulte [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span><span class="sxs-lookup"><span data-stu-id="2bb54-110">For more information about risk events, see [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>

><span data-ttu-id="2bb54-111">**Observação:** Usar a API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="2bb54-111">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="2bb54-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="2bb54-112">Methods</span></span>

| <span data-ttu-id="2bb54-113">Método</span><span class="sxs-lookup"><span data-stu-id="2bb54-113">Method</span></span>   | <span data-ttu-id="2bb54-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2bb54-114">Return Type</span></span>|<span data-ttu-id="2bb54-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bb54-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2bb54-116">Listar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="2bb54-116">List riskyUsers</span></span>](../api/riskyusers-list.md) | <span data-ttu-id="2bb54-117">[Coleção riskyUser](riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="2bb54-117">[riskyUser](riskyuser.md) collection</span></span>|<span data-ttu-id="2bb54-118">Listar usuários arriscados e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="2bb54-118">List risky users and their properties.</span></span>|
|[<span data-ttu-id="2bb54-119">Obter riskyUser</span><span class="sxs-lookup"><span data-stu-id="2bb54-119">Get riskyUser</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="2bb54-120">riskyUser</span><span class="sxs-lookup"><span data-stu-id="2bb54-120">riskyUser</span></span>](riskyuser.md)|<span data-ttu-id="2bb54-121">Obter um usuário de risco específico e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="2bb54-121">Get a specific risky user and its properties.</span></span>|
|[<span data-ttu-id="2bb54-122">Histórico de listas</span><span class="sxs-lookup"><span data-stu-id="2bb54-122">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="2bb54-123">[coleção riskyUserHistoryItem](riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="2bb54-123">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="2bb54-124">Obter o histórico de risco de um usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2bb54-124">Get the risk history of an Azure AD user.</span></span>|
|[<span data-ttu-id="2bb54-125">Confirmar riskyUsers comprometidos</span><span class="sxs-lookup"><span data-stu-id="2bb54-125">Confirm riskyUsers compromised</span></span>](../api/riskyusers-confirmcompromised.md)|<span data-ttu-id="2bb54-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2bb54-126">None</span></span> |<span data-ttu-id="2bb54-127">Confirme um usuário arriscado como comprometido.</span><span class="sxs-lookup"><span data-stu-id="2bb54-127">Confirm a risky user as compromised.</span></span>|
|[<span data-ttu-id="2bb54-128">Descartar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="2bb54-128">Dismiss riskyUsers</span></span>](../api/riskyusers-dismiss.md)|<span data-ttu-id="2bb54-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2bb54-129">None</span></span> | <span data-ttu-id="2bb54-130">Descartar o risco de um usuário arriscado.</span><span class="sxs-lookup"><span data-stu-id="2bb54-130">Dismiss the risk of a risky user.</span></span>|

## <a name="properties"></a><span data-ttu-id="2bb54-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2bb54-131">Properties</span></span>

| <span data-ttu-id="2bb54-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2bb54-132">Property</span></span>   | <span data-ttu-id="2bb54-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="2bb54-133">Type</span></span>|<span data-ttu-id="2bb54-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bb54-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2bb54-135">id</span><span class="sxs-lookup"><span data-stu-id="2bb54-135">id</span></span>|<span data-ttu-id="2bb54-136">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bb54-136">string</span></span>|<span data-ttu-id="2bb54-137">ID exclusiva do usuário em risco.</span><span class="sxs-lookup"><span data-stu-id="2bb54-137">Unique ID of the user at risk.</span></span>|
|<span data-ttu-id="2bb54-138">isDeleted</span><span class="sxs-lookup"><span data-stu-id="2bb54-138">isDeleted</span></span>|<span data-ttu-id="2bb54-139">boolean</span><span class="sxs-lookup"><span data-stu-id="2bb54-139">boolean</span></span>|<span data-ttu-id="2bb54-140">Indica se o usuário foi excluído.</span><span class="sxs-lookup"><span data-stu-id="2bb54-140">Indicates whether the user is deleted.</span></span> <span data-ttu-id="2bb54-141">Os valores possíveis são: `true` e `false`.</span><span class="sxs-lookup"><span data-stu-id="2bb54-141">Possible values are: `true`, `false`.</span></span>|
|<span data-ttu-id="2bb54-142">isProcessing</span><span class="sxs-lookup"><span data-stu-id="2bb54-142">isProcessing</span></span>|<span data-ttu-id="2bb54-143">booliano</span><span class="sxs-lookup"><span data-stu-id="2bb54-143">boolean</span></span>|<span data-ttu-id="2bb54-144">Indica se o estado de risco de um usuário está sendo processado pelo back-end.</span><span class="sxs-lookup"><span data-stu-id="2bb54-144">Indicates whether a user's risky state is being processed by the backend.</span></span>|
|<span data-ttu-id="2bb54-145">riskLastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2bb54-145">riskLastUpdatedDateTime</span></span>|<span data-ttu-id="2bb54-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bb54-146">DateTimeOffset</span></span>|<span data-ttu-id="2bb54-147">A data e a hora em que o usuário arriscado foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2bb54-147">The date and time that the risky user was last updated.</span></span>  <span data-ttu-id="2bb54-148">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2bb54-148">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2bb54-149">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="2bb54-149">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="2bb54-150">riskLevel</span><span class="sxs-lookup"><span data-stu-id="2bb54-150">riskLevel</span></span>|<span data-ttu-id="2bb54-151">riskLevel</span><span class="sxs-lookup"><span data-stu-id="2bb54-151">riskLevel</span></span>| <span data-ttu-id="2bb54-152">Nível do usuário arriscado detectado.</span><span class="sxs-lookup"><span data-stu-id="2bb54-152">Level of the detected risky user.</span></span> <span data-ttu-id="2bb54-153">Os valores possíveis `low` são , , , , , `medium` `high` `hidden` `none` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="2bb54-153">The possible values are `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span>  |
|<span data-ttu-id="2bb54-154">riskState</span><span class="sxs-lookup"><span data-stu-id="2bb54-154">riskState</span></span>|<span data-ttu-id="2bb54-155">riskState</span><span class="sxs-lookup"><span data-stu-id="2bb54-155">riskState</span></span>| <span data-ttu-id="2bb54-156">Estado do risco do usuário.</span><span class="sxs-lookup"><span data-stu-id="2bb54-156">State of the user's risk.</span></span> <span data-ttu-id="2bb54-157">Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="2bb54-157">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>  |
|<span data-ttu-id="2bb54-158">riskDetail</span><span class="sxs-lookup"><span data-stu-id="2bb54-158">riskDetail</span></span>|<span data-ttu-id="2bb54-159">riskDetail</span><span class="sxs-lookup"><span data-stu-id="2bb54-159">riskDetail</span></span>| <span data-ttu-id="2bb54-160">Os valores possíveis `none` são , , , , , , , `adminGeneratedTemporaryPassword` , , , `userPerformedSecuredPasswordChange` , , `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `hidden` `adminConfirmedUserCompromised` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="2bb54-160">The possible values are `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>  |
|<span data-ttu-id="2bb54-161">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="2bb54-161">userDisplayName</span></span>|<span data-ttu-id="2bb54-162">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bb54-162">string</span></span>|<span data-ttu-id="2bb54-163">Nome de exibição de usuário arriscado.</span><span class="sxs-lookup"><span data-stu-id="2bb54-163">Risky user display name.</span></span>|
|<span data-ttu-id="2bb54-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2bb54-164">userPrincipalName</span></span>|<span data-ttu-id="2bb54-165">string</span><span class="sxs-lookup"><span data-stu-id="2bb54-165">string</span></span>|<span data-ttu-id="2bb54-166">Nome principal do usuário arriscado.</span><span class="sxs-lookup"><span data-stu-id="2bb54-166">Risky user principal name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2bb54-167">Relações</span><span class="sxs-lookup"><span data-stu-id="2bb54-167">Relationships</span></span>

<span data-ttu-id="2bb54-168">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2bb54-168">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2bb54-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2bb54-169">JSON representation</span></span>

<span data-ttu-id="2bb54-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2bb54-170">The following is a JSON representation of the resource.</span></span>

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
