---
author: daspek
ms.author: dspektor
title: tipo de recurso DeleteAction
description: O objeto DeleteAction fornece informações sobre a exclusão de um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 93f605e74a0a483a94593a9aaa40d6fd30efe914
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032729"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="91b8e-103">tipo de recurso DeleteAction</span><span class="sxs-lookup"><span data-stu-id="91b8e-103">deleteAction resource type</span></span>

<span data-ttu-id="91b8e-104">A presença do recurso **DeleteAction** em uma myactivity indica que a atividade excluiu um item. [\*\*\*\*][activity]</span><span class="sxs-lookup"><span data-stu-id="91b8e-104">The presence of the **deleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

><span data-ttu-id="91b8e-105">**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="91b8e-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="91b8e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="91b8e-106">Properties</span></span>

| <span data-ttu-id="91b8e-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="91b8e-107">Property name</span></span> | <span data-ttu-id="91b8e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="91b8e-108">Type</span></span>   | <span data-ttu-id="91b8e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="91b8e-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="91b8e-110">name</span><span class="sxs-lookup"><span data-stu-id="91b8e-110">name</span></span>          | <span data-ttu-id="91b8e-111">string</span><span class="sxs-lookup"><span data-stu-id="91b8e-111">string</span></span> | <span data-ttu-id="91b8e-112">O nome do item que foi excluído.</span><span class="sxs-lookup"><span data-stu-id="91b8e-112">The name of the item that was deleted.</span></span>
| <span data-ttu-id="91b8e-113">objectType</span><span class="sxs-lookup"><span data-stu-id="91b8e-113">objectType</span></span>    | <span data-ttu-id="91b8e-114">string</span><span class="sxs-lookup"><span data-stu-id="91b8e-114">string</span></span> | <span data-ttu-id="91b8e-115">`File`ou `Folder`, dependendo do tipo do item excluído.</span><span class="sxs-lookup"><span data-stu-id="91b8e-115">`File` or `Folder`, depending on the type of the deleted item.</span></span>


## <a name="json-representation"></a><span data-ttu-id="91b8e-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="91b8e-116">JSON representation</span></span>

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
