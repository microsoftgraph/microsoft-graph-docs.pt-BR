---
author: daspek
ms.author: dspektor
title: tipo de recurso DeleteAction
description: O objeto DeleteAction fornece informações sobre a exclusão de um item.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ba5004c17f1cc71f66420a81b5eb66603df00eee
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970619"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="9e4c2-103">tipo de recurso DeleteAction</span><span class="sxs-lookup"><span data-stu-id="9e4c2-103">deleteAction resource type</span></span>

<span data-ttu-id="9e4c2-104">A presença do recurso **DeleteAction** em uma myactivity [\*\*\*\*] [ activity] indica que a atividade excluiu um item.</span><span class="sxs-lookup"><span data-stu-id="9e4c2-104">The presence of the **deleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

><span data-ttu-id="9e4c2-105">**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="9e4c2-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="9e4c2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9e4c2-106">Properties</span></span>

| <span data-ttu-id="9e4c2-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="9e4c2-107">Property name</span></span> | <span data-ttu-id="9e4c2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e4c2-108">Type</span></span>   | <span data-ttu-id="9e4c2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e4c2-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="9e4c2-110">nome</span><span class="sxs-lookup"><span data-stu-id="9e4c2-110">name</span></span>          | <span data-ttu-id="9e4c2-111">string</span><span class="sxs-lookup"><span data-stu-id="9e4c2-111">string</span></span> | <span data-ttu-id="9e4c2-112">O nome do item que foi excluído.</span><span class="sxs-lookup"><span data-stu-id="9e4c2-112">The name of the item that was deleted.</span></span>
| <span data-ttu-id="9e4c2-113">objectType</span><span class="sxs-lookup"><span data-stu-id="9e4c2-113">objectType</span></span>    | <span data-ttu-id="9e4c2-114">string</span><span class="sxs-lookup"><span data-stu-id="9e4c2-114">string</span></span> | <span data-ttu-id="9e4c2-115">`File`ou `Folder`, dependendo do tipo do item excluído.</span><span class="sxs-lookup"><span data-stu-id="9e4c2-115">`File` or `Folder`, depending on the type of the deleted item.</span></span>


## <a name="json-representation"></a><span data-ttu-id="9e4c2-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9e4c2-116">JSON representation</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "The deleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction",
  "suppressions": []
}
-->
