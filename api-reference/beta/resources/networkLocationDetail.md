---
title: tipo de recurso networkLocationDetail
description: Fornece o nome e o tipo de rede a partir da qual o usuário entrou.
localization_priority: Normal
author: khotz
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 210201613a2f93c99472b42c5ea3ef231a10125d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026604"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="cb3ef-103">tipo de recurso networkLocationDetail</span><span class="sxs-lookup"><span data-stu-id="cb3ef-103">networkLocationDetail resource type</span></span>

<span data-ttu-id="cb3ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb3ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb3ef-105">Fornece o nome e o tipo de rede a partir da qual o usuário entrou.</span><span class="sxs-lookup"><span data-stu-id="cb3ef-105">Provides the name and type of network from which the user signed in.</span></span>

## <a name="properties"></a><span data-ttu-id="cb3ef-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cb3ef-106">Properties</span></span>

| <span data-ttu-id="cb3ef-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb3ef-107">Property</span></span>     | <span data-ttu-id="cb3ef-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb3ef-108">Type</span></span>        | <span data-ttu-id="cb3ef-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb3ef-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cb3ef-110">networknames</span><span class="sxs-lookup"><span data-stu-id="cb3ef-110">networkNames</span></span>|<span data-ttu-id="cb3ef-111">Coleção String</span><span class="sxs-lookup"><span data-stu-id="cb3ef-111">String collection</span></span>|<span data-ttu-id="cb3ef-112">Fornece o nome da rede usada ao entrar.</span><span class="sxs-lookup"><span data-stu-id="cb3ef-112">Provides the name of the network used when signing in.</span></span>|
|<span data-ttu-id="cb3ef-113">NetworkType</span><span class="sxs-lookup"><span data-stu-id="cb3ef-113">networkType</span></span>|<span data-ttu-id="cb3ef-114">NetworkType</span><span class="sxs-lookup"><span data-stu-id="cb3ef-114">networkType</span></span>| <span data-ttu-id="cb3ef-115">Fornece o tipo de rede usada ao entrar.</span><span class="sxs-lookup"><span data-stu-id="cb3ef-115">Provides the type of network used when signing in.</span></span> <span data-ttu-id="cb3ef-116">Os valores possíveis são: `intranet`, `extranet`, `namedNetwork`, `trusted`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="cb3ef-116">Possible values are: `intranet`, `extranet`, `namedNetwork`, `trusted`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb3ef-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cb3ef-117">JSON representation</span></span>

<span data-ttu-id="cb3ef-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cb3ef-118">The following is a JSON representation of the resource.</span></span>

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

