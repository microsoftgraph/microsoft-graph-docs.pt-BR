---
author: daspek
description: A presença do recurso DeleteAction em uma itemActivity indica que a atividade excluiu um item.
ms.date: 09/14/2017
title: DeleteAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c5617c61f3221351930ab8d4bf940eaf1efa0629
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973832"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="cf08b-103">Tipo de recurso DeleteAction</span><span class="sxs-lookup"><span data-stu-id="cf08b-103">DeleteAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf08b-104">A presença do recurso **DeleteAction** em uma [**itemActivity**][activity] indica que a atividade excluiu um item.</span><span class="sxs-lookup"><span data-stu-id="cf08b-104">The presence of the **DeleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="cf08b-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf08b-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="cf08b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf08b-106">Properties</span></span>

| <span data-ttu-id="cf08b-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="cf08b-107">Property name</span></span> | <span data-ttu-id="cf08b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf08b-108">Type</span></span>   | <span data-ttu-id="cf08b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf08b-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="cf08b-110">name</span><span class="sxs-lookup"><span data-stu-id="cf08b-110">name</span></span>          | <span data-ttu-id="cf08b-111">string</span><span class="sxs-lookup"><span data-stu-id="cf08b-111">string</span></span> | <span data-ttu-id="cf08b-112">O nome do item que foi excluído.</span><span class="sxs-lookup"><span data-stu-id="cf08b-112">The name of the item that was deleted.</span></span>
| <span data-ttu-id="cf08b-113">objectType</span><span class="sxs-lookup"><span data-stu-id="cf08b-113">objectType</span></span>    | <span data-ttu-id="cf08b-114">string</span><span class="sxs-lookup"><span data-stu-id="cf08b-114">string</span></span> | <span data-ttu-id="cf08b-115">`File`ou `Folder`, dependendo do tipo do item excluído.</span><span class="sxs-lookup"><span data-stu-id="cf08b-115">`File` or `Folder`, depending on the type of the deleted item.</span></span>

## <a name="remarks"></a><span data-ttu-id="cf08b-116">Comentários</span><span class="sxs-lookup"><span data-stu-id="cf08b-116">Remarks</span></span>

<span data-ttu-id="cf08b-117">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="cf08b-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
