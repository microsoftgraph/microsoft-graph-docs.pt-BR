---
title: tipo de recurso networkLocationDetail
description: Fornece o nome e o tipo de rede a partir da qual o usuário entrou.
localization_priority: Normal
author: besiler
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7c43341ab5799da83a084e035c680a1926b3d8e8
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523011"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="7e7e1-103">tipo de recurso networkLocationDetail</span><span class="sxs-lookup"><span data-stu-id="7e7e1-103">networkLocationDetail resource type</span></span>

<span data-ttu-id="7e7e1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e7e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e7e1-105">Fornece o nome e o tipo de rede a partir da qual o usuário entrou.</span><span class="sxs-lookup"><span data-stu-id="7e7e1-105">Provides the name and type of network from which the user signed in.</span></span>

## <a name="properties"></a><span data-ttu-id="7e7e1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7e7e1-106">Properties</span></span>

| <span data-ttu-id="7e7e1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7e7e1-107">Property</span></span>     | <span data-ttu-id="7e7e1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e7e1-108">Type</span></span>        | <span data-ttu-id="7e7e1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e7e1-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7e7e1-110">networknames</span><span class="sxs-lookup"><span data-stu-id="7e7e1-110">networkNames</span></span>|<span data-ttu-id="7e7e1-111">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e7e1-111">String collection</span></span>|<span data-ttu-id="7e7e1-112">Fornece o nome da rede usada ao entrar.</span><span class="sxs-lookup"><span data-stu-id="7e7e1-112">Provides the name of the network used when signing in.</span></span>|
|<span data-ttu-id="7e7e1-113">NetworkType</span><span class="sxs-lookup"><span data-stu-id="7e7e1-113">networkType</span></span>|<span data-ttu-id="7e7e1-114">NetworkType</span><span class="sxs-lookup"><span data-stu-id="7e7e1-114">networkType</span></span>| <span data-ttu-id="7e7e1-115">Fornece o tipo de rede usada ao entrar.</span><span class="sxs-lookup"><span data-stu-id="7e7e1-115">Provides the type of network used when signing in.</span></span> <span data-ttu-id="7e7e1-116">Os valores possíveis são: `intranet`, `extranet`, `namedNetwork`, `trusted`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="7e7e1-116">Possible values are: `intranet`, `extranet`, `namedNetwork`, `trusted`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7e7e1-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7e7e1-117">JSON representation</span></span>

<span data-ttu-id="7e7e1-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7e7e1-118">The following is a JSON representation of the resource.</span></span>

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

