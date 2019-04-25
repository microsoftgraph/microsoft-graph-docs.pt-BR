---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: CreateAction
localization_priority: Normal
ms.openlocfilehash: 0872e74004fa65f1f1778c6e6123bb3c8af6c823
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543396"
---
# <a name="createaction-resource-type"></a><span data-ttu-id="c6d2a-102">Tipo de recurso CreateAction</span><span class="sxs-lookup"><span data-stu-id="c6d2a-102">CreateAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6d2a-103">A presença do recurso **CreateAction** em uma [**itemActivity**][activity] indica que a atividade criou um item.</span><span class="sxs-lookup"><span data-stu-id="c6d2a-103">The presence of the **CreateAction** resource on an [**itemActivity**][activity] indicates that the activity created an item.</span></span>

<span data-ttu-id="c6d2a-104">**Observação**: embora esse recurso esteja vazio no momento, em revisões futuras da API ele poderá ser preenchido com propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="c6d2a-104">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="c6d2a-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c6d2a-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.createAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="c6d2a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c6d2a-106">Properties</span></span>

<span data-ttu-id="c6d2a-107">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c6d2a-107">None.</span></span> <span data-ttu-id="c6d2a-108">Esta faceta tem um valor nulo ou não nulo e não contém propriedades.</span><span class="sxs-lookup"><span data-stu-id="c6d2a-108">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="c6d2a-109">Comentários</span><span class="sxs-lookup"><span data-stu-id="c6d2a-109">Remarks</span></span>

<span data-ttu-id="c6d2a-110">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="c6d2a-110">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The CreateAction object provides information about the creation of an item.",
  "keywords": "activities,activity,action,create,creation",
  "section": "documentation",
  "tocPath": "Resources/CreateAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/createaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
