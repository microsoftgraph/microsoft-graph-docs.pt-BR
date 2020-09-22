---
title: tipo de recurso visualproperties
description: 'Representa o conteúdo visual, como título e corpo, de uma notificação Visual direcionada para um usuário.  '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 62580847844a4b397ed117ea4b256cc4f035577a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057686"
---
# <a name="visualproperties-resource-type"></a><span data-ttu-id="5c50d-103">tipo de recurso visualproperties</span><span class="sxs-lookup"><span data-stu-id="5c50d-103">visualProperties resource type</span></span>

<span data-ttu-id="5c50d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c50d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c50d-105">Representa o conteúdo visual, como título e corpo, de uma notificação Visual direcionada para um usuário.</span><span class="sxs-lookup"><span data-stu-id="5c50d-105">Represents the visual content, namely title and body, of a visual notification targeted to a user.</span></span> 

## <a name="properties"></a><span data-ttu-id="5c50d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5c50d-106">Properties</span></span>

| <span data-ttu-id="5c50d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c50d-107">Property</span></span>     | <span data-ttu-id="5c50d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c50d-108">Type</span></span>        | <span data-ttu-id="5c50d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c50d-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5c50d-110">title</span><span class="sxs-lookup"><span data-stu-id="5c50d-110">title</span></span>|<span data-ttu-id="5c50d-111">String</span><span class="sxs-lookup"><span data-stu-id="5c50d-111">String</span></span>|<span data-ttu-id="5c50d-112">O título de uma notificação de usuário visual.</span><span class="sxs-lookup"><span data-stu-id="5c50d-112">The title of a visual user notification.</span></span> <span data-ttu-id="5c50d-113">Este campo é obrigatório para cargas de notificação visuais.</span><span class="sxs-lookup"><span data-stu-id="5c50d-113">This field is required for visual notification payloads.</span></span> |
|<span data-ttu-id="5c50d-114">body</span><span class="sxs-lookup"><span data-stu-id="5c50d-114">body</span></span>|<span data-ttu-id="5c50d-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c50d-115">String</span></span>|<span data-ttu-id="5c50d-116">O corpo de uma notificação de usuário visual.</span><span class="sxs-lookup"><span data-stu-id="5c50d-116">The body of a visual user notification.</span></span> <span data-ttu-id="5c50d-117">O corpo é opcional.</span><span class="sxs-lookup"><span data-stu-id="5c50d-117">Body is optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="5c50d-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5c50d-118">JSON representation</span></span>

<span data-ttu-id="5c50d-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5c50d-119">The following is a JSON representation of the resource.</span></span>

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

