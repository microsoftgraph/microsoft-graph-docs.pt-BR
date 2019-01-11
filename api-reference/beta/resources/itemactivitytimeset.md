---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityTimeSet
localization_priority: Normal
ms.openlocfilehash: 2ff3e1a2356c43457fe251928728632bd2228b10
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809889"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="2fa1f-102">Tipo de recurso ItemActivityTimeSet</span><span class="sxs-lookup"><span data-stu-id="2fa1f-102">ItemActivityTimeSet resource type</span></span>

> <span data-ttu-id="2fa1f-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2fa1f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2fa1f-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2fa1f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2fa1f-105">O recurso **ItemActivityTimeSet** fornece informações sobre quando uma [atividade][activity] em um item foi realizada.</span><span class="sxs-lookup"><span data-stu-id="2fa1f-105">The **ItemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="2fa1f-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2fa1f-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="2fa1f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2fa1f-107">Properties</span></span>

| <span data-ttu-id="2fa1f-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="2fa1f-108">Property name</span></span>    | <span data-ttu-id="2fa1f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fa1f-109">Type</span></span>           | <span data-ttu-id="2fa1f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fa1f-110">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="2fa1f-111">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="2fa1f-111">observedDateTime</span></span> | <span data-ttu-id="2fa1f-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fa1f-112">DateTimeOffset</span></span> | <span data-ttu-id="2fa1f-113">Quando observamos a atividade ocorrer.</span><span class="sxs-lookup"><span data-stu-id="2fa1f-113">When the activity was observed to take place.</span></span>
| <span data-ttu-id="2fa1f-114">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="2fa1f-114">recordedDateTime</span></span> | <span data-ttu-id="2fa1f-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fa1f-115">DateTimeOffset</span></span> | <span data-ttu-id="2fa1f-116">Quando a observação foi gravada no serviço.</span><span class="sxs-lookup"><span data-stu-id="2fa1f-116">When the observation was recorded on the service.</span></span>

<span data-ttu-id="2fa1f-117">A diferença entre os tempos de **observado** e **gravado** é particularmente importante para cenários de colaboração offline.</span><span class="sxs-lookup"><span data-stu-id="2fa1f-117">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="2fa1f-118">Se um usuário comenta em um arquivo enquanto está offline, o tempo pelo qual eles fazem o comentário é definido como o **observedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="2fa1f-118">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="2fa1f-119">Em um momento posterior quando o usuário se conectar novamente à nuvem e as alterações forem carregadas, esse momento posterior será definido como o **recordedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="2fa1f-119">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="remarks"></a><span data-ttu-id="2fa1f-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="2fa1f-120">Remarks</span></span>

<span data-ttu-id="2fa1f-121">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="2fa1f-121">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet"
} -->
