---
title: tipo de recurso riskUserActivity
description: detecções do riskUserActivity
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b2b20a5796f5e1266271cd29d0768aa52927062a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991870"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="f1c5f-103">tipo de recurso riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="f1c5f-103">riskUserActivity resource type</span></span>

<span data-ttu-id="f1c5f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1c5f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f1c5f-105">Representa as atividades de risco de um usuário do Azure AD, conforme determinado pela proteção de identidade do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f1c5f-105">Represents the risk activites of an Azure AD user as determined by Azure AD Identity Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="f1c5f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1c5f-106">Properties</span></span>
|<span data-ttu-id="f1c5f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1c5f-107">Property</span></span>|<span data-ttu-id="f1c5f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1c5f-108">Type</span></span>|<span data-ttu-id="f1c5f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1c5f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1c5f-110">detalhada</span><span class="sxs-lookup"><span data-stu-id="f1c5f-110">detail</span></span>|<span data-ttu-id="f1c5f-111">riskDetail</span><span class="sxs-lookup"><span data-stu-id="f1c5f-111">riskDetail</span></span>|<span data-ttu-id="f1c5f-112">Detalhes do risco detectado.</span><span class="sxs-lookup"><span data-stu-id="f1c5f-112">Details of the detected risk.</span></span> <span data-ttu-id="f1c5f-113">Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f1c5f-113">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="f1c5f-114">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="f1c5f-114">riskEventTypes</span></span>|<span data-ttu-id="f1c5f-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1c5f-115">String collection</span></span>|<span data-ttu-id="f1c5f-116">O tipo de evento de risco detectado.</span><span class="sxs-lookup"><span data-stu-id="f1c5f-116">The type of risk event detected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1c5f-117">Relações</span><span class="sxs-lookup"><span data-stu-id="f1c5f-117">Relationships</span></span>
<span data-ttu-id="f1c5f-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f1c5f-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1c5f-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1c5f-119">JSON representation</span></span>
<span data-ttu-id="f1c5f-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1c5f-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.riskUserActivity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskUserActivity",
  "riskEventTypes": [
    "String"
  ],
  "detail": "String"
}
```


