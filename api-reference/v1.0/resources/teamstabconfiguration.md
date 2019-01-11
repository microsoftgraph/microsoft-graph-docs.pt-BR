---
title: tipo de recurso de teamsTabConfiguration (Open tipo)
description: As configurações que determinam o conteúdo de uma guia.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: c33ab6d5102498ab26fcc609328c2562707883d3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858468"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="ef0e6-103">tipo de recurso de teamsTabConfiguration (Open tipo)</span><span class="sxs-lookup"><span data-stu-id="ef0e6-103">teamsTabConfiguration resource type (Open Type)</span></span>



<span data-ttu-id="ef0e6-104">As configurações que determinam o conteúdo de uma [guia](teamstab.md). Quando uma guia interativamente estiver configurada, essas informações são definidas pelo aplicativo do provedor de guia.</span><span class="sxs-lookup"><span data-stu-id="ef0e6-104">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="ef0e6-105">Além das propriedades abaixo, alguns aplicativos de provedor de guia especificam propriedades personalizadas adicionais.</span><span class="sxs-lookup"><span data-stu-id="ef0e6-105">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="ef0e6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ef0e6-106">Properties</span></span>

|<span data-ttu-id="ef0e6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef0e6-107">Property</span></span>|<span data-ttu-id="ef0e6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef0e6-108">Type</span></span>|<span data-ttu-id="ef0e6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef0e6-109">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="ef0e6-110">entityId</span><span class="sxs-lookup"><span data-stu-id="ef0e6-110">entityId</span></span>   |   <span data-ttu-id="ef0e6-111">string</span><span class="sxs-lookup"><span data-stu-id="ef0e6-111">string</span></span> |  <span data-ttu-id="ef0e6-112">Identificador da entidade hospedados pelo provedor de guia.</span><span class="sxs-lookup"><span data-stu-id="ef0e6-112">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="ef0e6-113">contentUrl</span><span class="sxs-lookup"><span data-stu-id="ef0e6-113">contentUrl</span></span> |   <span data-ttu-id="ef0e6-114">string</span><span class="sxs-lookup"><span data-stu-id="ef0e6-114">string</span></span> |  <span data-ttu-id="ef0e6-115">URL usada para processar o conteúdo da guia em equipes.</span><span class="sxs-lookup"><span data-stu-id="ef0e6-115">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="ef0e6-116">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef0e6-116">Required.</span></span>    |
|  <span data-ttu-id="ef0e6-117">removeUrl</span><span class="sxs-lookup"><span data-stu-id="ef0e6-117">removeUrl</span></span>  |   <span data-ttu-id="ef0e6-118">string</span><span class="sxs-lookup"><span data-stu-id="ef0e6-118">string</span></span> |  <span data-ttu-id="ef0e6-119">Chamado pelo cliente de equipes, quando uma guia é removida usando o cliente de equipes de URL.</span><span class="sxs-lookup"><span data-stu-id="ef0e6-119">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="ef0e6-120">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="ef0e6-120">websiteUrl</span></span> |   <span data-ttu-id="ef0e6-121">string</span><span class="sxs-lookup"><span data-stu-id="ef0e6-121">string</span></span> |  <span data-ttu-id="ef0e6-122">URL para a exibição de conteúdo da guia fora equipes.</span><span class="sxs-lookup"><span data-stu-id="ef0e6-122">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="ef0e6-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ef0e6-123">JSON representation</span></span>

<span data-ttu-id="ef0e6-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ef0e6-124">The following is a JSON representation of the resource.</span></span>
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
