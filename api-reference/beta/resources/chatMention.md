---
title: tipo de recurso de chatMessageMention
description: 'Representa uma mencionam em uma entidade chatMessage. O mencionam pode ser usuário, equipe, bot ou canal. '
localization_priority: Normal
ms.openlocfilehash: f37374a9793000ba641ed772e5dbfca5c0f1bd30
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515346"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="fdede-104">tipo de recurso de chatMessageMention</span><span class="sxs-lookup"><span data-stu-id="fdede-104">chatMessageMention resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdede-105">Representa uma mencionam em uma entidade [chatMessage](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="fdede-105">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="fdede-106">O mencionam pode ser usuário, equipe, bot ou canal.</span><span class="sxs-lookup"><span data-stu-id="fdede-106">The mention can be to a user, team, bot or channel.</span></span> 

## <a name="properties"></a><span data-ttu-id="fdede-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fdede-107">Properties</span></span>
| <span data-ttu-id="fdede-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fdede-108">Property</span></span>     | <span data-ttu-id="fdede-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fdede-109">Type</span></span>   |<span data-ttu-id="fdede-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdede-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fdede-111">id</span><span class="sxs-lookup"><span data-stu-id="fdede-111">id</span></span>|<span data-ttu-id="fdede-112">string</span><span class="sxs-lookup"><span data-stu-id="fdede-112">string</span></span>|<span data-ttu-id="fdede-113">ID da entidade que está sendo mencionada</span><span class="sxs-lookup"><span data-stu-id="fdede-113">Id of the entity being mentioned</span></span>|
|<span data-ttu-id="fdede-114">mentionText</span><span class="sxs-lookup"><span data-stu-id="fdede-114">mentionText</span></span>|<span data-ttu-id="fdede-115">string</span><span class="sxs-lookup"><span data-stu-id="fdede-115">string</span></span>|<span data-ttu-id="fdede-116">Cadeia de caracteres usada para representar o mencionam ex.: nome de exibição do usuário, o nome da equipe etc.</span><span class="sxs-lookup"><span data-stu-id="fdede-116">String used to represent the mention Ex: User display name, Team name etc</span></span>|
|<span data-ttu-id="fdede-117">mencionado</span><span class="sxs-lookup"><span data-stu-id="fdede-117">mentioned</span></span>|[<span data-ttu-id="fdede-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="fdede-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="fdede-119">O usuário que tenha sido mencionado</span><span class="sxs-lookup"><span data-stu-id="fdede-119">The user that was mentioned</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fdede-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fdede-120">JSON representation</span></span>

<span data-ttu-id="fdede-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fdede-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": "string (identifier)",
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
    "Error: /api-reference/beta/resources/chatMention.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
