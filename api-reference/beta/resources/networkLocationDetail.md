---
title: Tipo de recurso networkLocationDetail
description: Fornece o nome e o tipo de rede a partir do qual o usuário se inscreveu.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 986a2f292a23bc4c67a88770dac46de59b7294e7
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130007"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="13526-103">Tipo de recurso networkLocationDetail</span><span class="sxs-lookup"><span data-stu-id="13526-103">networkLocationDetail resource type</span></span>

<span data-ttu-id="13526-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13526-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13526-105">Fornece o nome e o tipo de rede a partir do qual o usuário se inscreveu.</span><span class="sxs-lookup"><span data-stu-id="13526-105">Provides the name and type of network from which the user signed in.</span></span>

## <a name="properties"></a><span data-ttu-id="13526-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="13526-106">Properties</span></span>

| <span data-ttu-id="13526-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13526-107">Property</span></span>     | <span data-ttu-id="13526-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="13526-108">Type</span></span>        | <span data-ttu-id="13526-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="13526-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="13526-110">networkNames</span><span class="sxs-lookup"><span data-stu-id="13526-110">networkNames</span></span>|<span data-ttu-id="13526-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="13526-111">String collection</span></span>|<span data-ttu-id="13526-112">Fornece o nome da rede usada ao entrar.</span><span class="sxs-lookup"><span data-stu-id="13526-112">Provides the name of the network used when signing in.</span></span>|
|<span data-ttu-id="13526-113">networkType</span><span class="sxs-lookup"><span data-stu-id="13526-113">networkType</span></span>|<span data-ttu-id="13526-114">networkType</span><span class="sxs-lookup"><span data-stu-id="13526-114">networkType</span></span>| <span data-ttu-id="13526-115">Fornece o tipo de rede usado ao entrar.</span><span class="sxs-lookup"><span data-stu-id="13526-115">Provides the type of network used when signing in.</span></span> <span data-ttu-id="13526-116">Os valores possíveis são: `intranet`, `extranet`, `namedNetwork`, `trusted`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="13526-116">Possible values are: `intranet`, `extranet`, `namedNetwork`, `trusted`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13526-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="13526-117">JSON representation</span></span>

<span data-ttu-id="13526-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="13526-118">The following is a JSON representation of the resource.</span></span>

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

