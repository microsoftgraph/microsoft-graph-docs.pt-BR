---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RenameAction
localization_priority: Normal
ms.openlocfilehash: 88fa2738c014f028ebd2cc6e37f83151c7fc984a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835704"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="008c4-102">Tipo de recurso RenameAction</span><span class="sxs-lookup"><span data-stu-id="008c4-102">RenameAction resource type</span></span>

> <span data-ttu-id="008c4-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="008c4-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="008c4-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="008c4-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="008c4-105">A presença do recurso **RenameAction** em uma [**itemActivity**][activity] indica que a atividade renomeou um item.</span><span class="sxs-lookup"><span data-stu-id="008c4-105">The presence of the **RenameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="008c4-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="008c4-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.renameAction"
}-->

```json
{
  "oldName": "string",
  "newName": "string"
}
```

## <a name="properties"></a><span data-ttu-id="008c4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="008c4-107">Properties</span></span>

| <span data-ttu-id="008c4-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="008c4-108">Property name</span></span> | <span data-ttu-id="008c4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="008c4-109">Type</span></span>   | <span data-ttu-id="008c4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="008c4-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="008c4-111">oldName</span><span class="sxs-lookup"><span data-stu-id="008c4-111">oldName</span></span>       | <span data-ttu-id="008c4-112">string</span><span class="sxs-lookup"><span data-stu-id="008c4-112">string</span></span> | <span data-ttu-id="008c4-113">O nome anterior do item.</span><span class="sxs-lookup"><span data-stu-id="008c4-113">The previous name of the item.</span></span>
| <span data-ttu-id="008c4-114">newName</span><span class="sxs-lookup"><span data-stu-id="008c4-114">newName</span></span>       | <span data-ttu-id="008c4-115">string</span><span class="sxs-lookup"><span data-stu-id="008c4-115">string</span></span> | <span data-ttu-id="008c4-116">O novo nome do item.</span><span class="sxs-lookup"><span data-stu-id="008c4-116">The new name of the item.</span></span>

## <a name="remarks"></a><span data-ttu-id="008c4-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="008c4-117">Remarks</span></span>

<span data-ttu-id="008c4-118">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="008c4-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The RenameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/RenameAction"
} -->
