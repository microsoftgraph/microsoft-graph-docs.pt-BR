---
author: daspek
ms.author: dspektor
title: tipo de recurso DeleteAction
description: O objeto DeleteAction fornece informações sobre a exclusão de um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 4d19b41d886c459822abc2ea1b04acebd94c7b68
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531694"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="78825-103">tipo de recurso DeleteAction</span><span class="sxs-lookup"><span data-stu-id="78825-103">deleteAction resource type</span></span>

<span data-ttu-id="78825-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78825-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="78825-105">A presença do recurso **DeleteAction** em uma [**myactivity**][activity] indica que a atividade excluiu um item.</span><span class="sxs-lookup"><span data-stu-id="78825-105">The presence of the **deleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

><span data-ttu-id="78825-106">**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="78825-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="78825-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="78825-107">Properties</span></span>

| <span data-ttu-id="78825-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="78825-108">Property name</span></span> | <span data-ttu-id="78825-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="78825-109">Type</span></span>   | <span data-ttu-id="78825-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="78825-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="78825-111">nome</span><span class="sxs-lookup"><span data-stu-id="78825-111">name</span></span>          | <span data-ttu-id="78825-112">string</span><span class="sxs-lookup"><span data-stu-id="78825-112">string</span></span> | <span data-ttu-id="78825-113">O nome do item que foi excluído.</span><span class="sxs-lookup"><span data-stu-id="78825-113">The name of the item that was deleted.</span></span>
| <span data-ttu-id="78825-114">objectType</span><span class="sxs-lookup"><span data-stu-id="78825-114">objectType</span></span>    | <span data-ttu-id="78825-115">string</span><span class="sxs-lookup"><span data-stu-id="78825-115">string</span></span> | <span data-ttu-id="78825-116">`File`ou `Folder`, dependendo do tipo do item excluído.</span><span class="sxs-lookup"><span data-stu-id="78825-116">`File` or `Folder`, depending on the type of the deleted item.</span></span>


## <a name="json-representation"></a><span data-ttu-id="78825-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="78825-117">JSON representation</span></span>

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
