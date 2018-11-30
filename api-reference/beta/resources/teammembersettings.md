---
title: tipo de recurso de teamMemberSettings
description: Configurações para configurar se os membros podem realizar determinadas ações, por exemplo, criam canais e adicionar bots, na equipe de.
ms.openlocfilehash: fa673e050ab3362ae7b132f30cfc4caf16d96dcc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033556"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="6f790-103">tipo de recurso de teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="6f790-103">teamMemberSettings resource type</span></span>

> <span data-ttu-id="6f790-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6f790-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f790-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6f790-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6f790-106">Configurações para configurar se os membros podem realizar determinadas ações, por exemplo, criam canais e adicionar bots, em que a [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="6f790-106">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6f790-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6f790-107">Properties</span></span>
| <span data-ttu-id="6f790-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f790-108">Property</span></span>     | <span data-ttu-id="6f790-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f790-109">Type</span></span>   |<span data-ttu-id="6f790-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f790-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f790-111">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="6f790-111">allowCreateUpdateChannels</span></span>|<span data-ttu-id="6f790-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="6f790-112">Boolean</span></span>|<span data-ttu-id="6f790-113">Se definido como true, membros pode adicionar e atualizar os canais.</span><span class="sxs-lookup"><span data-stu-id="6f790-113">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="6f790-114">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="6f790-114">allowDeleteChannels</span></span>|<span data-ttu-id="6f790-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="6f790-115">Boolean</span></span>|<span data-ttu-id="6f790-116">Se definido como true, membros pode excluir canais.</span><span class="sxs-lookup"><span data-stu-id="6f790-116">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="6f790-117">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="6f790-117">allowAddRemoveApps</span></span>|<span data-ttu-id="6f790-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="6f790-118">Boolean</span></span>|<span data-ttu-id="6f790-119">Se definido como true, membros pode adicionar e remover aplicativos.</span><span class="sxs-lookup"><span data-stu-id="6f790-119">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="6f790-120">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="6f790-120">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="6f790-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="6f790-121">Boolean</span></span>|<span data-ttu-id="6f790-122">Se definido como true, membros pode adicionar, atualizar e remover guias.</span><span class="sxs-lookup"><span data-stu-id="6f790-122">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="6f790-123">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="6f790-123">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="6f790-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="6f790-124">Boolean</span></span>|<span data-ttu-id="6f790-125">Se definido como true, membros pode adicionar, atualizar e remover conectores.</span><span class="sxs-lookup"><span data-stu-id="6f790-125">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6f790-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6f790-126">JSON representation</span></span>

<span data-ttu-id="6f790-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6f790-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
