---
title: tipo de recurso de mediaInfo
description: As informações de mídia usadas em ações para solicita.
author: VinodRavichandran
ms.openlocfilehash: ea2eaa9e8e85da737df4c0c0170457fb3350820b
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380272"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="266f7-103">tipo de recurso de mediaInfo</span><span class="sxs-lookup"><span data-stu-id="266f7-103">mediaInfo resource type</span></span>

> <span data-ttu-id="266f7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="266f7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="266f7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="266f7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="266f7-106">As informações de mídia usadas em ações para solicita.</span><span class="sxs-lookup"><span data-stu-id="266f7-106">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="266f7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="266f7-107">Properties</span></span>
| <span data-ttu-id="266f7-108">Propriedade	</span><span class="sxs-lookup"><span data-stu-id="266f7-108">Property</span></span>       | <span data-ttu-id="266f7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="266f7-109">Type</span></span>    | <span data-ttu-id="266f7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="266f7-110">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="266f7-111">resourceId</span><span class="sxs-lookup"><span data-stu-id="266f7-111">resourceId</span></span>     | <span data-ttu-id="266f7-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="266f7-112">String</span></span>  | <span data-ttu-id="266f7-113">Identidade exclusiva do recurso.</span><span class="sxs-lookup"><span data-stu-id="266f7-113">Unique identity of the resource.</span></span> |
| <span data-ttu-id="266f7-114">URI</span><span class="sxs-lookup"><span data-stu-id="266f7-114">uri</span></span>            | <span data-ttu-id="266f7-115">String</span><span class="sxs-lookup"><span data-stu-id="266f7-115">String</span></span>  | <span data-ttu-id="266f7-116">Caminho para o recurso.</span><span class="sxs-lookup"><span data-stu-id="266f7-116">Path to the resource.</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="266f7-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="266f7-117">JSON representation</span></span>

<span data-ttu-id="266f7-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="266f7-118">The following is a JSON representation of the resource.</span></span>

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