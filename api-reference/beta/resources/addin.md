---
title: Tipo de recurso addIn
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 80c9e3c31a3bcc0d7b74e24373e5d1bb6947840f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134054"
---
# <a name="addin-resource-type"></a><span data-ttu-id="ff2d7-103">Tipo de recurso addIn</span><span class="sxs-lookup"><span data-stu-id="ff2d7-103">addIn resource type</span></span>

<span data-ttu-id="ff2d7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff2d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff2d7-105">Define o comportamento personalizado que um serviço de consumo pode usar para chamar um aplicativo em contextos específicos.</span><span class="sxs-lookup"><span data-stu-id="ff2d7-105">Defines custom behavior that a consuming service can use to call an app in specific contexts.</span></span> <span data-ttu-id="ff2d7-106">Por exemplo, aplicativos que podem renderizar fluxos de [arquivos podem configurar os complementos para](/onedrive/developer/file-handlers/?view=odsp-graph-online) a funcionalidade de Manipulador de Arquivos.</span><span class="sxs-lookup"><span data-stu-id="ff2d7-106">For example, applications that can render file streams [might configure add-ins](/onedrive/developer/file-handlers/?view=odsp-graph-online) for File Handler functionality.</span></span> <span data-ttu-id="ff2d7-107">Isso permitirá que os serviços como o Microsoft 365 chamem o aplicativo no contexto de um documento no qual o usuário esteja trabalhando.</span><span class="sxs-lookup"><span data-stu-id="ff2d7-107">This will let services like Microsoft 365 call the application in the context of a document the user is working on.</span></span>

## <a name="properties"></a><span data-ttu-id="ff2d7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff2d7-108">Properties</span></span>
| <span data-ttu-id="ff2d7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff2d7-109">Property</span></span>     | <span data-ttu-id="ff2d7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff2d7-110">Type</span></span>   |<span data-ttu-id="ff2d7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff2d7-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff2d7-112">id</span><span class="sxs-lookup"><span data-stu-id="ff2d7-112">id</span></span>|<span data-ttu-id="ff2d7-113">guid</span><span class="sxs-lookup"><span data-stu-id="ff2d7-113">guid</span></span>||
|<span data-ttu-id="ff2d7-114">properties</span><span class="sxs-lookup"><span data-stu-id="ff2d7-114">properties</span></span>|<span data-ttu-id="ff2d7-115">Coleção [KeyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="ff2d7-115">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="ff2d7-116">type</span><span class="sxs-lookup"><span data-stu-id="ff2d7-116">type</span></span>|<span data-ttu-id="ff2d7-117">string</span><span class="sxs-lookup"><span data-stu-id="ff2d7-117">string</span></span>||

## <a name="json-representation"></a><span data-ttu-id="ff2d7-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff2d7-118">JSON representation</span></span>

<span data-ttu-id="ff2d7-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff2d7-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addIn"
}-->

```json
{
  "id": "guid",
  "properties": [{"@odata.type": "microsoft.graph.keyValue"}],
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "addIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
