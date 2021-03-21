---
title: tipo de recurso riskyUser
description: item de usuários arriscados
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 82b622838ddd5e7fb8c00a969184bdd729926b23
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961080"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="eab9a-103">tipo de recurso riskyUser</span><span class="sxs-lookup"><span data-stu-id="eab9a-103">riskyUser resource type</span></span>

<span data-ttu-id="eab9a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eab9a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eab9a-105">Representa os usuários do Azure AD que estão em risco.</span><span class="sxs-lookup"><span data-stu-id="eab9a-105">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="eab9a-106">O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina.</span><span class="sxs-lookup"><span data-stu-id="eab9a-106">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="eab9a-107">Essa API fornece acesso programático a todos os usuários em risco no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="eab9a-107">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="eab9a-108">Para obter mais informações sobre eventos de risco, consulte [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span><span class="sxs-lookup"><span data-stu-id="eab9a-108">For more information about risk events, see [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>

><span data-ttu-id="eab9a-109">**Observação:** Usar a API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="eab9a-109">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="eab9a-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="eab9a-110">Methods</span></span>
|<span data-ttu-id="eab9a-111">Método</span><span class="sxs-lookup"><span data-stu-id="eab9a-111">Method</span></span>|<span data-ttu-id="eab9a-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eab9a-112">Return type</span></span>|<span data-ttu-id="eab9a-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="eab9a-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="eab9a-114">Listar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="eab9a-114">List riskyUsers</span></span>](../api/riskyuser-list.md)|<span data-ttu-id="eab9a-115">[Coleção riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="eab9a-115">[riskyUser](../resources/riskyuser.md) collection</span></span>|<span data-ttu-id="eab9a-116">Obter uma lista dos **objetos riskyUser** e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="eab9a-116">Get a list of the **riskyUser** objects and their properties.</span></span>|
|[<span data-ttu-id="eab9a-117">Obter riskyUser</span><span class="sxs-lookup"><span data-stu-id="eab9a-117">Get riskyUser</span></span>](../api/riskyuser-get.md)|[<span data-ttu-id="eab9a-118">riskyUser</span><span class="sxs-lookup"><span data-stu-id="eab9a-118">riskyUser</span></span>](../resources/riskyuser.md)|<span data-ttu-id="eab9a-119">Leia as propriedades e as relações de um **objeto riskyUser.**</span><span class="sxs-lookup"><span data-stu-id="eab9a-119">Read the properties and relationships of a **riskyUser** object.</span></span>|
|[<span data-ttu-id="eab9a-120">Descartar um riskyUser</span><span class="sxs-lookup"><span data-stu-id="eab9a-120">Dismiss a riskyUser</span></span>](../api/riskyuser-dismiss.md)|<span data-ttu-id="eab9a-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eab9a-121">None</span></span>|<span data-ttu-id="eab9a-122">Descartar o risco de um ou mais **objetos riskyUser.**</span><span class="sxs-lookup"><span data-stu-id="eab9a-122">Dismiss the risk of one or more **riskyUser** objects.</span></span> |
|[<span data-ttu-id="eab9a-123">Confirmar um riskyUser como comprometido</span><span class="sxs-lookup"><span data-stu-id="eab9a-123">Confirm a riskyUser as compromised</span></span>](../api/riskyuser-confirmcompromised.md)|<span data-ttu-id="eab9a-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eab9a-124">None</span></span>|<span data-ttu-id="eab9a-125">Confirme um ou mais **objetos riskyUser** como comprometidos.</span><span class="sxs-lookup"><span data-stu-id="eab9a-125">Confirm one or more **riskyUser** objects as compromised.</span></span>|
|[<span data-ttu-id="eab9a-126">Histórico de listas</span><span class="sxs-lookup"><span data-stu-id="eab9a-126">List history</span></span>](../api/riskyuser-list-history.md)|<span data-ttu-id="eab9a-127">[coleção riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="eab9a-127">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="eab9a-128">Obter **os riskyUserHistoryItems** da propriedade de navegação histórico.</span><span class="sxs-lookup"><span data-stu-id="eab9a-128">Get the **riskyUserHistoryItems** from the history navigation property.</span></span>|
|[<span data-ttu-id="eab9a-129">Obter histórico</span><span class="sxs-lookup"><span data-stu-id="eab9a-129">Get history</span></span>](../api/riskyuser-get-riskyuserhistoryitem.md)|[<span data-ttu-id="eab9a-130">riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="eab9a-130">riskyUserHistoryItem</span></span>](../resources/riskyuserhistoryitem.md)|<span data-ttu-id="eab9a-131">Leia as propriedades e as relações de um [objeto riskyUserHistoryItem.](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="eab9a-131">Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="eab9a-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eab9a-132">Properties</span></span>
|<span data-ttu-id="eab9a-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eab9a-133">Property</span></span>|<span data-ttu-id="eab9a-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="eab9a-134">Type</span></span>|<span data-ttu-id="eab9a-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="eab9a-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eab9a-136">id</span><span class="sxs-lookup"><span data-stu-id="eab9a-136">id</span></span>|<span data-ttu-id="eab9a-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eab9a-137">String</span></span>|<span data-ttu-id="eab9a-138">ID exclusiva do usuário em risco.</span><span class="sxs-lookup"><span data-stu-id="eab9a-138">Unique ID of the user at risk.</span></span>|
|<span data-ttu-id="eab9a-139">isDeleted</span><span class="sxs-lookup"><span data-stu-id="eab9a-139">isDeleted</span></span>|<span data-ttu-id="eab9a-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="eab9a-140">Boolean</span></span>|<span data-ttu-id="eab9a-141">Indica se o usuário foi excluído.</span><span class="sxs-lookup"><span data-stu-id="eab9a-141">Indicates whether the user is deleted.</span></span> <span data-ttu-id="eab9a-142">Os valores possíveis são: `true` e `false`.</span><span class="sxs-lookup"><span data-stu-id="eab9a-142">Possible values are: `true`, `false`.</span></span>|
|<span data-ttu-id="eab9a-143">isProcessing</span><span class="sxs-lookup"><span data-stu-id="eab9a-143">isProcessing</span></span>|<span data-ttu-id="eab9a-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="eab9a-144">Boolean</span></span>|<span data-ttu-id="eab9a-145">Indica se o estado de risco de um usuário está sendo processado pelo back-end.</span><span class="sxs-lookup"><span data-stu-id="eab9a-145">Indicates whether a user's risky state is being processed by the backend.</span></span>|
|<span data-ttu-id="eab9a-146">riskDetail</span><span class="sxs-lookup"><span data-stu-id="eab9a-146">riskDetail</span></span>|<span data-ttu-id="eab9a-147">riskDetail</span><span class="sxs-lookup"><span data-stu-id="eab9a-147">riskDetail</span></span>|<span data-ttu-id="eab9a-148">Detalhes do risco detectado.</span><span class="sxs-lookup"><span data-stu-id="eab9a-148">Details of the detected risk.</span></span> <span data-ttu-id="eab9a-149">Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="eab9a-149">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="eab9a-150">riskLastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="eab9a-150">riskLastUpdatedDateTime</span></span>|<span data-ttu-id="eab9a-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eab9a-151">DateTimeOffset</span></span>|<span data-ttu-id="eab9a-152">A data e a hora em que o usuário arriscado foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="eab9a-152">The date and time that the risky user was last updated.</span></span>  <span data-ttu-id="eab9a-153">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="eab9a-153">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="eab9a-154">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="eab9a-154">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="eab9a-155">riskLevel</span><span class="sxs-lookup"><span data-stu-id="eab9a-155">riskLevel</span></span>|<span data-ttu-id="eab9a-156">riskLevel</span><span class="sxs-lookup"><span data-stu-id="eab9a-156">riskLevel</span></span>|<span data-ttu-id="eab9a-157">Nível do usuário arriscado detectado.</span><span class="sxs-lookup"><span data-stu-id="eab9a-157">Level of the detected risky user.</span></span> <span data-ttu-id="eab9a-158">Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="eab9a-158">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="eab9a-159">riskState</span><span class="sxs-lookup"><span data-stu-id="eab9a-159">riskState</span></span>|<span data-ttu-id="eab9a-160">riskState</span><span class="sxs-lookup"><span data-stu-id="eab9a-160">riskState</span></span>|<span data-ttu-id="eab9a-161">Estado do risco do usuário.</span><span class="sxs-lookup"><span data-stu-id="eab9a-161">State of the user's risk.</span></span> <span data-ttu-id="eab9a-162">Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="eab9a-162">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="eab9a-163">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="eab9a-163">userDisplayName</span></span>|<span data-ttu-id="eab9a-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eab9a-164">String</span></span>|<span data-ttu-id="eab9a-165">Nome de exibição de usuário arriscado.</span><span class="sxs-lookup"><span data-stu-id="eab9a-165">Risky user display name.</span></span>|
|<span data-ttu-id="eab9a-166">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="eab9a-166">userPrincipalName</span></span>|<span data-ttu-id="eab9a-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eab9a-167">String</span></span>|<span data-ttu-id="eab9a-168">Nome principal do usuário arriscado.</span><span class="sxs-lookup"><span data-stu-id="eab9a-168">Risky user principal name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eab9a-169">Relações</span><span class="sxs-lookup"><span data-stu-id="eab9a-169">Relationships</span></span>
|<span data-ttu-id="eab9a-170">Relação</span><span class="sxs-lookup"><span data-stu-id="eab9a-170">Relationship</span></span>|<span data-ttu-id="eab9a-171">Tipo</span><span class="sxs-lookup"><span data-stu-id="eab9a-171">Type</span></span>|<span data-ttu-id="eab9a-172">Descrição</span><span class="sxs-lookup"><span data-stu-id="eab9a-172">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eab9a-173">history</span><span class="sxs-lookup"><span data-stu-id="eab9a-173">history</span></span>|<span data-ttu-id="eab9a-174">[coleção riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="eab9a-174">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|   <span data-ttu-id="eab9a-175">A atividade relacionada à alteração no nível de risco do usuário</span><span class="sxs-lookup"><span data-stu-id="eab9a-175">The activity related to user risk level change</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eab9a-176">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eab9a-176">JSON representation</span></span>
<span data-ttu-id="eab9a-177">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eab9a-177">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUser",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskyUser",
  "id": "String (identifier)",
  "isDeleted": "Boolean",
  "isProcessing": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String"
}
```
