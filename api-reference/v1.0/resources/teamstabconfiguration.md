---
title: tipo de recurso teamsTabConfiguration (tipo aberto)
description: As configurações que determinam o conteúdo de uma guia.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ad6c3bcee979e10e308b307cec780c8ddc8950dd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446832"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="1cba5-103">tipo de recurso teamsTabConfiguration (tipo aberto)</span><span class="sxs-lookup"><span data-stu-id="1cba5-103">teamsTabConfiguration resource type (Open Type)</span></span>

<span data-ttu-id="1cba5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1cba5-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="1cba5-105">As configurações que determinam o conteúdo de uma [guia](teamstab.md). Quando uma guia é configurada de forma interativa, essa informação é definida pelo aplicativo de provedor de guias.</span><span class="sxs-lookup"><span data-stu-id="1cba5-105">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="1cba5-106">Além das propriedades abaixo, alguns aplicativos de provedor de guia especificam Propriedades personalizadas adicionais.</span><span class="sxs-lookup"><span data-stu-id="1cba5-106">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="1cba5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1cba5-107">Properties</span></span>

|<span data-ttu-id="1cba5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1cba5-108">Property</span></span>|<span data-ttu-id="1cba5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cba5-109">Type</span></span>|<span data-ttu-id="1cba5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cba5-110">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="1cba5-111">entityId</span><span class="sxs-lookup"><span data-stu-id="1cba5-111">entityId</span></span>   |   <span data-ttu-id="1cba5-112">string</span><span class="sxs-lookup"><span data-stu-id="1cba5-112">string</span></span> |  <span data-ttu-id="1cba5-113">Identificador da entidade hospedada pelo provedor de guias.</span><span class="sxs-lookup"><span data-stu-id="1cba5-113">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="1cba5-114">contentUrl</span><span class="sxs-lookup"><span data-stu-id="1cba5-114">contentUrl</span></span> |   <span data-ttu-id="1cba5-115">string</span><span class="sxs-lookup"><span data-stu-id="1cba5-115">string</span></span> |  <span data-ttu-id="1cba5-116">URL usada para renderizar o conteúdo da guia no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="1cba5-116">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="1cba5-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cba5-117">Required.</span></span>    |
|  <span data-ttu-id="1cba5-118">removeUrl</span><span class="sxs-lookup"><span data-stu-id="1cba5-118">removeUrl</span></span>  |   <span data-ttu-id="1cba5-119">string</span><span class="sxs-lookup"><span data-stu-id="1cba5-119">string</span></span> |  <span data-ttu-id="1cba5-120">URL chamada pelo cliente Teams quando uma guia é removida usando o cliente Teams.</span><span class="sxs-lookup"><span data-stu-id="1cba5-120">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="1cba5-121">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="1cba5-121">websiteUrl</span></span> |   <span data-ttu-id="1cba5-122">string</span><span class="sxs-lookup"><span data-stu-id="1cba5-122">string</span></span> |  <span data-ttu-id="1cba5-123">URL para mostrar o conteúdo de guia fora do teams.</span><span class="sxs-lookup"><span data-stu-id="1cba5-123">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="1cba5-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1cba5-124">JSON representation</span></span>

<span data-ttu-id="1cba5-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1cba5-125">The following is a JSON representation of the resource.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
