---
title: tipo de recurso de chatMessageMention
description: 'Representa uma mencionam em uma entidade chatMessage. O mencionam pode ser usuário, equipe, bot ou canal. '
localization_priority: Normal
ms.openlocfilehash: 7b24d2af6f61f3da69480557e1c5b5f32c009c25
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876130"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="5382c-104">tipo de recurso de chatMessageMention</span><span class="sxs-lookup"><span data-stu-id="5382c-104">chatMessageMention resource type</span></span>

> <span data-ttu-id="5382c-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5382c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5382c-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5382c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5382c-107">Representa uma mencionam em uma entidade [chatMessage](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="5382c-107">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="5382c-108">O mencionam pode ser usuário, equipe, bot ou canal.</span><span class="sxs-lookup"><span data-stu-id="5382c-108">The mention can be to a user, team, bot or channel.</span></span> 

## <a name="properties"></a><span data-ttu-id="5382c-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5382c-109">Properties</span></span>
| <span data-ttu-id="5382c-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5382c-110">Property</span></span>     | <span data-ttu-id="5382c-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="5382c-111">Type</span></span>   |<span data-ttu-id="5382c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="5382c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5382c-113">id</span><span class="sxs-lookup"><span data-stu-id="5382c-113">id</span></span>|<span data-ttu-id="5382c-114">string</span><span class="sxs-lookup"><span data-stu-id="5382c-114">string</span></span>|<span data-ttu-id="5382c-115">ID da entidade que está sendo mencionada</span><span class="sxs-lookup"><span data-stu-id="5382c-115">Id of the entity being mentioned</span></span>|
|<span data-ttu-id="5382c-116">mentionText</span><span class="sxs-lookup"><span data-stu-id="5382c-116">mentionText</span></span>|<span data-ttu-id="5382c-117">string</span><span class="sxs-lookup"><span data-stu-id="5382c-117">string</span></span>|<span data-ttu-id="5382c-118">Cadeia de caracteres usada para representar o mencionam ex.: nome de exibição do usuário, o nome da equipe etc.</span><span class="sxs-lookup"><span data-stu-id="5382c-118">String used to represent the mention Ex: User display name, Team name etc</span></span>|
|<span data-ttu-id="5382c-119">mencionado</span><span class="sxs-lookup"><span data-stu-id="5382c-119">mentioned</span></span>|[<span data-ttu-id="5382c-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="5382c-120">identitySet</span></span>](identityset.md)|<span data-ttu-id="5382c-121">O usuário que tenha sido mencionado</span><span class="sxs-lookup"><span data-stu-id="5382c-121">The user that was mentioned</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5382c-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5382c-122">JSON representation</span></span>

<span data-ttu-id="5382c-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5382c-123">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
