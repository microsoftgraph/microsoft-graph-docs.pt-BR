---
title: tipo de recurso riskyUserHistoryItem
description: item de histórico de usuários arriscados
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4bcf9e1834e8fff48a148095ffe7ddbd459ee23e
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895997"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="7b407-103">tipo de recurso riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="7b407-103">riskyUserHistoryItem resource type</span></span>

<span data-ttu-id="7b407-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b407-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7b407-105">Representa o histórico de riscos de um usuário do Azure AD, conforme determinado pela proteção de identidade do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7b407-105">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span>


<span data-ttu-id="7b407-106">Herda de [riskyUser](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="7b407-106">Inherits from [riskyUser](../resources/riskyuser.md).</span></span>

## <a name="methods"></a><span data-ttu-id="7b407-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="7b407-107">Methods</span></span>
|<span data-ttu-id="7b407-108">Método</span><span class="sxs-lookup"><span data-stu-id="7b407-108">Method</span></span>|<span data-ttu-id="7b407-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7b407-109">Return type</span></span>|<span data-ttu-id="7b407-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b407-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7b407-111">Histórico de lista</span><span class="sxs-lookup"><span data-stu-id="7b407-111">List history</span></span>](../api/riskyuser-list-history.md)|<span data-ttu-id="7b407-112">coleção [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="7b407-112">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="7b407-113">Obtenha o riskyUserHistoryItems da propriedade de navegação History.</span><span class="sxs-lookup"><span data-stu-id="7b407-113">Get the riskyUserHistoryItems from the history navigation property.</span></span>|
|[<span data-ttu-id="7b407-114">Obter histórico</span><span class="sxs-lookup"><span data-stu-id="7b407-114">Get history</span></span>](../api/riskyuser-get-riskyuserhistoryitem.md)|[<span data-ttu-id="7b407-115">riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="7b407-115">riskyUserHistoryItem</span></span>](../resources/riskyuserhistoryitem.md)|<span data-ttu-id="7b407-116">Leia as propriedades e os relacionamentos de um objeto [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) .</span><span class="sxs-lookup"><span data-stu-id="7b407-116">Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7b407-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b407-117">Properties</span></span>
|<span data-ttu-id="7b407-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b407-118">Property</span></span>|<span data-ttu-id="7b407-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b407-119">Type</span></span>|<span data-ttu-id="7b407-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b407-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b407-121">atividade</span><span class="sxs-lookup"><span data-stu-id="7b407-121">activity</span></span>|[<span data-ttu-id="7b407-122">riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="7b407-122">riskUserActivity</span></span>](../resources/riskuseractivity.md)|<span data-ttu-id="7b407-123">A atividade relacionada à alteração no nível de risco do usuário.</span><span class="sxs-lookup"><span data-stu-id="7b407-123">The activity related to user risk level change.</span></span>|
|<span data-ttu-id="7b407-124">id</span><span class="sxs-lookup"><span data-stu-id="7b407-124">id</span></span>|<span data-ttu-id="7b407-125">String</span><span class="sxs-lookup"><span data-stu-id="7b407-125">String</span></span>|<span data-ttu-id="7b407-126">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="7b407-126">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="7b407-127">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="7b407-127">initiatedBy</span></span>|<span data-ttu-id="7b407-128">String</span><span class="sxs-lookup"><span data-stu-id="7b407-128">String</span></span>|<span data-ttu-id="7b407-129">A ID do ator que faz a operação.</span><span class="sxs-lookup"><span data-stu-id="7b407-129">The id of actor that does the operation.</span></span>|
|<span data-ttu-id="7b407-130">isDeleted</span><span class="sxs-lookup"><span data-stu-id="7b407-130">isDeleted</span></span>|<span data-ttu-id="7b407-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b407-131">Boolean</span></span>| <span data-ttu-id="7b407-132">Herdado de [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="7b407-132">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="7b407-133">isprocessoing</span><span class="sxs-lookup"><span data-stu-id="7b407-133">isProcessing</span></span>|<span data-ttu-id="7b407-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b407-134">Boolean</span></span>| <span data-ttu-id="7b407-135">Herdado de [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="7b407-135">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="7b407-136">riskDetail</span><span class="sxs-lookup"><span data-stu-id="7b407-136">riskDetail</span></span>|<span data-ttu-id="7b407-137">riskDetail</span><span class="sxs-lookup"><span data-stu-id="7b407-137">riskDetail</span></span>|<span data-ttu-id="7b407-138">Herdado de [riskyUser](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="7b407-138">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="7b407-139">Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="7b407-139">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="7b407-140">riskLastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b407-140">riskLastUpdatedDateTime</span></span>|<span data-ttu-id="7b407-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b407-141">DateTimeOffset</span></span>|<span data-ttu-id="7b407-142">Herdado de [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="7b407-142">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="7b407-143">riskLevel</span><span class="sxs-lookup"><span data-stu-id="7b407-143">riskLevel</span></span>|<span data-ttu-id="7b407-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="7b407-144">riskLevel</span></span>|<span data-ttu-id="7b407-145">Herdado de [riskyUser](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="7b407-145">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="7b407-146">Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="7b407-146">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="7b407-147">riskState</span><span class="sxs-lookup"><span data-stu-id="7b407-147">riskState</span></span>|<span data-ttu-id="7b407-148">riskState</span><span class="sxs-lookup"><span data-stu-id="7b407-148">riskState</span></span>|<span data-ttu-id="7b407-149">Herdado de [riskyUser](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="7b407-149">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="7b407-150">Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="7b407-150">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="7b407-151">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="7b407-151">userDisplayName</span></span>|<span data-ttu-id="7b407-152">String</span><span class="sxs-lookup"><span data-stu-id="7b407-152">String</span></span>|<span data-ttu-id="7b407-153">Herdado de [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="7b407-153">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="7b407-154">userId</span><span class="sxs-lookup"><span data-stu-id="7b407-154">userId</span></span>|<span data-ttu-id="7b407-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7b407-155">String</span></span>|<span data-ttu-id="7b407-156">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="7b407-156">The id of the user.</span></span>|
|<span data-ttu-id="7b407-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7b407-157">userPrincipalName</span></span>|<span data-ttu-id="7b407-158">String</span><span class="sxs-lookup"><span data-stu-id="7b407-158">String</span></span>|<span data-ttu-id="7b407-159">Nome UPN de usuário arriscado.</span><span class="sxs-lookup"><span data-stu-id="7b407-159">Risky user principal name.</span></span> <span data-ttu-id="7b407-160">Herdado de [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="7b407-160">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b407-161">Relações</span><span class="sxs-lookup"><span data-stu-id="7b407-161">Relationships</span></span>
|<span data-ttu-id="7b407-162">Relação</span><span class="sxs-lookup"><span data-stu-id="7b407-162">Relationship</span></span>|<span data-ttu-id="7b407-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b407-163">Type</span></span>|<span data-ttu-id="7b407-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b407-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b407-165">histórico</span><span class="sxs-lookup"><span data-stu-id="7b407-165">history</span></span>|<span data-ttu-id="7b407-166">coleção [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="7b407-166">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>| <span data-ttu-id="7b407-167">Herdado de [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="7b407-167">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b407-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b407-168">JSON representation</span></span>
<span data-ttu-id="7b407-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b407-169">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUserHistoryItem",
  "baseType": "microsoft.graph.riskyUser",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
  "id": "String (identifier)",
  "isDeleted": "Boolean",
  "isProcessing": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "userId": "String",
  "initiatedBy": "String",
  "activity": {
    "@odata.type": "microsoft.graph.riskUserActivity"
  }
}
```

