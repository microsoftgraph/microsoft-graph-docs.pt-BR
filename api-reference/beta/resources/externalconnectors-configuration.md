---
title: tipo de recurso de configuração
description: Especifica IDs de aplicativo adicionais que podem gerenciar o externalConnection e indexar conteúdo em um externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 05fbf022c11cf318281831d1b4e8572646875a06
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467572"
---
# <a name="configuration-resource-type"></a><span data-ttu-id="6aa29-103">tipo de recurso de configuração</span><span class="sxs-lookup"><span data-stu-id="6aa29-103">configuration resource type</span></span>

<span data-ttu-id="6aa29-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="6aa29-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6aa29-105">Especifica IDs de aplicativo adicionais que podem gerenciar o externalConnection e indexar conteúdo em [um externalConnection](../resources/externalconnectors-externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="6aa29-105">Specifies additional application IDs that are allowed to manage the externalConnection and to index content in a [externalConnection](../resources/externalconnectors-externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6aa29-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6aa29-106">Properties</span></span>

| <span data-ttu-id="6aa29-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6aa29-107">Property</span></span>       | <span data-ttu-id="6aa29-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6aa29-108">Type</span></span>              | <span data-ttu-id="6aa29-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6aa29-109">Description</span></span> |
|:---------------|:------------------|:------------|
| <span data-ttu-id="6aa29-110">authorizedAppIds</span><span class="sxs-lookup"><span data-stu-id="6aa29-110">authorizedAppIds</span></span> | <span data-ttu-id="6aa29-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6aa29-111">String collection</span></span> | <span data-ttu-id="6aa29-112">Uma coleção de IDs de aplicativos para aplicativos Azure Active Directory registrados que podem gerenciar o externalConnection e indexar conteúdo no externalConnection.</span><span class="sxs-lookup"><span data-stu-id="6aa29-112">A collection of application IDs for registered Azure Active Directory apps that are allowed to manage the externalConnection and to index content in the externalConnection.</span></span> |

> [!NOTE]
> <span data-ttu-id="6aa29-113">A `authorizedAppIds` propriedade foi nomeada `authorizedApps` anteriormente .</span><span class="sxs-lookup"><span data-stu-id="6aa29-113">The `authorizedAppIds` property was previously named `authorizedApps`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6aa29-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6aa29-114">JSON representation</span></span>

<span data-ttu-id="6aa29-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6aa29-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.configuration",
  "baseType": null
}-->

```json
{
  "authorizedAppIds": ["String"]
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
