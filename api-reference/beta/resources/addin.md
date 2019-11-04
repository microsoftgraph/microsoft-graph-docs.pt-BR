---
title: tipo de recurso addIn
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 26a224989af3ab87036fbd6bd0964ea811016dcb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939092"
---
# <a name="addin-resource-type"></a><span data-ttu-id="d5eba-103">tipo de recurso addIn</span><span class="sxs-lookup"><span data-stu-id="d5eba-103">addIn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5eba-104">Define o comportamento personalizado que um serviço de consumo pode usar para chamar um aplicativo em contextos específicos.</span><span class="sxs-lookup"><span data-stu-id="d5eba-104">Defines custom behavior that a consuming service can use to call an app in specific contexts.</span></span> <span data-ttu-id="d5eba-105">Por exemplo, aplicativos que podem renderizar fluxos de arquivos [podem configurar suplementos](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online) para a funcionalidade do manipulador de arquivos.</span><span class="sxs-lookup"><span data-stu-id="d5eba-105">For example, applications that can render file streams [might configure add-ins](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online) for File Handler functionality.</span></span> <span data-ttu-id="d5eba-106">Isso permitirá que os serviços, como o Office 365, chamem o aplicativo no contexto de um documento em que o usuário esteja trabalhando.</span><span class="sxs-lookup"><span data-stu-id="d5eba-106">This will let services like Office 365 call the application in the context of a document the user is working on.</span></span>

## <a name="properties"></a><span data-ttu-id="d5eba-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5eba-107">Properties</span></span>
| <span data-ttu-id="d5eba-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5eba-108">Property</span></span>     | <span data-ttu-id="d5eba-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5eba-109">Type</span></span>   |<span data-ttu-id="d5eba-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5eba-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5eba-111">id</span><span class="sxs-lookup"><span data-stu-id="d5eba-111">id</span></span>|<span data-ttu-id="d5eba-112">#c0</span><span class="sxs-lookup"><span data-stu-id="d5eba-112">guid</span></span>||
|<span data-ttu-id="d5eba-113">properties</span><span class="sxs-lookup"><span data-stu-id="d5eba-113">properties</span></span>|<span data-ttu-id="d5eba-114">Coleção [KeyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d5eba-114">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="d5eba-115">type</span><span class="sxs-lookup"><span data-stu-id="d5eba-115">type</span></span>|<span data-ttu-id="d5eba-116">string</span><span class="sxs-lookup"><span data-stu-id="d5eba-116">string</span></span>||

## <a name="json-representation"></a><span data-ttu-id="d5eba-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5eba-117">JSON representation</span></span>

<span data-ttu-id="d5eba-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5eba-118">Here is a JSON representation of the resource.</span></span>

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
