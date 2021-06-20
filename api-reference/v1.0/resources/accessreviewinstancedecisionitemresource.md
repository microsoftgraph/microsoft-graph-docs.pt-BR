---
title: Tipo de recurso accessReviewInstanceDecisionItemResource
description: Representa o recurso associado ao item de decisão.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d75fb2f2b2fd4338f63d2c71893f2dab17524bc8
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030978"
---
# <a name="accessreviewinstancedecisionitemresource-resource-type"></a><span data-ttu-id="1f312-103">Tipo de recurso accessReviewInstanceDecisionItemResource</span><span class="sxs-lookup"><span data-stu-id="1f312-103">accessReviewInstanceDecisionItemResource resource type</span></span>

<span data-ttu-id="1f312-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f312-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1f312-105">Cada item de decisão em uma revisão de acesso representa o acesso de uma entidade a um recurso.</span><span class="sxs-lookup"><span data-stu-id="1f312-105">Every decision item in an access review represents a principal's access to a resource.</span></span> <span data-ttu-id="1f312-106">O objeto accessReviewInstanceDecisionItemResource representa o recurso associado ao item de decisão.</span><span class="sxs-lookup"><span data-stu-id="1f312-106">The accessReviewInstanceDecisionItemResource object represents the resource associated with the decision item.</span></span>

## <a name="properties"></a><span data-ttu-id="1f312-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1f312-107">Properties</span></span>
|<span data-ttu-id="1f312-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f312-108">Property</span></span>|<span data-ttu-id="1f312-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f312-109">Type</span></span>|<span data-ttu-id="1f312-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f312-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f312-111">displayName</span><span class="sxs-lookup"><span data-stu-id="1f312-111">displayName</span></span>|<span data-ttu-id="1f312-112">String</span><span class="sxs-lookup"><span data-stu-id="1f312-112">String</span></span>|<span data-ttu-id="1f312-113">Nome de exibição do recurso</span><span class="sxs-lookup"><span data-stu-id="1f312-113">Display name of the resource</span></span>|
|<span data-ttu-id="1f312-114">id</span><span class="sxs-lookup"><span data-stu-id="1f312-114">id</span></span>|<span data-ttu-id="1f312-115">String</span><span class="sxs-lookup"><span data-stu-id="1f312-115">String</span></span>|<span data-ttu-id="1f312-116">Identificador do recurso</span><span class="sxs-lookup"><span data-stu-id="1f312-116">Identifier of the resource</span></span>|
|<span data-ttu-id="1f312-117">tipo</span><span class="sxs-lookup"><span data-stu-id="1f312-117">type</span></span>|<span data-ttu-id="1f312-118">String</span><span class="sxs-lookup"><span data-stu-id="1f312-118">String</span></span>|<span data-ttu-id="1f312-119">Tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="1f312-119">Type of resource.</span></span> <span data-ttu-id="1f312-120">Os tipos `Group` incluem: `ServicePrincipal` , , , , `DirectoryRole` `AzureRole` `AccessPackageAssignmentPolicy` .</span><span class="sxs-lookup"><span data-stu-id="1f312-120">Types include: `Group`, `ServicePrincipal`, `DirectoryRole`, `AzureRole`, `AccessPackageAssignmentPolicy`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f312-121">Relações</span><span class="sxs-lookup"><span data-stu-id="1f312-121">Relationships</span></span>
<span data-ttu-id="1f312-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f312-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f312-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1f312-123">JSON representation</span></span>
<span data-ttu-id="1f312-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1f312-124">The following is a JSON representation of the resource.</span></span>
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
