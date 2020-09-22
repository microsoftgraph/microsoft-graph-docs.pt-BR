---
title: tipo de recurso de configuração
description: Especifica IDs de aplicativo adicionais que têm permissão para gerenciar o externalConnection e indexar o conteúdo em um externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: bd267c77a9904564e8b2b7f592f207204d9396b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994215"
---
# <a name="configuration-resource-type"></a><span data-ttu-id="fc867-103">tipo de recurso de configuração</span><span class="sxs-lookup"><span data-stu-id="fc867-103">configuration resource type</span></span>

<span data-ttu-id="fc867-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc867-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc867-105">Especifica IDs de aplicativo adicionais que têm permissão para gerenciar o externalConnection e indexar o conteúdo em um [externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="fc867-105">Specifies additional application IDs that are allowed to manage the externalConnection and to index content in a [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="fc867-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc867-106">Properties</span></span>

| <span data-ttu-id="fc867-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc867-107">Property</span></span>       | <span data-ttu-id="fc867-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc867-108">Type</span></span>              | <span data-ttu-id="fc867-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc867-109">Description</span></span> |
|:---------------|:------------------|:------------|
| <span data-ttu-id="fc867-110">authorizedApps</span><span class="sxs-lookup"><span data-stu-id="fc867-110">authorizedApps</span></span> | <span data-ttu-id="fc867-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="fc867-111">String collection</span></span> | <span data-ttu-id="fc867-112">Uma coleção de IDs de aplicativo para aplicativos registrados do Active Directory do Azure que têm permissão para gerenciar o externalConnection e indexar o conteúdo no externalConnection.</span><span class="sxs-lookup"><span data-stu-id="fc867-112">A collection of application IDs for registered Azure Active Directory apps that are allowed to manage the externalConnection and to index content in the externalConnection.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fc867-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc867-113">JSON representation</span></span>

<span data-ttu-id="fc867-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc867-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.configuration",
  "baseType": null
}-->

```json
{
  "authorizedApps": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "configuration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


