---
title: Tipo de recurso chatMessageMention
description: 'Representa uma menção em uma entidade chatMessage. A menção pode ser para um usuário, equipe, bot ou canal. '
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7af1260cbddfcecef21fc85ccf057c028681b061
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582757"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="e11e6-104">Tipo de recurso chatMessageMention</span><span class="sxs-lookup"><span data-stu-id="e11e6-104">chatMessageMention resource type</span></span>

<span data-ttu-id="e11e6-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e11e6-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e11e6-106">Representa uma menção em uma [entidade chatMessage.](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="e11e6-106">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="e11e6-107">A menção pode ser para um [usuário](user.md), [equipe,](team.md)bot ou [canal](channel.md).</span><span class="sxs-lookup"><span data-stu-id="e11e6-107">The mention can be to a [user](user.md), [team](team.md), bot, or [channel](channel.md).</span></span> 

<span data-ttu-id="e11e6-108">Em um **objeto chatMessage** que contém uma ou  mais menções, a propriedade de conteúdo do corpo da mensagem representa a mensagem de chat em HTML.</span><span class="sxs-lookup"><span data-stu-id="e11e6-108">In a **chatMessage** object that contains one or more mentions, the message body **content** property represents the chat message in HTML.</span></span> <span data-ttu-id="e11e6-109">Ele inclui o **mentionText** de cada menção em um elemento HTML, com um atributo que corresponde à propriedade `at` `id` **id** da menção.</span><span class="sxs-lookup"><span data-stu-id="e11e6-109">It encloses the **mentionText** of each mention in an HTML `at` element, with an `id` attribute that corresponds to the **id** property of the mention.</span></span>

<span data-ttu-id="e11e6-110">Como exemplo, uma mensagem de chat contém duas menções, com o texto de menção "Megan" e "Alex" respectivamente.</span><span class="sxs-lookup"><span data-stu-id="e11e6-110">As an example, a chat message contains two mentions, with the mention text "Megan" and "Alex" respectively.</span></span> <span data-ttu-id="e11e6-111">Sua propriedade **de conteúdo** do corpo especifica elementos para as `at` duas menções da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="e11e6-111">Its body **content** property specifies `at` elements for the two mentions as follows:</span></span>

``` json
"body": {
    "contentType": "html",
    "content": "<div><div>Ah, <at id=\"0\">Megan</at>, <at id=\"1\">Alex</at>, I saw them in a separate folder. Thanks!</div>\n</div>"
}
```

<span data-ttu-id="e11e6-112">Na propriedade **content,** a primeira menção tem um atributo HTML `id` de 0.</span><span class="sxs-lookup"><span data-stu-id="e11e6-112">In the **content** property, the first mention has an HTML `id` attribute of 0.</span></span> <span data-ttu-id="e11e6-113">Isso corresponde à propriedade **id** da primeira instância **do chatMessageMention**, que também é 0.</span><span class="sxs-lookup"><span data-stu-id="e11e6-113">This corresponds to the **id** property of that first instance of **chatMessageMention**, which is also 0.</span></span>

<span data-ttu-id="e11e6-114">A segunda menção tem um atributo 1, que corresponde à `id` **propriedade id** da segunda instância, que é 1.</span><span class="sxs-lookup"><span data-stu-id="e11e6-114">The second mention has an `id` attribute of 1, matching the **id** property of the second instance, which is 1.</span></span>

<span data-ttu-id="e11e6-115">Para um contexto mais completo do exemplo, consulte [List channel message replies](../api/chatmessage-list-replies.md#example).</span><span class="sxs-lookup"><span data-stu-id="e11e6-115">For a fuller context of the example, see [List channel message replies](../api/chatmessage-list-replies.md#example).</span></span>

## <a name="properties"></a><span data-ttu-id="e11e6-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e11e6-116">Properties</span></span>

| <span data-ttu-id="e11e6-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e11e6-117">Property</span></span>| <span data-ttu-id="e11e6-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="e11e6-118">Type</span></span>|<span data-ttu-id="e11e6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e11e6-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e11e6-120">id</span><span class="sxs-lookup"><span data-stu-id="e11e6-120">id</span></span>|<span data-ttu-id="e11e6-121">Int32</span><span class="sxs-lookup"><span data-stu-id="e11e6-121">Int32</span></span>|<span data-ttu-id="e11e6-122">Índice de uma entidade que está sendo mencionada no **chatMessage especificado.**</span><span class="sxs-lookup"><span data-stu-id="e11e6-122">Index of an entity being mentioned in the specified **chatMessage**.</span></span> <span data-ttu-id="e11e6-123">Corresponde ao valor {index} na `<at id="{index}">` marca correspondente no corpo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="e11e6-123">Matches the {index} value in the corresponding `<at id="{index}">` tag in the message body.</span></span>|
|<span data-ttu-id="e11e6-124">mentionText</span><span class="sxs-lookup"><span data-stu-id="e11e6-124">mentionText</span></span>|<span data-ttu-id="e11e6-125">string</span><span class="sxs-lookup"><span data-stu-id="e11e6-125">string</span></span>|<span data-ttu-id="e11e6-126">Cadeia de caracteres usada para representar a menção.</span><span class="sxs-lookup"><span data-stu-id="e11e6-126">String used to represent the mention.</span></span> <span data-ttu-id="e11e6-127">Por exemplo, o nome de exibição de um usuário, um nome de equipe.</span><span class="sxs-lookup"><span data-stu-id="e11e6-127">For example, a user's display name, a team name.</span></span>|
|<span data-ttu-id="e11e6-128">mencionado</span><span class="sxs-lookup"><span data-stu-id="e11e6-128">mentioned</span></span>|[<span data-ttu-id="e11e6-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="e11e6-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="e11e6-130">A entidade (usuário, aplicativo, equipe ou canal) mencionada.</span><span class="sxs-lookup"><span data-stu-id="e11e6-130">The entity (user, application, team, or channel) that was mentioned.</span></span>  <span data-ttu-id="e11e6-131">Se foi um canal ou uma equipe que foi @mentioned, o identitySet contém uma propriedade de conversa que dá **a** ID da equipe/canal e uma propriedade **conversationIdentityType** que representa a equipe ou o canal.</span><span class="sxs-lookup"><span data-stu-id="e11e6-131">If it was a channel or team that was @mentioned, the identitySet contains a **conversation** property giving the ID of the team/channel, and a **conversationIdentityType** property that represents either the team or channel.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e11e6-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e11e6-132">JSON representation</span></span>

<span data-ttu-id="e11e6-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e11e6-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
