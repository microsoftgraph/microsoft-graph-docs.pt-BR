---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: DeleteAction
localization_priority: Normal
ms.openlocfilehash: a380376a813df5f519464978851049e020ded8b8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340945"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="50421-102">Tipo de recurso DeleteAction</span><span class="sxs-lookup"><span data-stu-id="50421-102">DeleteAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50421-103">A presença do recurso **DeleteAction** em uma [**itemActivity**][activity] indica que a atividade excluiu um item.</span><span class="sxs-lookup"><span data-stu-id="50421-103">The presence of the **DeleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="50421-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50421-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="50421-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50421-105">Properties</span></span>

| <span data-ttu-id="50421-106">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="50421-106">Property name</span></span> | <span data-ttu-id="50421-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="50421-107">Type</span></span>   | <span data-ttu-id="50421-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="50421-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="50421-109">name</span><span class="sxs-lookup"><span data-stu-id="50421-109">name</span></span>          | <span data-ttu-id="50421-110">string</span><span class="sxs-lookup"><span data-stu-id="50421-110">string</span></span> | <span data-ttu-id="50421-111">O nome do item que foi excluído.</span><span class="sxs-lookup"><span data-stu-id="50421-111">The name of the item that was deleted.</span></span>
| <span data-ttu-id="50421-112">objectType</span><span class="sxs-lookup"><span data-stu-id="50421-112">objectType</span></span>    | <span data-ttu-id="50421-113">string</span><span class="sxs-lookup"><span data-stu-id="50421-113">string</span></span> | <span data-ttu-id="50421-114">`File`ou `Folder`, dependendo do tipo do item excluído.</span><span class="sxs-lookup"><span data-stu-id="50421-114">`File` or `Folder`, depending on the type of the deleted item.</span></span>

## <a name="remarks"></a><span data-ttu-id="50421-115">Comentários</span><span class="sxs-lookup"><span data-stu-id="50421-115">Remarks</span></span>

<span data-ttu-id="50421-116">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="50421-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The DeleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction",
  "suppressions": []
}
-->
