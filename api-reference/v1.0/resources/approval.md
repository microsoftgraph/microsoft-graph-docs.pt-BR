---
title: tipo de recurso de aprovação
description: O objeto de aprovação associado a um userConsentRequest.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c6d41146551586f681ebf5ed7fda735151f1efc5
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469511"
---
# <a name="approval-resource-type"></a><span data-ttu-id="562ec-103">tipo de recurso de aprovação</span><span class="sxs-lookup"><span data-stu-id="562ec-103">approval resource type</span></span>

<span data-ttu-id="562ec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="562ec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="562ec-105">Representa o objeto de aprovação para decisões associadas a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="562ec-105">Represents the approval object for decisions associated with a request.</span></span>

## <a name="properties"></a><span data-ttu-id="562ec-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="562ec-106">Properties</span></span>

|<span data-ttu-id="562ec-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="562ec-107">Property</span></span>|<span data-ttu-id="562ec-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="562ec-108">Type</span></span>|<span data-ttu-id="562ec-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="562ec-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="562ec-110">id</span><span class="sxs-lookup"><span data-stu-id="562ec-110">id</span></span>|<span data-ttu-id="562ec-111">String</span><span class="sxs-lookup"><span data-stu-id="562ec-111">String</span></span>|<span data-ttu-id="562ec-112">Identificador da decisão de aprovação.</span><span class="sxs-lookup"><span data-stu-id="562ec-112">Identifier of the approval decision.</span></span>|
|<span data-ttu-id="562ec-113">Estágios</span><span class="sxs-lookup"><span data-stu-id="562ec-113">stages</span></span>|<span data-ttu-id="562ec-114">[coleção approvalStage](../resources/approvalstage.md)</span><span class="sxs-lookup"><span data-stu-id="562ec-114">[approvalStage](../resources/approvalstage.md) collection</span></span>|<span data-ttu-id="562ec-115">Uma coleção de estágios na decisão de aprovação.</span><span class="sxs-lookup"><span data-stu-id="562ec-115">A collection of stages in the approval decision.</span></span> |

## <a name="relationships"></a><span data-ttu-id="562ec-116">Relações</span><span class="sxs-lookup"><span data-stu-id="562ec-116">Relationships</span></span>

|<span data-ttu-id="562ec-117">Relação</span><span class="sxs-lookup"><span data-stu-id="562ec-117">Relationship</span></span>|<span data-ttu-id="562ec-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="562ec-118">Type</span></span>|<span data-ttu-id="562ec-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="562ec-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="562ec-120">Estágios</span><span class="sxs-lookup"><span data-stu-id="562ec-120">stages</span></span>|<span data-ttu-id="562ec-121">[coleção approvalStage](../resources/approvalstage.md)</span><span class="sxs-lookup"><span data-stu-id="562ec-121">[approvalStage](../resources/approvalstage.md) collection</span></span>|<span data-ttu-id="562ec-122">Uma coleção de estágios na decisão de aprovação.</span><span class="sxs-lookup"><span data-stu-id="562ec-122">A collection of stages in the approval decision.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="562ec-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="562ec-123">JSON representation</span></span>

<span data-ttu-id="562ec-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="562ec-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approval",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.approval",
  "id": "String (identifier)",
  "stages": [{
        "@odata.type": "#microsoft.graph.approvalStage"
    }]
}
```
