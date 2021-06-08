---
title: Tipo de recurso accessReviewInstanceDecisionItemResource
description: Cada item de decisão em uma revisão de acesso representa o acesso de uma entidade a um recurso. accessReviewInstanceDecisionItemResource representa o recurso associado ao item de decisão.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 502bb1d376ca7534bcf967acfa5030e44540f86c
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52788133"
---
# <a name="accessreviewinstancedecisionitemresource-resource-type"></a><span data-ttu-id="0f01e-104">Tipo de recurso accessReviewInstanceDecisionItemResource</span><span class="sxs-lookup"><span data-stu-id="0f01e-104">accessReviewInstanceDecisionItemResource resource type</span></span>

<span data-ttu-id="0f01e-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f01e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="0f01e-106">Cada item de decisão em uma revisão de acesso representa o acesso de uma entidade a um recurso.</span><span class="sxs-lookup"><span data-stu-id="0f01e-106">Every decision item in an access review represents a principal's access to a resource.</span></span> <span data-ttu-id="0f01e-107">accessReviewInstanceDecisionItemResource representa o recurso associado ao item de decisão.</span><span class="sxs-lookup"><span data-stu-id="0f01e-107">accessReviewInstanceDecisionItemResource represents the resource associated with the decision item.</span></span>

## <a name="properties"></a><span data-ttu-id="0f01e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0f01e-108">Properties</span></span>
|<span data-ttu-id="0f01e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f01e-109">Property</span></span>|<span data-ttu-id="0f01e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f01e-110">Type</span></span>|<span data-ttu-id="0f01e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f01e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f01e-112">displayName</span><span class="sxs-lookup"><span data-stu-id="0f01e-112">displayName</span></span>|<span data-ttu-id="0f01e-113">String</span><span class="sxs-lookup"><span data-stu-id="0f01e-113">String</span></span>|<span data-ttu-id="0f01e-114">Nome de exibição do recurso</span><span class="sxs-lookup"><span data-stu-id="0f01e-114">Display name of the resource</span></span>|
|<span data-ttu-id="0f01e-115">id</span><span class="sxs-lookup"><span data-stu-id="0f01e-115">id</span></span>|<span data-ttu-id="0f01e-116">String</span><span class="sxs-lookup"><span data-stu-id="0f01e-116">String</span></span>|<span data-ttu-id="0f01e-117">ID do Recurso</span><span class="sxs-lookup"><span data-stu-id="0f01e-117">Resource ID</span></span>|
|<span data-ttu-id="0f01e-118">tipo</span><span class="sxs-lookup"><span data-stu-id="0f01e-118">type</span></span>|<span data-ttu-id="0f01e-119">String</span><span class="sxs-lookup"><span data-stu-id="0f01e-119">String</span></span>|<span data-ttu-id="0f01e-120">Tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="0f01e-120">Type of resource.</span></span> <span data-ttu-id="0f01e-121">Os tipos `Group` incluem: `ServicePrincipal` , , , , `DirectoryRole` `AzureRole` `AccessPackageAssignmentPolicy` .</span><span class="sxs-lookup"><span data-stu-id="0f01e-121">Types include: `Group`, `ServicePrincipal`, `DirectoryRole`, `AzureRole`, `AccessPackageAssignmentPolicy`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f01e-122">Relações</span><span class="sxs-lookup"><span data-stu-id="0f01e-122">Relationships</span></span>
<span data-ttu-id="0f01e-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0f01e-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f01e-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0f01e-124">JSON representation</span></span>
<span data-ttu-id="0f01e-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0f01e-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemResource",
  "id": "String (identifier)",
  "displayName": "String",
  "type": "String"
}
```
