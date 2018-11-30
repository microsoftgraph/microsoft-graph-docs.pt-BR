---
title: tipo de recurso de teamGuestSettings
description: Configurações para configurar se os convidados podem criar, atualizar ou excluir canais na equipe de.
ms.openlocfilehash: 744e19165121d101a720a86bec0242fc31137768
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036813"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="42006-103">tipo de recurso de teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="42006-103">teamGuestSettings resource type</span></span>

> <span data-ttu-id="42006-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="42006-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42006-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="42006-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="42006-106">Configurações para configurar se os convidados podem criar, atualizar ou excluir canais em que a [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="42006-106">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="42006-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="42006-107">Properties</span></span>
| <span data-ttu-id="42006-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42006-108">Property</span></span>     | <span data-ttu-id="42006-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="42006-109">Type</span></span>   |<span data-ttu-id="42006-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="42006-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42006-111">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="42006-111">allowCreateUpdateChannels</span></span>|<span data-ttu-id="42006-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="42006-112">Boolean</span></span>|<span data-ttu-id="42006-113">Se definido como true, convidados pode adicionar e atualizar os canais.</span><span class="sxs-lookup"><span data-stu-id="42006-113">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="42006-114">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="42006-114">allowDeleteChannels</span></span>|<span data-ttu-id="42006-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="42006-115">Boolean</span></span>|<span data-ttu-id="42006-116">Se definido como true, convidados pode excluir canais.</span><span class="sxs-lookup"><span data-stu-id="42006-116">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42006-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="42006-117">JSON representation</span></span>

<span data-ttu-id="42006-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="42006-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamGuestSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
