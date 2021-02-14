---
author: daspek
title: Tipo de recurso versionAction
description: O objeto VersionAction fornece informações sobre uma atividade que resultou em uma nova versão do item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f47d90c899ea9eb011837ae3c47dd6ec7ae22f30
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238985"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="c5bd0-103">Tipo de recurso versionAction</span><span class="sxs-lookup"><span data-stu-id="c5bd0-103">versionAction resource type</span></span>

<span data-ttu-id="c5bd0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5bd0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c5bd0-105">A presença do recurso **versionAction** em um [**itemActivity**][activity] indica que a atividade causou a criação de uma nova versão.</span><span class="sxs-lookup"><span data-stu-id="c5bd0-105">The presence of the **versionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

><span data-ttu-id="c5bd0-106">**Observação:** No momento, os registros de atividades do item só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="c5bd0-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="c5bd0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5bd0-107">Properties</span></span>

| <span data-ttu-id="c5bd0-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="c5bd0-108">Property name</span></span> | <span data-ttu-id="c5bd0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5bd0-109">Type</span></span>   | <span data-ttu-id="c5bd0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5bd0-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="c5bd0-111">newVersion</span><span class="sxs-lookup"><span data-stu-id="c5bd0-111">newVersion</span></span>    | <span data-ttu-id="c5bd0-112">string</span><span class="sxs-lookup"><span data-stu-id="c5bd0-112">string</span></span> | <span data-ttu-id="c5bd0-113">O nome da nova versão que foi criada por esta ação.</span><span class="sxs-lookup"><span data-stu-id="c5bd0-113">The name of the new version that was created by this action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5bd0-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5bd0-114">JSON representation</span></span>

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

