---
title: tipo de recurso de participantInfo
description: Contém propriedades adicionais sobre a identidade dos participantes
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 94bbc587f26f8b5122571899eb235d9c1fc27e90
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870661"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="5a8a8-103">tipo de recurso de participantInfo</span><span class="sxs-lookup"><span data-stu-id="5a8a8-103">participantInfo resource type</span></span>

> <span data-ttu-id="5a8a8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5a8a8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a8a8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5a8a8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a8a8-106">Contém propriedades adicionais sobre a identidade dos participantes</span><span class="sxs-lookup"><span data-stu-id="5a8a8-106">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="5a8a8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a8a8-107">Properties</span></span>

| <span data-ttu-id="5a8a8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a8a8-108">Property</span></span>       | <span data-ttu-id="5a8a8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a8a8-109">Type</span></span>                          | <span data-ttu-id="5a8a8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a8a8-110">Description</span></span>  |
|:---------------|:------------------------------|:-------------|
| <span data-ttu-id="5a8a8-111">identidade</span><span class="sxs-lookup"><span data-stu-id="5a8a8-111">identity</span></span>       | [<span data-ttu-id="5a8a8-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="5a8a8-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="5a8a8-113">O [identitySet](identityset.md) associado a esse participante.</span><span class="sxs-lookup"><span data-stu-id="5a8a8-113">The [identitySet](identityset.md) associated with this participant.</span></span> |
| <span data-ttu-id="5a8a8-114">languageId</span><span class="sxs-lookup"><span data-stu-id="5a8a8-114">languageId</span></span>     | <span data-ttu-id="5a8a8-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a8a8-115">String</span></span>                        | <span data-ttu-id="5a8a8-116">A cadeia de caracteres de cultura do idioma.</span><span class="sxs-lookup"><span data-stu-id="5a8a8-116">The language culture string.</span></span> |
| <span data-ttu-id="5a8a8-117">região</span><span class="sxs-lookup"><span data-stu-id="5a8a8-117">region</span></span>         | <span data-ttu-id="5a8a8-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a8a8-118">String</span></span>                        | <span data-ttu-id="5a8a8-119">Região do participante.</span><span class="sxs-lookup"><span data-stu-id="5a8a8-119">Region of the participant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5a8a8-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a8a8-120">JSON representation</span></span>

<span data-ttu-id="5a8a8-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5a8a8-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "languageId", "region"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
  "languageId": "String",
  "region": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
