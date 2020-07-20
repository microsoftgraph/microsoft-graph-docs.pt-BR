---
title: tipo de recurso riskUserActivity
description: detecções do riskUserActivity
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b8be06588194ad46722fc58b46c78e4a8bed53ec
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895913"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="c959c-103">tipo de recurso riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="c959c-103">riskUserActivity resource type</span></span>

<span data-ttu-id="c959c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c959c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c959c-105">Representa as atividades de risco de um usuário do Azure AD, conforme determinado pela proteção de identidade do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c959c-105">Represents the risk activites of an Azure AD user as determined by Azure AD Identity Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="c959c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c959c-106">Properties</span></span>
|<span data-ttu-id="c959c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c959c-107">Property</span></span>|<span data-ttu-id="c959c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c959c-108">Type</span></span>|<span data-ttu-id="c959c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c959c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c959c-110">detalhada</span><span class="sxs-lookup"><span data-stu-id="c959c-110">detail</span></span>|<span data-ttu-id="c959c-111">riskDetail</span><span class="sxs-lookup"><span data-stu-id="c959c-111">riskDetail</span></span>|<span data-ttu-id="c959c-112">Detalhes do risco detectado.</span><span class="sxs-lookup"><span data-stu-id="c959c-112">Details of the detected risk.</span></span> <span data-ttu-id="c959c-113">Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c959c-113">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c959c-114">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="c959c-114">riskEventTypes</span></span>|<span data-ttu-id="c959c-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c959c-115">String collection</span></span>|<span data-ttu-id="c959c-116">O tipo de evento de risco detectado.</span><span class="sxs-lookup"><span data-stu-id="c959c-116">The type of risk event detected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c959c-117">Relações</span><span class="sxs-lookup"><span data-stu-id="c959c-117">Relationships</span></span>
<span data-ttu-id="c959c-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c959c-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c959c-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c959c-119">JSON representation</span></span>
<span data-ttu-id="c959c-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c959c-120">The following is a JSON representation of the resource.</span></span>
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

