---
title: tipo de recurso networkLocationDetail
description: Fornece o nome e o tipo de rede a partir da qual o usuário entrou.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8cbf60f7e7e370c5813623643f9d14cb324950cc
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939506"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="45c29-103">tipo de recurso networkLocationDetail</span><span class="sxs-lookup"><span data-stu-id="45c29-103">networkLocationDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45c29-104">Fornece o nome e o tipo de rede a partir da qual o usuário entrou.</span><span class="sxs-lookup"><span data-stu-id="45c29-104">Provides the name and type of network from which the user signed in.</span></span>

## <a name="properties"></a><span data-ttu-id="45c29-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="45c29-105">Properties</span></span>

| <span data-ttu-id="45c29-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45c29-106">Property</span></span>     | <span data-ttu-id="45c29-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="45c29-107">Type</span></span>        | <span data-ttu-id="45c29-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="45c29-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="45c29-109">networknames</span><span class="sxs-lookup"><span data-stu-id="45c29-109">networkNames</span></span>|<span data-ttu-id="45c29-110">String collection</span><span class="sxs-lookup"><span data-stu-id="45c29-110">String collection</span></span>|<span data-ttu-id="45c29-111">Fornece o nome da rede usada ao entrar.</span><span class="sxs-lookup"><span data-stu-id="45c29-111">Provides the name of the network used when signing in.</span></span>|
|<span data-ttu-id="45c29-112">NetworkType</span><span class="sxs-lookup"><span data-stu-id="45c29-112">networkType</span></span>|<span data-ttu-id="45c29-113">NetworkType</span><span class="sxs-lookup"><span data-stu-id="45c29-113">networkType</span></span>| <span data-ttu-id="45c29-114">Fornece o tipo de rede usada ao entrar.</span><span class="sxs-lookup"><span data-stu-id="45c29-114">Provides the type of network used when signing in.</span></span> <span data-ttu-id="45c29-115">Os valores possíveis são: `intranet`, `extranet`, `namedNetwork`, `trusted`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="45c29-115">Possible values are: `intranet`, `extranet`, `namedNetwork`, `trusted`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="45c29-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="45c29-116">JSON representation</span></span>

<span data-ttu-id="45c29-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="45c29-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkLocationDetail",
  "baseType": null
}-->

```json
{
  "networkNames": ["String"],
  "networkType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkLocationDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->