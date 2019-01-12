---
title: tipo de recurso de teamGuestSettings
description: Configurações para configurar se os convidados podem criar, atualizar ou excluir canais na equipe de.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: d601ac704734f4c46e8b7bef9e8d3feb45905384
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987290"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="0e4b4-103">tipo de recurso de teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="0e4b4-103">teamGuestSettings resource type</span></span>

> <span data-ttu-id="0e4b4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0e4b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e4b4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0e4b4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0e4b4-106">Configurações para configurar se os convidados podem criar, atualizar ou excluir canais em que a [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="0e4b4-106">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0e4b4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0e4b4-107">Properties</span></span>
| <span data-ttu-id="0e4b4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e4b4-108">Property</span></span>     | <span data-ttu-id="0e4b4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e4b4-109">Type</span></span>   |<span data-ttu-id="0e4b4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e4b4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e4b4-111">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="0e4b4-111">allowCreateUpdateChannels</span></span>|<span data-ttu-id="0e4b4-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="0e4b4-112">Boolean</span></span>|<span data-ttu-id="0e4b4-113">Se definido como true, convidados pode adicionar e atualizar os canais.</span><span class="sxs-lookup"><span data-stu-id="0e4b4-113">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="0e4b4-114">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="0e4b4-114">allowDeleteChannels</span></span>|<span data-ttu-id="0e4b4-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="0e4b4-115">Boolean</span></span>|<span data-ttu-id="0e4b4-116">Se definido como true, convidados pode excluir canais.</span><span class="sxs-lookup"><span data-stu-id="0e4b4-116">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0e4b4-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0e4b4-117">JSON representation</span></span>

<span data-ttu-id="0e4b4-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0e4b4-118">The following is a JSON representation of the resource.</span></span>

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
