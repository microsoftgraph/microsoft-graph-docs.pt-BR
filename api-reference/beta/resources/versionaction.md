---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: VersionAction
localization_priority: Normal
ms.openlocfilehash: 59977b4ad84615f72dc008d671d64c62a2f4960f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345047"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="f6c5c-102">Tipo de recurso VersionAction</span><span class="sxs-lookup"><span data-stu-id="f6c5c-102">VersionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6c5c-103">A presença do recurso **VersionAction** em uma [**itemActivity**][activity] indica que a atividade fez uma nova versão a ser criada.</span><span class="sxs-lookup"><span data-stu-id="f6c5c-103">The presence of the **VersionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="f6c5c-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f6c5c-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.versionAction"
}-->

```json
{
  "newVersion": "string"
}
```

## <a name="properties"></a><span data-ttu-id="f6c5c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f6c5c-105">Properties</span></span>

| <span data-ttu-id="f6c5c-106">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="f6c5c-106">Property name</span></span> | <span data-ttu-id="f6c5c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6c5c-107">Type</span></span>   | <span data-ttu-id="f6c5c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6c5c-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="f6c5c-109">newVersion</span><span class="sxs-lookup"><span data-stu-id="f6c5c-109">newVersion</span></span>    | <span data-ttu-id="f6c5c-110">string</span><span class="sxs-lookup"><span data-stu-id="f6c5c-110">string</span></span> | <span data-ttu-id="f6c5c-111">O nome da nova versão que foi criada por esta ação.</span><span class="sxs-lookup"><span data-stu-id="f6c5c-111">The name of the new version that was created by this action.</span></span>

## <a name="remarks"></a><span data-ttu-id="f6c5c-112">Comentários</span><span class="sxs-lookup"><span data-stu-id="f6c5c-112">Remarks</span></span>

<span data-ttu-id="f6c5c-113">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="f6c5c-113">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The VersionAction object provides information about an activity that resulted in a new item version.",
  "keywords": "activities,activity,action,version",
  "section": "documentation",
  "tocPath": "Resources/VersionAction",
  "suppressions": []
}
-->
