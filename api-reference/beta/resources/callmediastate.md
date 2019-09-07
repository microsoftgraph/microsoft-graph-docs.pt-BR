---
title: tipo de recurso callMediaState
description: Representa o estado de mídia de uma chamada.
author: VinodRavichandran
ms.prod: microsoft-teams
localization_priority: Normal
doc_type: resourcePageType
ms.openlocfilehash: 6b092598c50663ec9e7803a13332798d05fe095b
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36793015"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="00e73-103">tipo de recurso audioConferencing</span><span class="sxs-lookup"><span data-stu-id="00e73-103">audioConferencing resource type</span></span>

> <span data-ttu-id="00e73-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="00e73-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00e73-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="00e73-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="00e73-106">Representa o estado de mídia de uma [chamada](call.md)de chamada.</span><span class="sxs-lookup"><span data-stu-id="00e73-106">Represents the media state for a call [call](call.md).</span></span>

## <a name="properties"></a><span data-ttu-id="00e73-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="00e73-107">Properties</span></span>

| <span data-ttu-id="00e73-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00e73-108">Property</span></span>            | <span data-ttu-id="00e73-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="00e73-109">Type</span></span>    | <span data-ttu-id="00e73-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="00e73-110">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="00e73-111">audio</span><span class="sxs-lookup"><span data-stu-id="00e73-111">audio</span></span>           | <span data-ttu-id="00e73-112">String</span><span class="sxs-lookup"><span data-stu-id="00e73-112">String</span></span>  | <span data-ttu-id="00e73-113">O estado da mídia de áudio.</span><span class="sxs-lookup"><span data-stu-id="00e73-113">The audio media state.</span></span> <span data-ttu-id="00e73-114">Os valores possíveis são: `active` e `inactive`.</span><span class="sxs-lookup"><span data-stu-id="00e73-114">Possible values are: `active`, `inactive`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="00e73-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="00e73-115">JSON representation</span></span>

<span data-ttu-id="00e73-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="00e73-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callMediaState"
}-->
```json
{
  "audio": "active | inactive",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callMediaState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
