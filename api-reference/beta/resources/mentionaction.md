---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MentionAction
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 48ac49c80a39fd6bc51b048a8eb7dab6e62da810
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974137"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="664d4-102">Tipo de recurso MentionAction</span><span class="sxs-lookup"><span data-stu-id="664d4-102">MentionAction resource type</span></span>

> <span data-ttu-id="664d4-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="664d4-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="664d4-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="664d4-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="664d4-105">O recurso **MentionAction** fornece informações sobre um [atividade][] que mencionou pessoas.</span><span class="sxs-lookup"><span data-stu-id="664d4-105">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[atividade]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="664d4-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="664d4-107">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.mentionAction"
}-->

```json
{
  "mentionees": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a><span data-ttu-id="664d4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="664d4-108">Properties</span></span>

| <span data-ttu-id="664d4-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="664d4-109">Property name</span></span> | <span data-ttu-id="664d4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="664d4-110">Type</span></span>                       | <span data-ttu-id="664d4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="664d4-111">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="664d4-112">mentionees</span><span class="sxs-lookup"><span data-stu-id="664d4-112">mentionees</span></span>    | <span data-ttu-id="664d4-113">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="664d4-113">[identitySet][] collection</span></span> | <span data-ttu-id="664d4-114">As identidades dos usuários mencionados nesta ação.</span><span class="sxs-lookup"><span data-stu-id="664d4-114">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="664d4-116">Comentários</span><span class="sxs-lookup"><span data-stu-id="664d4-116">Remarks</span></span>

<span data-ttu-id="664d4-117">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="664d4-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The MentionAction object provides information about who was mentioned during an activity.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/MentionAction"
} -->
