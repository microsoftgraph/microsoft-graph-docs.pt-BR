---
author: daspek
ms.author: dspektor
title: tipo de recurso commentaction
description: O objeto commentaction fornece informações sobre um comentário que foi feito em um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f3720d84624fa728a168515beb28422ab355b335
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531802"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="d86a0-103">tipo de recurso commentaction</span><span class="sxs-lookup"><span data-stu-id="d86a0-103">commentAction resource type</span></span>

<span data-ttu-id="d86a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d86a0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d86a0-105">O recurso **commentaction** fornece informações sobre uma [atividade][] de comentário feita em um item.</span><span class="sxs-lookup"><span data-stu-id="d86a0-105">The **commentAction** resource provides information about a comment [activity][] made on an item.</span></span>

><span data-ttu-id="d86a0-106">**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="d86a0-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[atividade]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="d86a0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d86a0-108">Properties</span></span>

| <span data-ttu-id="d86a0-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="d86a0-109">Property name</span></span>    | <span data-ttu-id="d86a0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d86a0-110">Type</span></span>                       | <span data-ttu-id="d86a0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d86a0-111">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="d86a0-112">isReply</span><span class="sxs-lookup"><span data-stu-id="d86a0-112">isReply</span></span>          | <span data-ttu-id="d86a0-113">booliano</span><span class="sxs-lookup"><span data-stu-id="d86a0-113">boolean</span></span>                    | <span data-ttu-id="d86a0-114">Se for verdadeiro, essa atividade era uma resposta para um thread de comentário existente.</span><span class="sxs-lookup"><span data-stu-id="d86a0-114">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="d86a0-115">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="d86a0-115">parentAuthor</span></span>     | <span data-ttu-id="d86a0-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="d86a0-116">[identitySet][]</span></span>            | <span data-ttu-id="d86a0-117">A identidade do usuário que iniciou o thread de comentários.</span><span class="sxs-lookup"><span data-stu-id="d86a0-117">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="d86a0-118">participantes</span><span class="sxs-lookup"><span data-stu-id="d86a0-118">participants</span></span>     | <span data-ttu-id="d86a0-119">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="d86a0-119">[identitySet][] collection</span></span> | <span data-ttu-id="d86a0-120">As identidades dos usuários que participam deste thread de comentário.</span><span class="sxs-lookup"><span data-stu-id="d86a0-120">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="d86a0-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d86a0-122">JSON representation</span></span>

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
