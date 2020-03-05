---
author: daspek
description: <decription>
ms.date: 09/14/2017
title: RestoreAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: ec2456105c7ae1844f97e80601fe2df3bf38d028
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521086"
---
# <a name="restoreaction-resource-type"></a><span data-ttu-id="5a1b8-102">Tipo de recurso RestoreAction</span><span class="sxs-lookup"><span data-stu-id="5a1b8-102">RestoreAction resource type</span></span>

<span data-ttu-id="5a1b8-103">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5a1b8-103">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a1b8-104">A presença do recurso **RestoreAction** em uma [**itemActivity**][activity] indica que a atividade restaurou um item.</span><span class="sxs-lookup"><span data-stu-id="5a1b8-104">The presence of the **RestoreAction** resource on an [**itemActivity**][activity] indicates that the activity restored an item.</span></span>

<span data-ttu-id="5a1b8-105">**Observação**: embora esse recurso esteja vazio no momento, em revisões futuras da API ele poderá ser preenchido com propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="5a1b8-105">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="5a1b8-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a1b8-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.restoreAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="5a1b8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a1b8-107">Properties</span></span>

<span data-ttu-id="5a1b8-108">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5a1b8-108">None.</span></span> <span data-ttu-id="5a1b8-109">Esta faceta tem um valor nulo ou não nulo e não contém propriedades.</span><span class="sxs-lookup"><span data-stu-id="5a1b8-109">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="5a1b8-110">Comentários</span><span class="sxs-lookup"><span data-stu-id="5a1b8-110">Remarks</span></span>

<span data-ttu-id="5a1b8-111">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="5a1b8-111">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
