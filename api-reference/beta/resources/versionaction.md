---
author: daspek
description: A presença do recurso VersionAction em uma itemActivity indica que a atividade fez uma nova versão a ser criada.
ms.date: 09/14/2017
title: VersionAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 63b22b34abda4d1f268e16b00f65d6c4bb867c7e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519474"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="9bca4-103">Tipo de recurso VersionAction</span><span class="sxs-lookup"><span data-stu-id="9bca4-103">VersionAction resource type</span></span>

<span data-ttu-id="9bca4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9bca4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bca4-105">A presença do recurso **VersionAction** em uma [**itemActivity**][activity] indica que a atividade fez uma nova versão a ser criada.</span><span class="sxs-lookup"><span data-stu-id="9bca4-105">The presence of the **VersionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="9bca4-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9bca4-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="9bca4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9bca4-107">Properties</span></span>

| <span data-ttu-id="9bca4-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="9bca4-108">Property name</span></span> | <span data-ttu-id="9bca4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bca4-109">Type</span></span>   | <span data-ttu-id="9bca4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bca4-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="9bca4-111">newVersion</span><span class="sxs-lookup"><span data-stu-id="9bca4-111">newVersion</span></span>    | <span data-ttu-id="9bca4-112">string</span><span class="sxs-lookup"><span data-stu-id="9bca4-112">string</span></span> | <span data-ttu-id="9bca4-113">O nome da nova versão que foi criada por esta ação.</span><span class="sxs-lookup"><span data-stu-id="9bca4-113">The name of the new version that was created by this action.</span></span>

## <a name="remarks"></a><span data-ttu-id="9bca4-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="9bca4-114">Remarks</span></span>

<span data-ttu-id="9bca4-115">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="9bca4-115">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
