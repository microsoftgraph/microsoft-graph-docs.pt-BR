---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: DeleteAction
localization_priority: Normal
ms.openlocfilehash: 5e3b7cbf752d3ddb2c4b7bde3981d2a443028b92
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543235"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="e8a41-102">Tipo de recurso DeleteAction</span><span class="sxs-lookup"><span data-stu-id="e8a41-102">DeleteAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8a41-103">A presença do recurso **DeleteAction** em uma [**itemActivity**][activity] indica que a atividade excluiu um item.</span><span class="sxs-lookup"><span data-stu-id="e8a41-103">The presence of the **DeleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="e8a41-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e8a41-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.deleteAction"
}-->

```json
{
  "name": "string",
  "objectType": "File | Folder"
}
```

## <a name="properties"></a><span data-ttu-id="e8a41-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e8a41-105">Properties</span></span>

| <span data-ttu-id="e8a41-106">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="e8a41-106">Property name</span></span> | <span data-ttu-id="e8a41-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8a41-107">Type</span></span>   | <span data-ttu-id="e8a41-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8a41-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="e8a41-109">name</span><span class="sxs-lookup"><span data-stu-id="e8a41-109">name</span></span>          | <span data-ttu-id="e8a41-110">string</span><span class="sxs-lookup"><span data-stu-id="e8a41-110">string</span></span> | <span data-ttu-id="e8a41-111">O nome do item que foi excluído.</span><span class="sxs-lookup"><span data-stu-id="e8a41-111">The name of the item that was deleted.</span></span>
| <span data-ttu-id="e8a41-112">objectType</span><span class="sxs-lookup"><span data-stu-id="e8a41-112">objectType</span></span>    | <span data-ttu-id="e8a41-113">string</span><span class="sxs-lookup"><span data-stu-id="e8a41-113">string</span></span> | <span data-ttu-id="e8a41-114">`File`ou `Folder`, dependendo do tipo do item excluído.</span><span class="sxs-lookup"><span data-stu-id="e8a41-114">`File` or `Folder`, depending on the type of the deleted item.</span></span>

## <a name="remarks"></a><span data-ttu-id="e8a41-115">Comentários</span><span class="sxs-lookup"><span data-stu-id="e8a41-115">Remarks</span></span>

<span data-ttu-id="e8a41-116">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="e8a41-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The DeleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/deleteaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
