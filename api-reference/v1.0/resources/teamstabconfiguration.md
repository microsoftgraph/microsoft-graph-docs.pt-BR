---
title: tipo de recurso de teamsTabConfiguration (Open tipo)
description: As configurações que determinam o conteúdo de uma guia.
author: nkramer
ms.openlocfilehash: 281d27dfec1efa83859fad262e1b25fd06b5f4cc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344958"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="e2b80-103">tipo de recurso de teamsTabConfiguration (Open tipo)</span><span class="sxs-lookup"><span data-stu-id="e2b80-103">teamsTabConfiguration resource type (Open Type)</span></span>



<span data-ttu-id="e2b80-104">As configurações que determinam o conteúdo de uma [guia](teamstab.md). Quando uma guia interativamente estiver configurada, essas informações são definidas pelo aplicativo do provedor de guia.</span><span class="sxs-lookup"><span data-stu-id="e2b80-104">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="e2b80-105">Além das propriedades abaixo, alguns aplicativos de provedor de guia especificam propriedades personalizadas adicionais.</span><span class="sxs-lookup"><span data-stu-id="e2b80-105">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="e2b80-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2b80-106">Properties</span></span>

|<span data-ttu-id="e2b80-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2b80-107">Property</span></span>|<span data-ttu-id="e2b80-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2b80-108">Type</span></span>|<span data-ttu-id="e2b80-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2b80-109">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="e2b80-110">entityId</span><span class="sxs-lookup"><span data-stu-id="e2b80-110">entityId</span></span>   |   <span data-ttu-id="e2b80-111">string</span><span class="sxs-lookup"><span data-stu-id="e2b80-111">string</span></span> |  <span data-ttu-id="e2b80-112">Identificador da entidade hospedados pelo provedor de guia.</span><span class="sxs-lookup"><span data-stu-id="e2b80-112">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="e2b80-113">contentUrl</span><span class="sxs-lookup"><span data-stu-id="e2b80-113">contentUrl</span></span> |   <span data-ttu-id="e2b80-114">string</span><span class="sxs-lookup"><span data-stu-id="e2b80-114">string</span></span> |  <span data-ttu-id="e2b80-115">URL usada para processar o conteúdo da guia em equipes.</span><span class="sxs-lookup"><span data-stu-id="e2b80-115">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="e2b80-116">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2b80-116">Required.</span></span>    |
|  <span data-ttu-id="e2b80-117">removeUrl</span><span class="sxs-lookup"><span data-stu-id="e2b80-117">removeUrl</span></span>  |   <span data-ttu-id="e2b80-118">string</span><span class="sxs-lookup"><span data-stu-id="e2b80-118">string</span></span> |  <span data-ttu-id="e2b80-119">Chamado pelo cliente de equipes, quando uma guia é removida usando o cliente de equipes de URL.</span><span class="sxs-lookup"><span data-stu-id="e2b80-119">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="e2b80-120">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="e2b80-120">websiteUrl</span></span> |   <span data-ttu-id="e2b80-121">string</span><span class="sxs-lookup"><span data-stu-id="e2b80-121">string</span></span> |  <span data-ttu-id="e2b80-122">URL para a exibição de conteúdo da guia fora equipes.</span><span class="sxs-lookup"><span data-stu-id="e2b80-122">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="e2b80-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2b80-123">JSON representation</span></span>

<span data-ttu-id="e2b80-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e2b80-124">The following is a JSON representation of the resource.</span></span>
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
