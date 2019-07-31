---
author: daspek
description: O recurso ItemActivityTimeSet fornece informações sobre quando uma atividade em um item foi realizada.
ms.date: 09/14/2017
title: ItemActivityTimeSet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c81bf7885ee1466e293236a987e90e21323daefd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010088"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="58e5b-103">Tipo de recurso ItemActivityTimeSet</span><span class="sxs-lookup"><span data-stu-id="58e5b-103">ItemActivityTimeSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58e5b-104">O recurso **ItemActivityTimeSet** fornece informações sobre quando uma [atividade][activity] em um item foi realizada.</span><span class="sxs-lookup"><span data-stu-id="58e5b-104">The **ItemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="58e5b-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="58e5b-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActivityTimeSet",
  "@type.aka": "oneDrive.times",
  "@property.aka": "observedDateTime=observedTime recordedDateTime=recordedTime"
}-->

```json
{
  "observedDateTime": "String (timestamp)",
  "recordedDateTime": "String (timestamp)"
}
```

## <a name="properties"></a><span data-ttu-id="58e5b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="58e5b-106">Properties</span></span>

| <span data-ttu-id="58e5b-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="58e5b-107">Property name</span></span>    | <span data-ttu-id="58e5b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="58e5b-108">Type</span></span>           | <span data-ttu-id="58e5b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="58e5b-109">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="58e5b-110">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="58e5b-110">observedDateTime</span></span> | <span data-ttu-id="58e5b-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58e5b-111">DateTimeOffset</span></span> | <span data-ttu-id="58e5b-112">Quando observamos a atividade ocorrer.</span><span class="sxs-lookup"><span data-stu-id="58e5b-112">When the activity was observed to take place.</span></span>
| <span data-ttu-id="58e5b-113">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="58e5b-113">recordedDateTime</span></span> | <span data-ttu-id="58e5b-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58e5b-114">DateTimeOffset</span></span> | <span data-ttu-id="58e5b-115">Quando a observação foi gravada no serviço.</span><span class="sxs-lookup"><span data-stu-id="58e5b-115">When the observation was recorded on the service.</span></span>

<span data-ttu-id="58e5b-116">A diferença entre os tempos de **observado** e **gravado** é particularmente importante para cenários de colaboração offline.</span><span class="sxs-lookup"><span data-stu-id="58e5b-116">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="58e5b-117">Se um usuário comenta em um arquivo enquanto está offline, o tempo pelo qual eles fazem o comentário é definido como o **observedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="58e5b-117">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="58e5b-118">Em um momento posterior quando o usuário se conectar novamente à nuvem e as alterações forem carregadas, esse momento posterior será definido como o **recordedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="58e5b-118">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="remarks"></a><span data-ttu-id="58e5b-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="58e5b-119">Remarks</span></span>

<span data-ttu-id="58e5b-120">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="58e5b-120">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet",
  "suppressions": []
}
-->
