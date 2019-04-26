---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RestoreAction
localization_priority: Normal
ms.openlocfilehash: fa92c4667d3421420b203cfc158c94d1b4cf78dd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343581"
---
# <a name="restoreaction-resource-type"></a><span data-ttu-id="992bc-102">Tipo de recurso RestoreAction</span><span class="sxs-lookup"><span data-stu-id="992bc-102">RestoreAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="992bc-103">A presença do recurso **RestoreAction** em uma [**itemActivity**][activity] indica que a atividade restaurou um item.</span><span class="sxs-lookup"><span data-stu-id="992bc-103">The presence of the **RestoreAction** resource on an [**itemActivity**][activity] indicates that the activity restored an item.</span></span>

<span data-ttu-id="992bc-104">**Observação**: embora esse recurso esteja vazio no momento, em revisões futuras da API ele poderá ser preenchido com propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="992bc-104">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="992bc-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="992bc-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.restoreAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="992bc-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="992bc-106">Properties</span></span>

<span data-ttu-id="992bc-107">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="992bc-107">None.</span></span> <span data-ttu-id="992bc-108">Esta faceta tem um valor nulo ou não nulo e não contém propriedades.</span><span class="sxs-lookup"><span data-stu-id="992bc-108">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="992bc-109">Comentários</span><span class="sxs-lookup"><span data-stu-id="992bc-109">Remarks</span></span>

<span data-ttu-id="992bc-110">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="992bc-110">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The RestoreAction object provides information about an activity that restored an item.",
  "keywords": "activities,activity,action,restore,undelete",
  "section": "documentation",
  "tocPath": "Resources/RestoreAction",
  "suppressions": []
}
-->
