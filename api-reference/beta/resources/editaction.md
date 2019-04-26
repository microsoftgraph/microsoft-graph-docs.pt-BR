---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: EditAction
localization_priority: Normal
ms.openlocfilehash: 68e6419206d03ba44cb34919ae46b8f1688d49a0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334624"
---
# <a name="editaction-resource-type"></a><span data-ttu-id="e173a-102">Tipo de recurso EditAction</span><span class="sxs-lookup"><span data-stu-id="e173a-102">EditAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e173a-103">A presença do recurso **EditAction** em uma [**itemActivity**][activity] indica que a atividade editou um item.</span><span class="sxs-lookup"><span data-stu-id="e173a-103">The presence of the **EditAction** resource on an [**itemActivity**][activity] indicates that the activity edited an item.</span></span>

<span data-ttu-id="e173a-104">**Observação**: embora esse recurso esteja vazio no momento, em revisões futuras da API ele poderá ser preenchido com propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="e173a-104">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="e173a-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e173a-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.editAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="e173a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e173a-106">Properties</span></span>

<span data-ttu-id="e173a-107">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e173a-107">None.</span></span> <span data-ttu-id="e173a-108">Esta faceta tem um valor nulo ou não nulo e não contém propriedades.</span><span class="sxs-lookup"><span data-stu-id="e173a-108">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="e173a-109">Comentários</span><span class="sxs-lookup"><span data-stu-id="e173a-109">Remarks</span></span>

<span data-ttu-id="e173a-110">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="e173a-110">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The EditAction object provides information about an activity that edited an item.",
  "keywords": "activities,activity,action,edit,modify",
  "section": "documentation",
  "tocPath": "Resources/EditAction",
  "suppressions": []
}
-->
