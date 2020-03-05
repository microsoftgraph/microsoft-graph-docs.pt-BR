---
author: daspek
description: A presença do recurso DeleteAction em uma itemActivity indica que a atividade excluiu um item.
ms.date: 09/14/2017
title: DeleteAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 453be9ad3764081207cfa51e56b69111186ff87b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507272"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="44582-103">Tipo de recurso DeleteAction</span><span class="sxs-lookup"><span data-stu-id="44582-103">DeleteAction resource type</span></span>

<span data-ttu-id="44582-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="44582-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44582-105">A presença do recurso **DeleteAction** em uma [**itemActivity**][activity] indica que a atividade excluiu um item.</span><span class="sxs-lookup"><span data-stu-id="44582-105">The presence of the **DeleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="44582-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44582-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="44582-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44582-107">Properties</span></span>

| <span data-ttu-id="44582-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="44582-108">Property name</span></span> | <span data-ttu-id="44582-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="44582-109">Type</span></span>   | <span data-ttu-id="44582-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="44582-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="44582-111">nome</span><span class="sxs-lookup"><span data-stu-id="44582-111">name</span></span>          | <span data-ttu-id="44582-112">string</span><span class="sxs-lookup"><span data-stu-id="44582-112">string</span></span> | <span data-ttu-id="44582-113">O nome do item que foi excluído.</span><span class="sxs-lookup"><span data-stu-id="44582-113">The name of the item that was deleted.</span></span>
| <span data-ttu-id="44582-114">objectType</span><span class="sxs-lookup"><span data-stu-id="44582-114">objectType</span></span>    | <span data-ttu-id="44582-115">string</span><span class="sxs-lookup"><span data-stu-id="44582-115">string</span></span> | <span data-ttu-id="44582-116">`File`ou `Folder`, dependendo do tipo do item excluído.</span><span class="sxs-lookup"><span data-stu-id="44582-116">`File` or `Folder`, depending on the type of the deleted item.</span></span>

## <a name="remarks"></a><span data-ttu-id="44582-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="44582-117">Remarks</span></span>

<span data-ttu-id="44582-118">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="44582-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
