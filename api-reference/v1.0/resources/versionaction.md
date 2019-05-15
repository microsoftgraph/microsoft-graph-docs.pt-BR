---
author: daspek
ms.author: dspektor
title: tipo de recurso versionaction
description: O objeto Versionaction fornece informações sobre uma atividade que resultou em uma nova versão do item.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 0d05ad93c59ba736dd90276fc5e3db6e05740344
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970593"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="fd179-103">tipo de recurso versionaction</span><span class="sxs-lookup"><span data-stu-id="fd179-103">versionAction resource type</span></span>

<span data-ttu-id="fd179-104">A presença do recurso **versionaction** em um myactivity [\*\*\*\*] [ activity] indica que a atividade causou a criação de uma nova versão.</span><span class="sxs-lookup"><span data-stu-id="fd179-104">The presence of the **versionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

><span data-ttu-id="fd179-105">**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="fd179-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="fd179-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fd179-106">Properties</span></span>

| <span data-ttu-id="fd179-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="fd179-107">Property name</span></span> | <span data-ttu-id="fd179-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd179-108">Type</span></span>   | <span data-ttu-id="fd179-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd179-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="fd179-110">newVersion</span><span class="sxs-lookup"><span data-stu-id="fd179-110">newVersion</span></span>    | <span data-ttu-id="fd179-111">string</span><span class="sxs-lookup"><span data-stu-id="fd179-111">string</span></span> | <span data-ttu-id="fd179-112">O nome da nova versão que foi criada por esta ação.</span><span class="sxs-lookup"><span data-stu-id="fd179-112">The name of the new version that was created by this action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd179-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fd179-113">JSON representation</span></span>

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
