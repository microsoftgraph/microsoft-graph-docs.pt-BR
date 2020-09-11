---
title: tipo de recurso teamsTabConfiguration (tipo aberto)
description: As configurações que determinam o conteúdo de uma guia.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 154d94811766f55aeb2bf066d22fc76775e99405
ms.sourcegitcommit: c7c198f6fa252b68e91be341b93b818afd387486
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2020
ms.locfileid: "47439875"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="7f0bc-103">tipo de recurso teamsTabConfiguration (tipo aberto)</span><span class="sxs-lookup"><span data-stu-id="7f0bc-103">teamsTabConfiguration resource type (Open Type)</span></span>

<span data-ttu-id="7f0bc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f0bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f0bc-105">As configurações que determinam o conteúdo de uma [guia](teamstab.md). Quando uma guia é configurada de forma interativa, essa informação é definida pelo aplicativo de provedor de guias.</span><span class="sxs-lookup"><span data-stu-id="7f0bc-105">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="7f0bc-106">Além das propriedades abaixo, alguns aplicativos de provedor de guia especificam Propriedades personalizadas adicionais.</span><span class="sxs-lookup"><span data-stu-id="7f0bc-106">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="7f0bc-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f0bc-107">Properties</span></span>

|<span data-ttu-id="7f0bc-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f0bc-108">Property</span></span>|<span data-ttu-id="7f0bc-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f0bc-109">Type</span></span>|<span data-ttu-id="7f0bc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f0bc-110">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="7f0bc-111">entityId</span><span class="sxs-lookup"><span data-stu-id="7f0bc-111">entityId</span></span>   |   <span data-ttu-id="7f0bc-112">string</span><span class="sxs-lookup"><span data-stu-id="7f0bc-112">string</span></span> |  <span data-ttu-id="7f0bc-113">Identificador da entidade hospedada pelo provedor de guias.</span><span class="sxs-lookup"><span data-stu-id="7f0bc-113">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="7f0bc-114">contentUrl</span><span class="sxs-lookup"><span data-stu-id="7f0bc-114">contentUrl</span></span> |   <span data-ttu-id="7f0bc-115">string</span><span class="sxs-lookup"><span data-stu-id="7f0bc-115">string</span></span> |  <span data-ttu-id="7f0bc-116">URL usada para renderizar o conteúdo da guia no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7f0bc-116">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="7f0bc-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f0bc-117">Required.</span></span>    |
|  <span data-ttu-id="7f0bc-118">removeUrl</span><span class="sxs-lookup"><span data-stu-id="7f0bc-118">removeUrl</span></span>  |   <span data-ttu-id="7f0bc-119">string</span><span class="sxs-lookup"><span data-stu-id="7f0bc-119">string</span></span> |  <span data-ttu-id="7f0bc-120">URL chamada pelo cliente Teams quando uma guia é removida usando o cliente Teams.</span><span class="sxs-lookup"><span data-stu-id="7f0bc-120">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="7f0bc-121">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="7f0bc-121">websiteUrl</span></span> |   <span data-ttu-id="7f0bc-122">string</span><span class="sxs-lookup"><span data-stu-id="7f0bc-122">string</span></span> |  <span data-ttu-id="7f0bc-123">URL para mostrar o conteúdo de guia fora do teams.</span><span class="sxs-lookup"><span data-stu-id="7f0bc-123">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="7f0bc-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f0bc-124">JSON representation</span></span>

<span data-ttu-id="7f0bc-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7f0bc-125">The following is a JSON representation of the resource.</span></span>
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
