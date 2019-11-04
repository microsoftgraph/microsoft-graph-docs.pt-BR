---
title: tipo de recurso visualproperties
description: 'Representa o conteúdo visual, como título e corpo, de uma notificação Visual direcionada para um usuário.  '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: f03563549cc1b2f42a274032dab7b310511c70c7
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939177"
---
# <a name="visualproperties-resource-type"></a><span data-ttu-id="4634b-103">tipo de recurso visualproperties</span><span class="sxs-lookup"><span data-stu-id="4634b-103">visualProperties resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4634b-104">Representa o conteúdo visual, como título e corpo, de uma notificação Visual direcionada para um usuário.</span><span class="sxs-lookup"><span data-stu-id="4634b-104">Represents the visual content, namely title and body, of a visual notification targeted to a user.</span></span> 

## <a name="properties"></a><span data-ttu-id="4634b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4634b-105">Properties</span></span>

| <span data-ttu-id="4634b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4634b-106">Property</span></span>     | <span data-ttu-id="4634b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="4634b-107">Type</span></span>        | <span data-ttu-id="4634b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4634b-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4634b-109">title</span><span class="sxs-lookup"><span data-stu-id="4634b-109">title</span></span>|<span data-ttu-id="4634b-110">String</span><span class="sxs-lookup"><span data-stu-id="4634b-110">String</span></span>|<span data-ttu-id="4634b-111">O título de uma notificação de usuário visual.</span><span class="sxs-lookup"><span data-stu-id="4634b-111">The title of a visual user notification.</span></span> <span data-ttu-id="4634b-112">Este campo é obrigatório para cargas de notificação visuais.</span><span class="sxs-lookup"><span data-stu-id="4634b-112">This field is required for visual notification payloads.</span></span> |
|<span data-ttu-id="4634b-113">corpo</span><span class="sxs-lookup"><span data-stu-id="4634b-113">body</span></span>|<span data-ttu-id="4634b-114">String</span><span class="sxs-lookup"><span data-stu-id="4634b-114">String</span></span>|<span data-ttu-id="4634b-115">O corpo de uma notificação de usuário visual.</span><span class="sxs-lookup"><span data-stu-id="4634b-115">The body of a visual user notification.</span></span> <span data-ttu-id="4634b-116">O corpo é opcional.</span><span class="sxs-lookup"><span data-stu-id="4634b-116">Body is optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="4634b-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4634b-117">JSON representation</span></span>

<span data-ttu-id="4634b-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4634b-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.visualProperties",
  "baseType": null
}-->

```json
{
  "title": "String",
  "body": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "visualProperties resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->