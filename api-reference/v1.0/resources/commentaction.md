---
author: daspek
title: Tipo de recurso commentAction
description: O objeto commentAction fornece informações sobre um comentário que foi feito em um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f2f3ab7f0798ee1020b107c38262a912fdae53ef
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238411"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="dd4ea-103">Tipo de recurso commentAction</span><span class="sxs-lookup"><span data-stu-id="dd4ea-103">commentAction resource type</span></span>

<span data-ttu-id="dd4ea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd4ea-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dd4ea-105">O **recurso commentAction** fornece informações sobre uma atividade [de comentário][] feita em um item.</span><span class="sxs-lookup"><span data-stu-id="dd4ea-105">The **commentAction** resource provides information about a comment [activity][] made on an item.</span></span>

><span data-ttu-id="dd4ea-106">**Observação:** No momento, os registros de atividades do item só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="dd4ea-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[atividade]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="dd4ea-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd4ea-108">Properties</span></span>

| <span data-ttu-id="dd4ea-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="dd4ea-109">Property name</span></span>    | <span data-ttu-id="dd4ea-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd4ea-110">Type</span></span>                       | <span data-ttu-id="dd4ea-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd4ea-111">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="dd4ea-112">isReply</span><span class="sxs-lookup"><span data-stu-id="dd4ea-112">isReply</span></span>          | <span data-ttu-id="dd4ea-113">booliano</span><span class="sxs-lookup"><span data-stu-id="dd4ea-113">boolean</span></span>                    | <span data-ttu-id="dd4ea-114">Se for verdadeiro, essa atividade era uma resposta para um thread de comentário existente.</span><span class="sxs-lookup"><span data-stu-id="dd4ea-114">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="dd4ea-115">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="dd4ea-115">parentAuthor</span></span>     | <span data-ttu-id="dd4ea-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="dd4ea-116">[identitySet][]</span></span>            | <span data-ttu-id="dd4ea-117">A identidade do usuário que iniciou o thread de comentários.</span><span class="sxs-lookup"><span data-stu-id="dd4ea-117">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="dd4ea-118">participantes</span><span class="sxs-lookup"><span data-stu-id="dd4ea-118">participants</span></span>     | <span data-ttu-id="dd4ea-119">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="dd4ea-119">[identitySet][] collection</span></span> | <span data-ttu-id="dd4ea-120">As identidades dos usuários que participam deste thread de comentário.</span><span class="sxs-lookup"><span data-stu-id="dd4ea-120">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="dd4ea-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd4ea-122">JSON representation</span></span>

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

