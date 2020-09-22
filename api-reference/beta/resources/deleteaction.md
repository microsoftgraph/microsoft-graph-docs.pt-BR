---
author: daspek
description: A presença do recurso DeleteAction em uma itemActivity indica que a atividade excluiu um item.
ms.date: 09/14/2017
title: DeleteAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b8f00827a37ba9c010acd1b52e751bd55638afb3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049881"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="b7994-103">Tipo de recurso DeleteAction</span><span class="sxs-lookup"><span data-stu-id="b7994-103">DeleteAction resource type</span></span>

<span data-ttu-id="b7994-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7994-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7994-105">A presença do recurso **DeleteAction** em uma [**itemActivity**][activity] indica que a atividade excluiu um item.</span><span class="sxs-lookup"><span data-stu-id="b7994-105">The presence of the **DeleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="b7994-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b7994-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b7994-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b7994-107">Properties</span></span>

| <span data-ttu-id="b7994-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="b7994-108">Property name</span></span> | <span data-ttu-id="b7994-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7994-109">Type</span></span>   | <span data-ttu-id="b7994-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7994-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="b7994-111">nome</span><span class="sxs-lookup"><span data-stu-id="b7994-111">name</span></span>          | <span data-ttu-id="b7994-112">string</span><span class="sxs-lookup"><span data-stu-id="b7994-112">string</span></span> | <span data-ttu-id="b7994-113">O nome do item que foi excluído.</span><span class="sxs-lookup"><span data-stu-id="b7994-113">The name of the item that was deleted.</span></span>
| <span data-ttu-id="b7994-114">objectType</span><span class="sxs-lookup"><span data-stu-id="b7994-114">objectType</span></span>    | <span data-ttu-id="b7994-115">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7994-115">string</span></span> | <span data-ttu-id="b7994-116">`File` ou `Folder` , dependendo do tipo do item excluído.</span><span class="sxs-lookup"><span data-stu-id="b7994-116">`File` or `Folder`, depending on the type of the deleted item.</span></span>

## <a name="remarks"></a><span data-ttu-id="b7994-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="b7994-117">Remarks</span></span>

<span data-ttu-id="b7994-118">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="b7994-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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


