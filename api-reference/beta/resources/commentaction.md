---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: CommentAction
localization_priority: Normal
ms.openlocfilehash: 952a86161047ab869238feaba50b8ad4d8ce0658
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845595"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="9921d-102">Tipo de recurso CommentAction</span><span class="sxs-lookup"><span data-stu-id="9921d-102">CommentAction resource type</span></span>

> <span data-ttu-id="9921d-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9921d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9921d-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9921d-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9921d-105">O recurso **CommentAction** fornece informações sobre uma [atividade][] de comentário feitas em um item.</span><span class="sxs-lookup"><span data-stu-id="9921d-105">The **CommentAction** resource provides information about a comment [activity][] made on an item.</span></span>

[atividade]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="9921d-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9921d-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="9921d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9921d-108">Properties</span></span>

| <span data-ttu-id="9921d-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="9921d-109">Property name</span></span>    | <span data-ttu-id="9921d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9921d-110">Type</span></span>                       | <span data-ttu-id="9921d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9921d-111">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="9921d-112">isReply</span><span class="sxs-lookup"><span data-stu-id="9921d-112">isReply</span></span>          | <span data-ttu-id="9921d-113">booliano</span><span class="sxs-lookup"><span data-stu-id="9921d-113">boolean</span></span>                    | <span data-ttu-id="9921d-114">Se for verdadeiro, essa atividade era uma resposta para um thread de comentário existente.</span><span class="sxs-lookup"><span data-stu-id="9921d-114">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="9921d-115">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="9921d-115">parentAuthor</span></span>     | <span data-ttu-id="9921d-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="9921d-116">[identitySet][]</span></span>            | <span data-ttu-id="9921d-117">A identidade do usuário que iniciou o thread de comentários.</span><span class="sxs-lookup"><span data-stu-id="9921d-117">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="9921d-118">participantes</span><span class="sxs-lookup"><span data-stu-id="9921d-118">participants</span></span>     | <span data-ttu-id="9921d-119">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="9921d-119">[identitySet][] collection</span></span> | <span data-ttu-id="9921d-120">As identidades dos usuários que participam deste thread de comentário.</span><span class="sxs-lookup"><span data-stu-id="9921d-120">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="9921d-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="9921d-122">Remarks</span></span>

<span data-ttu-id="9921d-123">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="9921d-123">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The CommentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/CommentAction"
} -->
