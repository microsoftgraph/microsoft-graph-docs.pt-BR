---
author: daspek
ms.author: dspektor
title: tipo de recurso versionaction
description: O objeto Versionaction fornece informações sobre uma atividade que resultou em uma nova versão do item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 94efbb554420030eb33a814de72d5d79ab065738
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015278"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="da308-103">tipo de recurso versionaction</span><span class="sxs-lookup"><span data-stu-id="da308-103">versionAction resource type</span></span>

<span data-ttu-id="da308-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da308-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="da308-105">A presença do recurso **versionaction** em um [**myactivity**][activity] indica que a atividade causou a criação de uma nova versão.</span><span class="sxs-lookup"><span data-stu-id="da308-105">The presence of the **versionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

><span data-ttu-id="da308-106">**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="da308-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="da308-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da308-107">Properties</span></span>

| <span data-ttu-id="da308-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="da308-108">Property name</span></span> | <span data-ttu-id="da308-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="da308-109">Type</span></span>   | <span data-ttu-id="da308-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="da308-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="da308-111">newVersion</span><span class="sxs-lookup"><span data-stu-id="da308-111">newVersion</span></span>    | <span data-ttu-id="da308-112">string</span><span class="sxs-lookup"><span data-stu-id="da308-112">string</span></span> | <span data-ttu-id="da308-113">O nome da nova versão que foi criada por esta ação.</span><span class="sxs-lookup"><span data-stu-id="da308-113">The name of the new version that was created by this action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="da308-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da308-114">JSON representation</span></span>

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

