---
title: tipo de recurso chatMessageMention
description: 'Representa uma menção em uma entidade chat. A menção pode ser a um usuário, uma equipe, um bot ou um canal. '
localization_priority: Normal
ms.openlocfilehash: 45b4c60e22f727210150a64078935741dfb71640
ms.sourcegitcommit: 953895b28b6bae6e17eead938565fde289c49ef7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/05/2019
ms.locfileid: "31481367"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="4ff92-104">tipo de recurso chatMessageMention</span><span class="sxs-lookup"><span data-stu-id="4ff92-104">chatMessageMention resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ff92-105">Representa uma menção em uma entidade [chat](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="4ff92-105">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="4ff92-106">A menção pode ser a um usuário, uma equipe, um bot ou um canal.</span><span class="sxs-lookup"><span data-stu-id="4ff92-106">The mention can be to a user, team, bot or channel.</span></span> 

## <a name="properties"></a><span data-ttu-id="4ff92-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ff92-107">Properties</span></span>
| <span data-ttu-id="4ff92-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ff92-108">Property</span></span>     | <span data-ttu-id="4ff92-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ff92-109">Type</span></span>   |<span data-ttu-id="4ff92-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ff92-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ff92-111">id</span><span class="sxs-lookup"><span data-stu-id="4ff92-111">id</span></span>|<span data-ttu-id="4ff92-112">string</span><span class="sxs-lookup"><span data-stu-id="4ff92-112">string</span></span>|<span data-ttu-id="4ff92-113">ID da entidade que está sendo mencionada</span><span class="sxs-lookup"><span data-stu-id="4ff92-113">Id of the entity being mentioned</span></span>|
|<span data-ttu-id="4ff92-114">mentionText</span><span class="sxs-lookup"><span data-stu-id="4ff92-114">mentionText</span></span>|<span data-ttu-id="4ff92-115">string</span><span class="sxs-lookup"><span data-stu-id="4ff92-115">string</span></span>|<span data-ttu-id="4ff92-116">Cadeia de caracteres usada para representar a menção ex: nome de exibição do usuário, nome da equipe, etc.</span><span class="sxs-lookup"><span data-stu-id="4ff92-116">String used to represent the mention Ex: User display name, Team name etc</span></span>|
|<span data-ttu-id="4ff92-117">foi</span><span class="sxs-lookup"><span data-stu-id="4ff92-117">mentioned</span></span>|[<span data-ttu-id="4ff92-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="4ff92-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="4ff92-119">O usuário que foi mencionado</span><span class="sxs-lookup"><span data-stu-id="4ff92-119">The user that was mentioned</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4ff92-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ff92-120">JSON representation</span></span>

<span data-ttu-id="4ff92-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4ff92-121">The following is a JSON representation of the resource.</span></span>

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
    "Error: /api-reference/beta/resources/chatmessagemention.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
