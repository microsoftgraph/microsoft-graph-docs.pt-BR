---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionStat
localization_priority: Normal
ms.openlocfilehash: 1d2ab438e7aaf5b0a6aede99290394a9a4ea7f0e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879524"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="5315f-102">tipo de recurso de itemActionStat</span><span class="sxs-lookup"><span data-stu-id="5315f-102">itemActionStat resource type</span></span>

> <span data-ttu-id="5315f-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5315f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5315f-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5315f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5315f-105">O recurso de **itemActionStat** fornece agregação detalhes sobre uma ação durante um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="5315f-105">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5315f-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5315f-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.itemActionStat",
}-->

```json
{
  "actionCount": 123,
  "actorCount": 60
}
```

## <a name="properties"></a><span data-ttu-id="5315f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5315f-107">Properties</span></span>

| <span data-ttu-id="5315f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5315f-108">Property</span></span>    | <span data-ttu-id="5315f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5315f-109">Type</span></span>  | <span data-ttu-id="5315f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5315f-110">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="5315f-111">actionCount</span><span class="sxs-lookup"><span data-stu-id="5315f-111">actionCount</span></span> | <span data-ttu-id="5315f-112">Int32</span><span class="sxs-lookup"><span data-stu-id="5315f-112">Int32</span></span> | <span data-ttu-id="5315f-113">O número de vezes que a ação foi realizada.</span><span class="sxs-lookup"><span data-stu-id="5315f-113">The number of times the action took place.</span></span> <span data-ttu-id="5315f-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5315f-114">Read-only.</span></span>
| <span data-ttu-id="5315f-115">actorCount</span><span class="sxs-lookup"><span data-stu-id="5315f-115">actorCount</span></span>  | <span data-ttu-id="5315f-116">Int32</span><span class="sxs-lookup"><span data-stu-id="5315f-116">Int32</span></span> | <span data-ttu-id="5315f-117">O número de atores distintos que executou a ação.</span><span class="sxs-lookup"><span data-stu-id="5315f-117">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="5315f-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5315f-118">Read-only.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActionStat"
} -->
