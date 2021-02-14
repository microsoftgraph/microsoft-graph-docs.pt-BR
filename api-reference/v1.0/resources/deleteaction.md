---
author: daspek
title: Tipo de recurso deleteAction
description: O objeto deleteAction fornece informações sobre a exclusão de um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: e78b4369606b0e0e3880fc3bfd13fdec263fcb58
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239629"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="8aadb-103">Tipo de recurso deleteAction</span><span class="sxs-lookup"><span data-stu-id="8aadb-103">deleteAction resource type</span></span>

<span data-ttu-id="8aadb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8aadb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8aadb-105">A presença do recurso **deleteAction** em um [**itemActivity**][activity] indica que a atividade excluiu um item.</span><span class="sxs-lookup"><span data-stu-id="8aadb-105">The presence of the **deleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

><span data-ttu-id="8aadb-106">**Observação:** No momento, os registros de atividades do item só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="8aadb-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="8aadb-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8aadb-107">Properties</span></span>

| <span data-ttu-id="8aadb-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="8aadb-108">Property name</span></span> | <span data-ttu-id="8aadb-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8aadb-109">Type</span></span>   | <span data-ttu-id="8aadb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8aadb-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="8aadb-111">name</span><span class="sxs-lookup"><span data-stu-id="8aadb-111">name</span></span>          | <span data-ttu-id="8aadb-112">string</span><span class="sxs-lookup"><span data-stu-id="8aadb-112">string</span></span> | <span data-ttu-id="8aadb-113">O nome do item que foi excluído.</span><span class="sxs-lookup"><span data-stu-id="8aadb-113">The name of the item that was deleted.</span></span>
| <span data-ttu-id="8aadb-114">objectType</span><span class="sxs-lookup"><span data-stu-id="8aadb-114">objectType</span></span>    | <span data-ttu-id="8aadb-115">string</span><span class="sxs-lookup"><span data-stu-id="8aadb-115">string</span></span> | <span data-ttu-id="8aadb-116">`File` ou `Folder` , dependendo do tipo do item excluído.</span><span class="sxs-lookup"><span data-stu-id="8aadb-116">`File` or `Folder`, depending on the type of the deleted item.</span></span>


## <a name="json-representation"></a><span data-ttu-id="8aadb-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8aadb-117">JSON representation</span></span>

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

