---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: DeleteAction
localization_priority: Normal
ms.openlocfilehash: a845a6609991041f12266cd97e95460f96bf742f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876759"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="b0a5d-102">Tipo de recurso DeleteAction</span><span class="sxs-lookup"><span data-stu-id="b0a5d-102">DeleteAction resource type</span></span>

> <span data-ttu-id="b0a5d-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b0a5d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0a5d-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b0a5d-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b0a5d-105">A presença do recurso **DeleteAction** em uma [**itemActivity**][activity] indica que a atividade excluiu um item.</span><span class="sxs-lookup"><span data-stu-id="b0a5d-105">The presence of the **DeleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="b0a5d-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0a5d-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b0a5d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0a5d-107">Properties</span></span>

| <span data-ttu-id="b0a5d-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="b0a5d-108">Property name</span></span> | <span data-ttu-id="b0a5d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0a5d-109">Type</span></span>   | <span data-ttu-id="b0a5d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0a5d-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="b0a5d-111">name</span><span class="sxs-lookup"><span data-stu-id="b0a5d-111">name</span></span>          | <span data-ttu-id="b0a5d-112">string</span><span class="sxs-lookup"><span data-stu-id="b0a5d-112">string</span></span> | <span data-ttu-id="b0a5d-113">O nome do item que foi excluído.</span><span class="sxs-lookup"><span data-stu-id="b0a5d-113">The name of the item that was deleted.</span></span>
| <span data-ttu-id="b0a5d-114">objectType</span><span class="sxs-lookup"><span data-stu-id="b0a5d-114">objectType</span></span>    | <span data-ttu-id="b0a5d-115">string</span><span class="sxs-lookup"><span data-stu-id="b0a5d-115">string</span></span> | <span data-ttu-id="b0a5d-116">`File`ou `Folder`, dependendo do tipo de item excluído.</span><span class="sxs-lookup"><span data-stu-id="b0a5d-116">`File` or `Folder`, depending on the type of the deleted item.</span></span>

## <a name="remarks"></a><span data-ttu-id="b0a5d-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="b0a5d-117">Remarks</span></span>

<span data-ttu-id="b0a5d-118">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="b0a5d-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The DeleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction"
} -->
