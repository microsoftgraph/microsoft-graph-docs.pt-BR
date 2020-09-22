---
author: daspek
description: O recurso CommentAction fornece informações sobre uma atividade de comentário feitas em um item.
ms.date: 09/14/2017
title: CommentAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: f09785ae438225aa109a3b6a30790546cf3f30c1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033983"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="cfbcf-103">Tipo de recurso CommentAction</span><span class="sxs-lookup"><span data-stu-id="cfbcf-103">CommentAction resource type</span></span>

<span data-ttu-id="cfbcf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfbcf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfbcf-105">O recurso **CommentAction** fornece informações sobre uma [atividade][] de comentário feitas em um item.</span><span class="sxs-lookup"><span data-stu-id="cfbcf-105">The **CommentAction** resource provides information about a comment [activity][] made on an item.</span></span>

[atividade]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="cfbcf-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cfbcf-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="cfbcf-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cfbcf-108">Properties</span></span>

| <span data-ttu-id="cfbcf-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="cfbcf-109">Property name</span></span>    | <span data-ttu-id="cfbcf-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfbcf-110">Type</span></span>                       | <span data-ttu-id="cfbcf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfbcf-111">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="cfbcf-112">isReply</span><span class="sxs-lookup"><span data-stu-id="cfbcf-112">isReply</span></span>          | <span data-ttu-id="cfbcf-113">booliano</span><span class="sxs-lookup"><span data-stu-id="cfbcf-113">boolean</span></span>                    | <span data-ttu-id="cfbcf-114">Se for verdadeiro, essa atividade era uma resposta para um thread de comentário existente.</span><span class="sxs-lookup"><span data-stu-id="cfbcf-114">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="cfbcf-115">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="cfbcf-115">parentAuthor</span></span>     | <span data-ttu-id="cfbcf-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="cfbcf-116">[identitySet][]</span></span>            | <span data-ttu-id="cfbcf-117">A identidade do usuário que iniciou o thread de comentários.</span><span class="sxs-lookup"><span data-stu-id="cfbcf-117">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="cfbcf-118">participantes</span><span class="sxs-lookup"><span data-stu-id="cfbcf-118">participants</span></span>     | <span data-ttu-id="cfbcf-119">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="cfbcf-119">[identitySet][] collection</span></span> | <span data-ttu-id="cfbcf-120">As identidades dos usuários que participam deste thread de comentário.</span><span class="sxs-lookup"><span data-stu-id="cfbcf-120">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="cfbcf-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="cfbcf-122">Remarks</span></span>

<span data-ttu-id="cfbcf-123">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="cfbcf-123">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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


