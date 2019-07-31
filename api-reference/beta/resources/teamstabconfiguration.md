---
title: tipo de recurso teamsTabConfiguration (tipo aberto)
description: As configurações que determinam o conteúdo de uma guia.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c53fdc0b21a00c5eae43b8c170a1512e55d496b0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964423"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="597a0-103">tipo de recurso teamsTabConfiguration (tipo aberto)</span><span class="sxs-lookup"><span data-stu-id="597a0-103">teamsTabConfiguration resource type (Open Type)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="597a0-104">As configurações que determinam o conteúdo de uma [guia](teamstab.md). Quando uma guia é configurada de forma interativa, essa informação é definida pelo aplicativo de provedor de guias.</span><span class="sxs-lookup"><span data-stu-id="597a0-104">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="597a0-105">Além das propriedades abaixo, alguns aplicativos de provedor de guia especificam Propriedades personalizadas adicionais.</span><span class="sxs-lookup"><span data-stu-id="597a0-105">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="597a0-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="597a0-106">Properties</span></span>

|<span data-ttu-id="597a0-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="597a0-107">Property</span></span>|<span data-ttu-id="597a0-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="597a0-108">Type</span></span>|<span data-ttu-id="597a0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="597a0-109">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="597a0-110">entityId</span><span class="sxs-lookup"><span data-stu-id="597a0-110">entityId</span></span>   |   <span data-ttu-id="597a0-111">string</span><span class="sxs-lookup"><span data-stu-id="597a0-111">string</span></span> |  <span data-ttu-id="597a0-112">Identificador da entidade hospedada pelo provedor de guias.</span><span class="sxs-lookup"><span data-stu-id="597a0-112">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="597a0-113">contentUrl</span><span class="sxs-lookup"><span data-stu-id="597a0-113">contentUrl</span></span> |   <span data-ttu-id="597a0-114">string</span><span class="sxs-lookup"><span data-stu-id="597a0-114">string</span></span> |  <span data-ttu-id="597a0-115">URL usada para renderizar o conteúdo da guia no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="597a0-115">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="597a0-116">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="597a0-116">Required.</span></span>    |
|  <span data-ttu-id="597a0-117">removeUrl</span><span class="sxs-lookup"><span data-stu-id="597a0-117">removeUrl</span></span>  |   <span data-ttu-id="597a0-118">string</span><span class="sxs-lookup"><span data-stu-id="597a0-118">string</span></span> |  <span data-ttu-id="597a0-119">URL chamada pelo cliente Teams quando uma guia é removida usando o cliente Teams.</span><span class="sxs-lookup"><span data-stu-id="597a0-119">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="597a0-120">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="597a0-120">websiteUrl</span></span> |   <span data-ttu-id="597a0-121">string</span><span class="sxs-lookup"><span data-stu-id="597a0-121">string</span></span> |  <span data-ttu-id="597a0-122">URL para mostrar o conteúdo de guia fora do teams.</span><span class="sxs-lookup"><span data-stu-id="597a0-122">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="597a0-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="597a0-123">JSON representation</span></span>

<span data-ttu-id="597a0-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="597a0-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTabConfiguration"
}-->

```json
{
   "entityId": "string",
   "contentUrl": "string (HTTPS Url)",
   "websiteUrl": "string (HTTPS Url)",
   "removeUrl": "string (HTTPS Url)"  
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
