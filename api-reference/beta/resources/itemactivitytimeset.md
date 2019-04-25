---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityTimeSet
localization_priority: Normal
ms.openlocfilehash: 474d20e08d96294a30029e764d0b01f5b0c6bfcd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581583"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="fc421-102">Tipo de recurso ItemActivityTimeSet</span><span class="sxs-lookup"><span data-stu-id="fc421-102">ItemActivityTimeSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc421-103">O recurso **ItemActivityTimeSet** fornece informações sobre quando uma [atividade][activity] em um item foi realizada.</span><span class="sxs-lookup"><span data-stu-id="fc421-103">The **ItemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="fc421-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc421-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="fc421-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc421-105">Properties</span></span>

| <span data-ttu-id="fc421-106">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="fc421-106">Property name</span></span>    | <span data-ttu-id="fc421-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc421-107">Type</span></span>           | <span data-ttu-id="fc421-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc421-108">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="fc421-109">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc421-109">observedDateTime</span></span> | <span data-ttu-id="fc421-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc421-110">DateTimeOffset</span></span> | <span data-ttu-id="fc421-111">Quando observamos a atividade ocorrer.</span><span class="sxs-lookup"><span data-stu-id="fc421-111">When the activity was observed to take place.</span></span>
| <span data-ttu-id="fc421-112">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc421-112">recordedDateTime</span></span> | <span data-ttu-id="fc421-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc421-113">DateTimeOffset</span></span> | <span data-ttu-id="fc421-114">Quando a observação foi gravada no serviço.</span><span class="sxs-lookup"><span data-stu-id="fc421-114">When the observation was recorded on the service.</span></span>

<span data-ttu-id="fc421-115">A diferença entre os tempos de **observado** e **gravado** é particularmente importante para cenários de colaboração offline.</span><span class="sxs-lookup"><span data-stu-id="fc421-115">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="fc421-116">Se um usuário comenta em um arquivo enquanto está offline, o tempo pelo qual eles fazem o comentário é definido como o **observedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="fc421-116">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="fc421-117">Em um momento posterior quando o usuário se conectar novamente à nuvem e as alterações forem carregadas, esse momento posterior será definido como o **recordedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="fc421-117">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="remarks"></a><span data-ttu-id="fc421-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="fc421-118">Remarks</span></span>

<span data-ttu-id="fc421-119">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="fc421-119">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemactivitytimeset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
