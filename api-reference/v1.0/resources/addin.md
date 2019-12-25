---
title: tipo de recurso addIn
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 3671ad561fde44aac90d20284c7acbfedba6b0c3
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863932"
---
# <a name="addin-resource-type"></a><span data-ttu-id="cdb05-103">tipo de recurso addIn</span><span class="sxs-lookup"><span data-stu-id="cdb05-103">addIn resource type</span></span>

<span data-ttu-id="cdb05-104">Define o comportamento personalizado que um serviço de consumo pode usar para chamar um aplicativo em contextos específicos.</span><span class="sxs-lookup"><span data-stu-id="cdb05-104">Defines custom behavior that a consuming service can use to call an app in specific contexts.</span></span> <span data-ttu-id="cdb05-105">Por exemplo, aplicativos que podem renderizar fluxos de arquivos [podem configurar AddIns](/onedrive/developer/file-handlers/?view=odsp-graph-online) para sua funcionalidade "FileHandler".</span><span class="sxs-lookup"><span data-stu-id="cdb05-105">For example, applications that can render file streams [may configure addIns](/onedrive/developer/file-handlers/?view=odsp-graph-online) for its "FileHandler" functionality.</span></span> <span data-ttu-id="cdb05-106">Isso permitirá que serviços como o Office 365 chamem o aplicativo no contexto de um documento em que o usuário esteja trabalhando.</span><span class="sxs-lookup"><span data-stu-id="cdb05-106">This will let services like Office 365 call the application in the context of a document the user is working on.</span></span>

## <a name="properties"></a><span data-ttu-id="cdb05-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cdb05-107">Properties</span></span>
| <span data-ttu-id="cdb05-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cdb05-108">Property</span></span>     | <span data-ttu-id="cdb05-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="cdb05-109">Type</span></span>   |<span data-ttu-id="cdb05-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdb05-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cdb05-111">id</span><span class="sxs-lookup"><span data-stu-id="cdb05-111">id</span></span>|<span data-ttu-id="cdb05-112">#c0</span><span class="sxs-lookup"><span data-stu-id="cdb05-112">guid</span></span>||
|<span data-ttu-id="cdb05-113">properties</span><span class="sxs-lookup"><span data-stu-id="cdb05-113">properties</span></span>|<span data-ttu-id="cdb05-114">Coleção [KeyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="cdb05-114">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="cdb05-115">type</span><span class="sxs-lookup"><span data-stu-id="cdb05-115">type</span></span>|<span data-ttu-id="cdb05-116">string</span><span class="sxs-lookup"><span data-stu-id="cdb05-116">string</span></span>||

## <a name="json-representation"></a><span data-ttu-id="cdb05-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cdb05-117">JSON representation</span></span>

<span data-ttu-id="cdb05-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cdb05-118">Here is a JSON representation of the resource.</span></span>

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
