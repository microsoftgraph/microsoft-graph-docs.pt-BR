---
title: tipo de recurso addIn
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 1700f3c6bec06c9f2e7ec6093fccffab443d2b08
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895969"
---
# <a name="addin-resource-type"></a><span data-ttu-id="84bb7-103">tipo de recurso addIn</span><span class="sxs-lookup"><span data-stu-id="84bb7-103">addIn resource type</span></span>

<span data-ttu-id="84bb7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84bb7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84bb7-105">Define o comportamento personalizado que um serviço de consumo pode usar para chamar um aplicativo em contextos específicos.</span><span class="sxs-lookup"><span data-stu-id="84bb7-105">Defines custom behavior that a consuming service can use to call an app in specific contexts.</span></span> <span data-ttu-id="84bb7-106">Por exemplo, aplicativos que podem renderizar fluxos de arquivos [podem configurar suplementos](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online) para a funcionalidade do manipulador de arquivos.</span><span class="sxs-lookup"><span data-stu-id="84bb7-106">For example, applications that can render file streams [might configure add-ins](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online) for File Handler functionality.</span></span> <span data-ttu-id="84bb7-107">Isso permitirá que os serviços, como o Microsoft 365, chamem o aplicativo no contexto de um documento em que o usuário esteja trabalhando.</span><span class="sxs-lookup"><span data-stu-id="84bb7-107">This will let services like Microsoft 365 call the application in the context of a document the user is working on.</span></span>

## <a name="properties"></a><span data-ttu-id="84bb7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="84bb7-108">Properties</span></span>
| <span data-ttu-id="84bb7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84bb7-109">Property</span></span>     | <span data-ttu-id="84bb7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="84bb7-110">Type</span></span>   |<span data-ttu-id="84bb7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="84bb7-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84bb7-112">id</span><span class="sxs-lookup"><span data-stu-id="84bb7-112">id</span></span>|<span data-ttu-id="84bb7-113">#c0</span><span class="sxs-lookup"><span data-stu-id="84bb7-113">guid</span></span>||
|<span data-ttu-id="84bb7-114">properties</span><span class="sxs-lookup"><span data-stu-id="84bb7-114">properties</span></span>|<span data-ttu-id="84bb7-115">Coleção [KeyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="84bb7-115">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="84bb7-116">type</span><span class="sxs-lookup"><span data-stu-id="84bb7-116">type</span></span>|<span data-ttu-id="84bb7-117">string</span><span class="sxs-lookup"><span data-stu-id="84bb7-117">string</span></span>||

## <a name="json-representation"></a><span data-ttu-id="84bb7-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="84bb7-118">JSON representation</span></span>

<span data-ttu-id="84bb7-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="84bb7-119">Here is a JSON representation of the resource.</span></span>

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
