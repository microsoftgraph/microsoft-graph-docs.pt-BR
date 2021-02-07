---
title: Tipo de recurso riskUserActivity
description: Detecções riskUserActivity
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7677832b2887bbb5dcddbeda21481da39f079669
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133221"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="69c45-103">Tipo de recurso riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="69c45-103">riskUserActivity resource type</span></span>

<span data-ttu-id="69c45-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69c45-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="69c45-105">Representa os activites de risco de um usuário do Azure AD, conforme determinado pelo Azure AD Identity Protection.</span><span class="sxs-lookup"><span data-stu-id="69c45-105">Represents the risk activites of an Azure AD user as determined by Azure AD Identity Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="69c45-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69c45-106">Properties</span></span>
|<span data-ttu-id="69c45-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69c45-107">Property</span></span>|<span data-ttu-id="69c45-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="69c45-108">Type</span></span>|<span data-ttu-id="69c45-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="69c45-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69c45-110">detalhe</span><span class="sxs-lookup"><span data-stu-id="69c45-110">detail</span></span>|<span data-ttu-id="69c45-111">riskDetail</span><span class="sxs-lookup"><span data-stu-id="69c45-111">riskDetail</span></span>|<span data-ttu-id="69c45-112">Detalhes do risco detectado.</span><span class="sxs-lookup"><span data-stu-id="69c45-112">Details of the detected risk.</span></span> <span data-ttu-id="69c45-113">Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="69c45-113">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="69c45-114">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="69c45-114">riskEventTypes</span></span>|<span data-ttu-id="69c45-115">String collection</span><span class="sxs-lookup"><span data-stu-id="69c45-115">String collection</span></span>|<span data-ttu-id="69c45-116">O tipo de evento de risco detectado.</span><span class="sxs-lookup"><span data-stu-id="69c45-116">The type of risk event detected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69c45-117">Relações</span><span class="sxs-lookup"><span data-stu-id="69c45-117">Relationships</span></span>
<span data-ttu-id="69c45-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="69c45-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="69c45-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69c45-119">JSON representation</span></span>
<span data-ttu-id="69c45-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69c45-120">The following is a JSON representation of the resource.</span></span>
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


