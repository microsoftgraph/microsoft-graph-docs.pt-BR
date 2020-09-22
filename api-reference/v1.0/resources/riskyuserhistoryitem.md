---
title: tipo de recurso riskyUserHistoryItem
description: item de histórico de usuários arriscados
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 551f008696b3c9507f1cae414c34de5a8779ab24
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984156"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="95352-103">tipo de recurso riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="95352-103">riskyUserHistoryItem resource type</span></span>

<span data-ttu-id="95352-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95352-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="95352-105">Representa o histórico de riscos de um usuário do Azure AD, conforme determinado pela proteção de identidade do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="95352-105">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span>


<span data-ttu-id="95352-106">Herda de [riskyUser](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="95352-106">Inherits from [riskyUser](../resources/riskyuser.md).</span></span>

## <a name="methods"></a><span data-ttu-id="95352-107">Methods</span><span class="sxs-lookup"><span data-stu-id="95352-107">Methods</span></span>
|<span data-ttu-id="95352-108">Método</span><span class="sxs-lookup"><span data-stu-id="95352-108">Method</span></span>|<span data-ttu-id="95352-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="95352-109">Return type</span></span>|<span data-ttu-id="95352-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="95352-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="95352-111">Histórico de lista</span><span class="sxs-lookup"><span data-stu-id="95352-111">List history</span></span>](../api/riskyuser-list-history.md)|<span data-ttu-id="95352-112">coleção [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="95352-112">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="95352-113">Obtenha o riskyUserHistoryItems da propriedade de navegação History.</span><span class="sxs-lookup"><span data-stu-id="95352-113">Get the riskyUserHistoryItems from the history navigation property.</span></span>|
|[<span data-ttu-id="95352-114">Obter histórico</span><span class="sxs-lookup"><span data-stu-id="95352-114">Get history</span></span>](../api/riskyuser-get-riskyuserhistoryitem.md)|[<span data-ttu-id="95352-115">riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="95352-115">riskyUserHistoryItem</span></span>](../resources/riskyuserhistoryitem.md)|<span data-ttu-id="95352-116">Leia as propriedades e os relacionamentos de um objeto [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) .</span><span class="sxs-lookup"><span data-stu-id="95352-116">Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="95352-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="95352-117">Properties</span></span>
|<span data-ttu-id="95352-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95352-118">Property</span></span>|<span data-ttu-id="95352-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="95352-119">Type</span></span>|<span data-ttu-id="95352-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="95352-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95352-121">atividade</span><span class="sxs-lookup"><span data-stu-id="95352-121">activity</span></span>|[<span data-ttu-id="95352-122">riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="95352-122">riskUserActivity</span></span>](../resources/riskuseractivity.md)|<span data-ttu-id="95352-123">A atividade relacionada à alteração no nível de risco do usuário.</span><span class="sxs-lookup"><span data-stu-id="95352-123">The activity related to user risk level change.</span></span>|
|<span data-ttu-id="95352-124">id</span><span class="sxs-lookup"><span data-stu-id="95352-124">id</span></span>|<span data-ttu-id="95352-125">String</span><span class="sxs-lookup"><span data-stu-id="95352-125">String</span></span>|<span data-ttu-id="95352-126">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="95352-126">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="95352-127">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="95352-127">initiatedBy</span></span>|<span data-ttu-id="95352-128">String</span><span class="sxs-lookup"><span data-stu-id="95352-128">String</span></span>|<span data-ttu-id="95352-129">A ID do ator que faz a operação.</span><span class="sxs-lookup"><span data-stu-id="95352-129">The id of actor that does the operation.</span></span>|
|<span data-ttu-id="95352-130">isDeleted</span><span class="sxs-lookup"><span data-stu-id="95352-130">isDeleted</span></span>|<span data-ttu-id="95352-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="95352-131">Boolean</span></span>| <span data-ttu-id="95352-132">Herdado de [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="95352-132">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="95352-133">isprocessoing</span><span class="sxs-lookup"><span data-stu-id="95352-133">isProcessing</span></span>|<span data-ttu-id="95352-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="95352-134">Boolean</span></span>| <span data-ttu-id="95352-135">Herdado de [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="95352-135">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="95352-136">riskDetail</span><span class="sxs-lookup"><span data-stu-id="95352-136">riskDetail</span></span>|<span data-ttu-id="95352-137">riskDetail</span><span class="sxs-lookup"><span data-stu-id="95352-137">riskDetail</span></span>|<span data-ttu-id="95352-138">Herdado de [riskyUser](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="95352-138">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="95352-139">Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="95352-139">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="95352-140">riskLastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="95352-140">riskLastUpdatedDateTime</span></span>|<span data-ttu-id="95352-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95352-141">DateTimeOffset</span></span>|<span data-ttu-id="95352-142">Herdado de [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="95352-142">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="95352-143">riskLevel</span><span class="sxs-lookup"><span data-stu-id="95352-143">riskLevel</span></span>|<span data-ttu-id="95352-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="95352-144">riskLevel</span></span>|<span data-ttu-id="95352-145">Herdado de [riskyUser](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="95352-145">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="95352-146">Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="95352-146">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="95352-147">riskState</span><span class="sxs-lookup"><span data-stu-id="95352-147">riskState</span></span>|<span data-ttu-id="95352-148">riskState</span><span class="sxs-lookup"><span data-stu-id="95352-148">riskState</span></span>|<span data-ttu-id="95352-149">Herdado de [riskyUser](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="95352-149">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="95352-150">Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="95352-150">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="95352-151">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="95352-151">userDisplayName</span></span>|<span data-ttu-id="95352-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="95352-152">String</span></span>|<span data-ttu-id="95352-153">Herdado de [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="95352-153">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="95352-154">userId</span><span class="sxs-lookup"><span data-stu-id="95352-154">userId</span></span>|<span data-ttu-id="95352-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="95352-155">String</span></span>|<span data-ttu-id="95352-156">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="95352-156">The id of the user.</span></span>|
|<span data-ttu-id="95352-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="95352-157">userPrincipalName</span></span>|<span data-ttu-id="95352-158">String</span><span class="sxs-lookup"><span data-stu-id="95352-158">String</span></span>|<span data-ttu-id="95352-159">Nome UPN de usuário arriscado.</span><span class="sxs-lookup"><span data-stu-id="95352-159">Risky user principal name.</span></span> <span data-ttu-id="95352-160">Herdado de [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="95352-160">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="95352-161">Relações</span><span class="sxs-lookup"><span data-stu-id="95352-161">Relationships</span></span>
|<span data-ttu-id="95352-162">Relação</span><span class="sxs-lookup"><span data-stu-id="95352-162">Relationship</span></span>|<span data-ttu-id="95352-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="95352-163">Type</span></span>|<span data-ttu-id="95352-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="95352-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95352-165">histórico</span><span class="sxs-lookup"><span data-stu-id="95352-165">history</span></span>|<span data-ttu-id="95352-166">coleção [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="95352-166">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>| <span data-ttu-id="95352-167">Herdado de [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="95352-167">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="95352-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="95352-168">JSON representation</span></span>
<span data-ttu-id="95352-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="95352-169">The following is a JSON representation of the resource.</span></span>
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


