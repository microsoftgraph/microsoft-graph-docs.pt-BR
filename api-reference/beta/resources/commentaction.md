---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: CommentAction
localization_priority: Normal
ms.openlocfilehash: e674c996002b3a54c92886dd1c5dca7a76c56b51
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543459"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="4d3e3-102">Tipo de recurso CommentAction</span><span class="sxs-lookup"><span data-stu-id="4d3e3-102">CommentAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d3e3-103">O recurso **CommentAction** fornece informações sobre uma [atividade][] de comentário feitas em um item.</span><span class="sxs-lookup"><span data-stu-id="4d3e3-103">The **CommentAction** resource provides information about a comment [activity][] made on an item.</span></span>

[atividade]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="4d3e3-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4d3e3-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="4d3e3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4d3e3-106">Properties</span></span>

| <span data-ttu-id="4d3e3-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="4d3e3-107">Property name</span></span>    | <span data-ttu-id="4d3e3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d3e3-108">Type</span></span>                       | <span data-ttu-id="4d3e3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d3e3-109">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="4d3e3-110">isReply</span><span class="sxs-lookup"><span data-stu-id="4d3e3-110">isReply</span></span>          | <span data-ttu-id="4d3e3-111">booliano</span><span class="sxs-lookup"><span data-stu-id="4d3e3-111">boolean</span></span>                    | <span data-ttu-id="4d3e3-112">Se for verdadeiro, essa atividade era uma resposta para um thread de comentário existente.</span><span class="sxs-lookup"><span data-stu-id="4d3e3-112">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="4d3e3-113">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="4d3e3-113">parentAuthor</span></span>     | <span data-ttu-id="4d3e3-114">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="4d3e3-114">[identitySet][]</span></span>            | <span data-ttu-id="4d3e3-115">A identidade do usuário que iniciou o thread de comentários.</span><span class="sxs-lookup"><span data-stu-id="4d3e3-115">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="4d3e3-116">participantes</span><span class="sxs-lookup"><span data-stu-id="4d3e3-116">participants</span></span>     | <span data-ttu-id="4d3e3-117">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="4d3e3-117">[identitySet][] collection</span></span> | <span data-ttu-id="4d3e3-118">As identidades dos usuários que participam deste thread de comentário.</span><span class="sxs-lookup"><span data-stu-id="4d3e3-118">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="4d3e3-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="4d3e3-120">Remarks</span></span>

<span data-ttu-id="4d3e3-121">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="4d3e3-121">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The CommentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/CommentAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/commentaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
