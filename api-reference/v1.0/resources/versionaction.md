---
author: daspek
ms.author: dspektor
title: tipo de recurso versionaction
description: O objeto Versionaction fornece informações sobre uma atividade que resultou em uma nova versão do item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 22f06691824d2ffa5b773a796b4c456cb2fcaecc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033443"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="16556-103">tipo de recurso versionaction</span><span class="sxs-lookup"><span data-stu-id="16556-103">versionAction resource type</span></span>

<span data-ttu-id="16556-104">A presença do recurso **versionaction** em um myactivity indica que a atividade causou a criação de uma nova versão. [\*\*\*\*][activity]</span><span class="sxs-lookup"><span data-stu-id="16556-104">The presence of the **versionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

><span data-ttu-id="16556-105">**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="16556-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="16556-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="16556-106">Properties</span></span>

| <span data-ttu-id="16556-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="16556-107">Property name</span></span> | <span data-ttu-id="16556-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="16556-108">Type</span></span>   | <span data-ttu-id="16556-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="16556-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="16556-110">newVersion</span><span class="sxs-lookup"><span data-stu-id="16556-110">newVersion</span></span>    | <span data-ttu-id="16556-111">string</span><span class="sxs-lookup"><span data-stu-id="16556-111">string</span></span> | <span data-ttu-id="16556-112">O nome da nova versão que foi criada por esta ação.</span><span class="sxs-lookup"><span data-stu-id="16556-112">The name of the new version that was created by this action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="16556-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="16556-113">JSON representation</span></span>

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
