---
title: tipo de recurso chatMessageMention
description: 'Representa uma menção em uma entidade chat. A menção pode ser a um usuário, uma equipe, um bot ou um canal. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 130b1d536c881991a54e5b6fd06aee2f3f59483a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012958"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="ece6a-104">tipo de recurso chatMessageMention</span><span class="sxs-lookup"><span data-stu-id="ece6a-104">chatMessageMention resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ece6a-105">Representa uma menção em uma entidade [chat](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="ece6a-105">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="ece6a-106">A menção pode ser a um [usuário](user.md), uma [equipe](team.md), um bot ou um [canal](channel.md).</span><span class="sxs-lookup"><span data-stu-id="ece6a-106">The mention can be to a [user](user.md), [team](team.md), bot, or [channel](channel.md).</span></span> 

<span data-ttu-id="ece6a-107">Em um objeto **chat** que contém uma ou mais menciona, a propriedade de **conteúdo** do corpo da mensagem representa a mensagem de chat em HTML.</span><span class="sxs-lookup"><span data-stu-id="ece6a-107">In a **chatMessage** object that contains one or more mentions, the message body **content** property represents the chat message in HTML.</span></span> <span data-ttu-id="ece6a-108">Ele inclui o **mentionText** de cada menção em um elemento HTML `at` , com um `id` atributo que corresponde à propriedade **ID** da menção.</span><span class="sxs-lookup"><span data-stu-id="ece6a-108">It encloses the **mentionText** of each mention in an HTML `at` element, with an `id` attribute that corresponds to the **id** property of the mention.</span></span>

<span data-ttu-id="ece6a-109">Por exemplo, uma mensagem de chat contém duas menção, com o texto de menção "Megan" e "Alex", respectivamente.</span><span class="sxs-lookup"><span data-stu-id="ece6a-109">As an example, a chat message contains two mentions, with the mention text "Megan" and "Alex" respectively.</span></span> <span data-ttu-id="ece6a-110">A propriedade de **conteúdo** do `at` corpo especifica os elementos das duas mencionas da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="ece6a-110">Its body **content** property specifies `at` elements for the two mentions as follows:</span></span>

``` json
"body": {
    "contentType": "html",
    "content": "<div><div>Ah, <at id=\"0\">Megan</at>, <at id=\"1\">Alex</at>, I saw them in a separate folder. Thanks!</div>\n</div>"
}
```

<span data-ttu-id="ece6a-111">Na propriedade **Content** , a primeira menção tem um atributo HTML `id` de 0.</span><span class="sxs-lookup"><span data-stu-id="ece6a-111">In the **content** property, the first mention has an HTML `id` attribute of 0.</span></span> <span data-ttu-id="ece6a-112">Isso corresponde à propriedade **ID** dessa primeira instância de **chatMessageMention**, que também é 0.</span><span class="sxs-lookup"><span data-stu-id="ece6a-112">This corresponds to the **id** property of that first instance of **chatMessageMention**, which is also 0.</span></span>

<span data-ttu-id="ece6a-113">A segunda menção tem um `id` atributo de 1, correspondendo à propriedade **ID** da segunda instância, que é 1.</span><span class="sxs-lookup"><span data-stu-id="ece6a-113">The second mention has an `id` attribute of 1, matching the **id** property of the second instance, which is 1.</span></span>

<span data-ttu-id="ece6a-114">Para obter um contexto mais completo do exemplo, consulte [listar respostas de mensagens de canal](../api/channel-list-messagereplies.md#example).</span><span class="sxs-lookup"><span data-stu-id="ece6a-114">For a fuller context of the example, see [List channel message replies](../api/channel-list-messagereplies.md#example).</span></span>

## <a name="properties"></a><span data-ttu-id="ece6a-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ece6a-115">Properties</span></span>
| <span data-ttu-id="ece6a-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ece6a-116">Property</span></span>     | <span data-ttu-id="ece6a-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="ece6a-117">Type</span></span>   |<span data-ttu-id="ece6a-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="ece6a-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ece6a-119">id</span><span class="sxs-lookup"><span data-stu-id="ece6a-119">id</span></span>|<span data-ttu-id="ece6a-120">Int32</span><span class="sxs-lookup"><span data-stu-id="ece6a-120">Int32</span></span>|<span data-ttu-id="ece6a-121">Índice de uma entidade que está sendo mencionada no **chat**especificado.</span><span class="sxs-lookup"><span data-stu-id="ece6a-121">Index of an entity being mentioned in the specified **chatMessage**.</span></span> <span data-ttu-id="ece6a-122">Corresponde ao valor {index} na marca correspondente `<at id="{index}">` no corpo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="ece6a-122">Matches the {index} value in the corresponding `<at id="{index}">` tag in the message body.</span></span>|
|<span data-ttu-id="ece6a-123">mentionText</span><span class="sxs-lookup"><span data-stu-id="ece6a-123">mentionText</span></span>|<span data-ttu-id="ece6a-124">string</span><span class="sxs-lookup"><span data-stu-id="ece6a-124">string</span></span>|<span data-ttu-id="ece6a-125">Cadeia de caracteres usada para representar a menção.</span><span class="sxs-lookup"><span data-stu-id="ece6a-125">String used to represent the mention.</span></span> <span data-ttu-id="ece6a-126">Por exemplo, o nome de exibição de um usuário, o nome de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="ece6a-126">For example, a user's display name, a team name.</span></span>|
|<span data-ttu-id="ece6a-127">foi</span><span class="sxs-lookup"><span data-stu-id="ece6a-127">mentioned</span></span>|[<span data-ttu-id="ece6a-128">identitySet</span><span class="sxs-lookup"><span data-stu-id="ece6a-128">identitySet</span></span>](identityset.md)|<span data-ttu-id="ece6a-129">A entidade (usuário, aplicativo, equipe ou canal) que foi mencionada.</span><span class="sxs-lookup"><span data-stu-id="ece6a-129">The entity (user, application, team, or channel) that was mentioned.</span></span>  <span data-ttu-id="ece6a-130">Se fosse um canal ou uma equipe que foi @mentioned, o identityset contém uma propriedade de **conversa** que concede a ID da equipe/canal, e uma propriedade **conversationIdentityType** que representa a equipe ou o canal.</span><span class="sxs-lookup"><span data-stu-id="ece6a-130">If it was a channel or team that was @mentioned, the identitySet contains a **conversation** property giving the ID of the team/channel, and a **conversationIdentityType** property that represents either the team or channel.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ece6a-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ece6a-131">JSON representation</span></span>

<span data-ttu-id="ece6a-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ece6a-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": 1024,
  "mentionText": "string",
  "mentioned": {"@odata.type": "microsoft.graph.identitySet"}
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
  "suppressions": []
}
-->
