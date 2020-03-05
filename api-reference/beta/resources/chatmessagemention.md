---
title: tipo de recurso chatMessageMention
description: 'Representa uma menção em uma entidade chat. A menção pode ser a um usuário, uma equipe, um bot ou um canal. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 70dd4a277caa005883d205f353bbcfbf63428bcf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507695"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="20fe1-104">tipo de recurso chatMessageMention</span><span class="sxs-lookup"><span data-stu-id="20fe1-104">chatMessageMention resource type</span></span>

<span data-ttu-id="20fe1-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="20fe1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20fe1-106">Representa uma menção em uma entidade [chat](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="20fe1-106">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="20fe1-107">A menção pode ser a um [usuário](user.md), uma [equipe](team.md), um bot ou um [canal](channel.md).</span><span class="sxs-lookup"><span data-stu-id="20fe1-107">The mention can be to a [user](user.md), [team](team.md), bot, or [channel](channel.md).</span></span> 

<span data-ttu-id="20fe1-108">Em um objeto **chat** que contém uma ou mais menciona, a propriedade de **conteúdo** do corpo da mensagem representa a mensagem de chat em HTML.</span><span class="sxs-lookup"><span data-stu-id="20fe1-108">In a **chatMessage** object that contains one or more mentions, the message body **content** property represents the chat message in HTML.</span></span> <span data-ttu-id="20fe1-109">Ele inclui o **mentionText** de cada menção em um elemento HTML `at` , com um `id` atributo que corresponde à propriedade **ID** da menção.</span><span class="sxs-lookup"><span data-stu-id="20fe1-109">It encloses the **mentionText** of each mention in an HTML `at` element, with an `id` attribute that corresponds to the **id** property of the mention.</span></span>

<span data-ttu-id="20fe1-110">Por exemplo, uma mensagem de chat contém duas menção, com o texto de menção "Megan" e "Alex", respectivamente.</span><span class="sxs-lookup"><span data-stu-id="20fe1-110">As an example, a chat message contains two mentions, with the mention text "Megan" and "Alex" respectively.</span></span> <span data-ttu-id="20fe1-111">A propriedade de **conteúdo** do `at` corpo especifica os elementos das duas mencionas da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="20fe1-111">Its body **content** property specifies `at` elements for the two mentions as follows:</span></span>

``` json
"body": {
    "contentType": "html",
    "content": "<div><div>Ah, <at id=\"0\">Megan</at>, <at id=\"1\">Alex</at>, I saw them in a separate folder. Thanks!</div>\n</div>"
}
```

<span data-ttu-id="20fe1-112">Na propriedade **Content** , a primeira menção tem um atributo HTML `id` de 0.</span><span class="sxs-lookup"><span data-stu-id="20fe1-112">In the **content** property, the first mention has an HTML `id` attribute of 0.</span></span> <span data-ttu-id="20fe1-113">Isso corresponde à propriedade **ID** dessa primeira instância de **chatMessageMention**, que também é 0.</span><span class="sxs-lookup"><span data-stu-id="20fe1-113">This corresponds to the **id** property of that first instance of **chatMessageMention**, which is also 0.</span></span>

<span data-ttu-id="20fe1-114">A segunda menção tem um `id` atributo de 1, correspondendo à propriedade **ID** da segunda instância, que é 1.</span><span class="sxs-lookup"><span data-stu-id="20fe1-114">The second mention has an `id` attribute of 1, matching the **id** property of the second instance, which is 1.</span></span>

<span data-ttu-id="20fe1-115">Para obter um contexto mais completo do exemplo, consulte [listar respostas de mensagens de canal](../api/channel-list-messagereplies.md#example).</span><span class="sxs-lookup"><span data-stu-id="20fe1-115">For a fuller context of the example, see [List channel message replies](../api/channel-list-messagereplies.md#example).</span></span>

## <a name="properties"></a><span data-ttu-id="20fe1-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20fe1-116">Properties</span></span>
| <span data-ttu-id="20fe1-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20fe1-117">Property</span></span>     | <span data-ttu-id="20fe1-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="20fe1-118">Type</span></span>   |<span data-ttu-id="20fe1-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="20fe1-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20fe1-120">id</span><span class="sxs-lookup"><span data-stu-id="20fe1-120">id</span></span>|<span data-ttu-id="20fe1-121">Int32</span><span class="sxs-lookup"><span data-stu-id="20fe1-121">Int32</span></span>|<span data-ttu-id="20fe1-122">Índice de uma entidade que está sendo mencionada no **chat**especificado.</span><span class="sxs-lookup"><span data-stu-id="20fe1-122">Index of an entity being mentioned in the specified **chatMessage**.</span></span> <span data-ttu-id="20fe1-123">Corresponde ao valor {index} na marca correspondente `<at id="{index}">` no corpo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="20fe1-123">Matches the {index} value in the corresponding `<at id="{index}">` tag in the message body.</span></span>|
|<span data-ttu-id="20fe1-124">mentionText</span><span class="sxs-lookup"><span data-stu-id="20fe1-124">mentionText</span></span>|<span data-ttu-id="20fe1-125">string</span><span class="sxs-lookup"><span data-stu-id="20fe1-125">string</span></span>|<span data-ttu-id="20fe1-126">Cadeia de caracteres usada para representar a menção.</span><span class="sxs-lookup"><span data-stu-id="20fe1-126">String used to represent the mention.</span></span> <span data-ttu-id="20fe1-127">Por exemplo, o nome de exibição de um usuário, o nome de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="20fe1-127">For example, a user's display name, a team name.</span></span>|
|<span data-ttu-id="20fe1-128">foi</span><span class="sxs-lookup"><span data-stu-id="20fe1-128">mentioned</span></span>|[<span data-ttu-id="20fe1-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="20fe1-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="20fe1-130">A entidade (usuário, aplicativo, equipe ou canal) que foi mencionada.</span><span class="sxs-lookup"><span data-stu-id="20fe1-130">The entity (user, application, team, or channel) that was mentioned.</span></span>  <span data-ttu-id="20fe1-131">Se fosse um canal ou uma equipe que foi @mentioned, o identityset contém uma propriedade de **conversa** que concede a ID da equipe/canal, e uma propriedade **conversationIdentityType** que representa a equipe ou o canal.</span><span class="sxs-lookup"><span data-stu-id="20fe1-131">If it was a channel or team that was @mentioned, the identitySet contains a **conversation** property giving the ID of the team/channel, and a **conversationIdentityType** property that represents either the team or channel.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="20fe1-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20fe1-132">JSON representation</span></span>

<span data-ttu-id="20fe1-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="20fe1-133">The following is a JSON representation of the resource.</span></span>

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
