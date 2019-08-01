---
author: daspek
ms.author: dspektor
title: tipo de recurso commentaction
description: O objeto commentaction fornece informações sobre um comentário que foi feito em um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 72502e466ff90ec0a299eb993346968c9038e2d1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029677"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="92f33-103">tipo de recurso commentaction</span><span class="sxs-lookup"><span data-stu-id="92f33-103">commentAction resource type</span></span>

<span data-ttu-id="92f33-104">O \*\*\*\* recurso commentaction fornece informações sobre uma [atividade][] de comentário feita em um item.</span><span class="sxs-lookup"><span data-stu-id="92f33-104">The **commentAction** resource provides information about a comment [activity][] made on an item.</span></span>

><span data-ttu-id="92f33-105">**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="92f33-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[atividade]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="92f33-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="92f33-107">Properties</span></span>

| <span data-ttu-id="92f33-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="92f33-108">Property name</span></span>    | <span data-ttu-id="92f33-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="92f33-109">Type</span></span>                       | <span data-ttu-id="92f33-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="92f33-110">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="92f33-111">isReply</span><span class="sxs-lookup"><span data-stu-id="92f33-111">isReply</span></span>          | <span data-ttu-id="92f33-112">booliano</span><span class="sxs-lookup"><span data-stu-id="92f33-112">boolean</span></span>                    | <span data-ttu-id="92f33-113">Se for verdadeiro, essa atividade era uma resposta para um thread de comentário existente.</span><span class="sxs-lookup"><span data-stu-id="92f33-113">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="92f33-114">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="92f33-114">parentAuthor</span></span>     | <span data-ttu-id="92f33-115">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="92f33-115">[identitySet][]</span></span>            | <span data-ttu-id="92f33-116">A identidade do usuário que iniciou o thread de comentários.</span><span class="sxs-lookup"><span data-stu-id="92f33-116">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="92f33-117">participantes</span><span class="sxs-lookup"><span data-stu-id="92f33-117">participants</span></span>     | <span data-ttu-id="92f33-118">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="92f33-118">[identitySet][] collection</span></span> | <span data-ttu-id="92f33-119">As identidades dos usuários que participam deste thread de comentário.</span><span class="sxs-lookup"><span data-stu-id="92f33-119">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="92f33-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="92f33-121">JSON representation</span></span>

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
