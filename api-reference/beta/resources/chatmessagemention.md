---
title: tipo de recurso chatMessageMention
description: 'Representa uma menção em uma entidade chat. A menção pode ser a um usuário, uma equipe, um bot ou um canal. '
localization_priority: Normal
author: nkramer
ms.openlocfilehash: 5d7304325e48c87bfd75b57bf49585f66a77b262
ms.sourcegitcommit: a39db1154a07aa0dd7e96fb6f9d7e891a812207e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2019
ms.locfileid: "31889993"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="9da55-104">tipo de recurso chatMessageMention</span><span class="sxs-lookup"><span data-stu-id="9da55-104">chatMessageMention resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9da55-105">Representa uma menção em uma entidade [chat](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="9da55-105">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="9da55-106">A menção pode ser a um usuário, uma equipe, um bot ou um canal.</span><span class="sxs-lookup"><span data-stu-id="9da55-106">The mention can be to a user, team, bot, or channel.</span></span> 

## <a name="properties"></a><span data-ttu-id="9da55-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9da55-107">Properties</span></span>
| <span data-ttu-id="9da55-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9da55-108">Property</span></span>     | <span data-ttu-id="9da55-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9da55-109">Type</span></span>   |<span data-ttu-id="9da55-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9da55-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9da55-111">id</span><span class="sxs-lookup"><span data-stu-id="9da55-111">id</span></span>|<span data-ttu-id="9da55-112">int</span><span class="sxs-lookup"><span data-stu-id="9da55-112">int</span></span>|<span data-ttu-id="9da55-113">Índice da entidade que está sendo mencionada.</span><span class="sxs-lookup"><span data-stu-id="9da55-113">Index of the entity being mentioned.</span></span> <span data-ttu-id="9da55-114">Corresponde à <at id="index"> marca do corpo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="9da55-114">Matches with the <at id="index"> tag of the message body.</span></span>|
|<span data-ttu-id="9da55-115">mentionText</span><span class="sxs-lookup"><span data-stu-id="9da55-115">mentionText</span></span>|<span data-ttu-id="9da55-116">string</span><span class="sxs-lookup"><span data-stu-id="9da55-116">string</span></span>|<span data-ttu-id="9da55-117">Cadeia de caracteres usada para representar a menção.</span><span class="sxs-lookup"><span data-stu-id="9da55-117">String used to represent the mention.</span></span> <span data-ttu-id="9da55-118">Por exemplo, nome de exibição do usuário, nome da equipe.</span><span class="sxs-lookup"><span data-stu-id="9da55-118">For example, User display name, Team name.</span></span>|
|<span data-ttu-id="9da55-119">foi</span><span class="sxs-lookup"><span data-stu-id="9da55-119">mentioned</span></span>|[<span data-ttu-id="9da55-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="9da55-120">identitySet</span></span>](identityset.md)|<span data-ttu-id="9da55-121">A entidade (usuário, aplicativo, equipe ou canal) que foi mencionada.</span><span class="sxs-lookup"><span data-stu-id="9da55-121">The entity (user, application, team, or channel) that was mentioned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9da55-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9da55-122">JSON representation</span></span>

<span data-ttu-id="9da55-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9da55-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": "number",
  "mentionText": "string",
  "mentioned": "microsoft.graph.identitySet"
 }

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessagemention.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
