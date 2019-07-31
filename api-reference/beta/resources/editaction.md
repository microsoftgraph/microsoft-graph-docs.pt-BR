---
author: daspek
description: A presença do recurso EditAction em uma itemActivity indica que a atividade editou um item.
ms.date: 09/14/2017
title: EditAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 374b4f7374ba91360bdaa97e5bc36fb0f5aabbae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006504"
---
# <a name="editaction-resource-type"></a><span data-ttu-id="cf2c5-103">Tipo de recurso EditAction</span><span class="sxs-lookup"><span data-stu-id="cf2c5-103">EditAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf2c5-104">A presença do recurso **EditAction** em uma [**itemActivity**][activity] indica que a atividade editou um item.</span><span class="sxs-lookup"><span data-stu-id="cf2c5-104">The presence of the **EditAction** resource on an [**itemActivity**][activity] indicates that the activity edited an item.</span></span>

<span data-ttu-id="cf2c5-105">**Observação**: embora esse recurso esteja vazio no momento, em revisões futuras da API ele poderá ser preenchido com propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="cf2c5-105">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="cf2c5-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf2c5-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.editAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="cf2c5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf2c5-107">Properties</span></span>

<span data-ttu-id="cf2c5-108">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cf2c5-108">None.</span></span> <span data-ttu-id="cf2c5-109">Esta faceta tem um valor nulo ou não nulo e não contém propriedades.</span><span class="sxs-lookup"><span data-stu-id="cf2c5-109">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="cf2c5-110">Comentários</span><span class="sxs-lookup"><span data-stu-id="cf2c5-110">Remarks</span></span>

<span data-ttu-id="cf2c5-111">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="cf2c5-111">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
