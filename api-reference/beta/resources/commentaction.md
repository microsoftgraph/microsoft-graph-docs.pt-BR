---
author: daspek
description: O recurso CommentAction fornece informações sobre uma atividade de comentário feitas em um item.
ms.date: 09/14/2017
title: CommentAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b7782c6e4dd30b503a9be88737ef6bd2dbad109b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973255"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="26ac8-103">Tipo de recurso CommentAction</span><span class="sxs-lookup"><span data-stu-id="26ac8-103">CommentAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26ac8-104">O recurso **CommentAction** fornece informações sobre uma [atividade][] de comentário feitas em um item.</span><span class="sxs-lookup"><span data-stu-id="26ac8-104">The **CommentAction** resource provides information about a comment [activity][] made on an item.</span></span>

[atividade]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="26ac8-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="26ac8-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="26ac8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="26ac8-107">Properties</span></span>

| <span data-ttu-id="26ac8-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="26ac8-108">Property name</span></span>    | <span data-ttu-id="26ac8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="26ac8-109">Type</span></span>                       | <span data-ttu-id="26ac8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="26ac8-110">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="26ac8-111">isReply</span><span class="sxs-lookup"><span data-stu-id="26ac8-111">isReply</span></span>          | <span data-ttu-id="26ac8-112">booliano</span><span class="sxs-lookup"><span data-stu-id="26ac8-112">boolean</span></span>                    | <span data-ttu-id="26ac8-113">Se for verdadeiro, essa atividade era uma resposta para um thread de comentário existente.</span><span class="sxs-lookup"><span data-stu-id="26ac8-113">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="26ac8-114">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="26ac8-114">parentAuthor</span></span>     | <span data-ttu-id="26ac8-115">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="26ac8-115">[identitySet][]</span></span>            | <span data-ttu-id="26ac8-116">A identidade do usuário que iniciou o thread de comentários.</span><span class="sxs-lookup"><span data-stu-id="26ac8-116">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="26ac8-117">participantes</span><span class="sxs-lookup"><span data-stu-id="26ac8-117">participants</span></span>     | <span data-ttu-id="26ac8-118">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="26ac8-118">[identitySet][] collection</span></span> | <span data-ttu-id="26ac8-119">As identidades dos usuários que participam deste thread de comentário.</span><span class="sxs-lookup"><span data-stu-id="26ac8-119">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="26ac8-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="26ac8-121">Remarks</span></span>

<span data-ttu-id="26ac8-122">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="26ac8-122">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The CommentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/CommentAction",
  "suppressions": []
}
-->
