---
author: daspek
description: A presença do recurso VersionAction em uma itemActivity indica que a atividade fez uma nova versão a ser criada.
ms.date: 09/14/2017
title: VersionAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8eeec313ac4ed901d7552e2ad65d02edcaa821cd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007393"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="fb826-103">Tipo de recurso VersionAction</span><span class="sxs-lookup"><span data-stu-id="fb826-103">VersionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb826-104">A presença do recurso **VersionAction** em uma [**itemActivity**][activity] indica que a atividade fez uma nova versão a ser criada.</span><span class="sxs-lookup"><span data-stu-id="fb826-104">The presence of the **VersionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="fb826-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fb826-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="fb826-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fb826-106">Properties</span></span>

| <span data-ttu-id="fb826-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="fb826-107">Property name</span></span> | <span data-ttu-id="fb826-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb826-108">Type</span></span>   | <span data-ttu-id="fb826-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb826-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="fb826-110">newVersion</span><span class="sxs-lookup"><span data-stu-id="fb826-110">newVersion</span></span>    | <span data-ttu-id="fb826-111">string</span><span class="sxs-lookup"><span data-stu-id="fb826-111">string</span></span> | <span data-ttu-id="fb826-112">O nome da nova versão que foi criada por esta ação.</span><span class="sxs-lookup"><span data-stu-id="fb826-112">The name of the new version that was created by this action.</span></span>

## <a name="remarks"></a><span data-ttu-id="fb826-113">Comentários</span><span class="sxs-lookup"><span data-stu-id="fb826-113">Remarks</span></span>

<span data-ttu-id="fb826-114">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="fb826-114">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
