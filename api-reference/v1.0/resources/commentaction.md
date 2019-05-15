---
author: daspek
ms.author: dspektor
title: tipo de recurso commentaction
description: O objeto commentaction fornece informações sobre um comentário que foi feito em um item.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 12e6cd68d5809b8e4c1765234eeb77b40b30a78e
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970589"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="7c9c1-103">tipo de recurso commentaction</span><span class="sxs-lookup"><span data-stu-id="7c9c1-103">commentAction resource type</span></span>

<span data-ttu-id="7c9c1-104">O \*\*\*\* recurso commentaction fornece informações sobre uma [atividade][] de comentário feita em um item.</span><span class="sxs-lookup"><span data-stu-id="7c9c1-104">The **commentAction** resource provides information about a comment [activity][] made on an item.</span></span>

><span data-ttu-id="7c9c1-105">**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="7c9c1-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[atividade]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="7c9c1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7c9c1-107">Properties</span></span>

| <span data-ttu-id="7c9c1-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="7c9c1-108">Property name</span></span>    | <span data-ttu-id="7c9c1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c9c1-109">Type</span></span>                       | <span data-ttu-id="7c9c1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c9c1-110">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="7c9c1-111">isReply</span><span class="sxs-lookup"><span data-stu-id="7c9c1-111">isReply</span></span>          | <span data-ttu-id="7c9c1-112">booliano</span><span class="sxs-lookup"><span data-stu-id="7c9c1-112">boolean</span></span>                    | <span data-ttu-id="7c9c1-113">Se for verdadeiro, essa atividade era uma resposta para um thread de comentário existente.</span><span class="sxs-lookup"><span data-stu-id="7c9c1-113">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="7c9c1-114">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="7c9c1-114">parentAuthor</span></span>     | <span data-ttu-id="7c9c1-115">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="7c9c1-115">[identitySet][]</span></span>            | <span data-ttu-id="7c9c1-116">A identidade do usuário que iniciou o thread de comentários.</span><span class="sxs-lookup"><span data-stu-id="7c9c1-116">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="7c9c1-117">participantes</span><span class="sxs-lookup"><span data-stu-id="7c9c1-117">participants</span></span>     | <span data-ttu-id="7c9c1-118">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="7c9c1-118">[identitySet][] collection</span></span> | <span data-ttu-id="7c9c1-119">As identidades dos usuários que participam deste thread de comentário.</span><span class="sxs-lookup"><span data-stu-id="7c9c1-119">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="7c9c1-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7c9c1-121">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.commentAction"
}-->

```json
{
  "isReply": false,
  "parentAuthor": {"@odata.type": "microsoft.graph.identitySet"},
  "participants": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```
<!--
{
  "type": "#page.annotation",
  "description": "The commentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/commentAction",
  "suppressions": []
}
-->
