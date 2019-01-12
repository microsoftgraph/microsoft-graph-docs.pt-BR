---
title: tipo de recurso de mediaInfo
description: As informações de mídia usadas em ações para solicita.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 217b9a5aaa88a1bbf343447fad344b322cfeb611
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924528"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="763c6-103">tipo de recurso de mediaInfo</span><span class="sxs-lookup"><span data-stu-id="763c6-103">mediaInfo resource type</span></span>

> <span data-ttu-id="763c6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="763c6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="763c6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="763c6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="763c6-106">As informações de mídia usadas em ações para solicita.</span><span class="sxs-lookup"><span data-stu-id="763c6-106">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="763c6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="763c6-107">Properties</span></span>
| <span data-ttu-id="763c6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="763c6-108">Property</span></span>       | <span data-ttu-id="763c6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="763c6-109">Type</span></span>    | <span data-ttu-id="763c6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="763c6-110">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="763c6-111">resourceId</span><span class="sxs-lookup"><span data-stu-id="763c6-111">resourceId</span></span>     | <span data-ttu-id="763c6-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="763c6-112">String</span></span>  | <span data-ttu-id="763c6-113">Identidade exclusiva do recurso.</span><span class="sxs-lookup"><span data-stu-id="763c6-113">Unique identity of the resource.</span></span> |
| <span data-ttu-id="763c6-114">URI</span><span class="sxs-lookup"><span data-stu-id="763c6-114">uri</span></span>            | <span data-ttu-id="763c6-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="763c6-115">String</span></span>  | <span data-ttu-id="763c6-116">Caminho para o recurso.</span><span class="sxs-lookup"><span data-stu-id="763c6-116">Path to the resource.</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="763c6-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="763c6-117">JSON representation</span></span>

<span data-ttu-id="763c6-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="763c6-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaInfo"
}-->
```json
{
  "resourceId": "String",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
