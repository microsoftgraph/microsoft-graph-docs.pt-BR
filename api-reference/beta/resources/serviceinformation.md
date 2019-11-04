---
title: tipo de recurso do minhas informações
description: tipo de recurso do minhas informações
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ba13967a2b4373c1a3599baf2fcc856967fbb00c
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939828"
---
# <a name="serviceinformation-resource-type"></a><span data-ttu-id="3816c-103">tipo de recurso do minhas informações</span><span class="sxs-lookup"><span data-stu-id="3816c-103">serviceInformation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3816c-104">Representa dados descritivos básicos sobre os serviços de nuvem que um usuário optou por consultar de sua conta.</span><span class="sxs-lookup"><span data-stu-id="3816c-104">Represents basic descriptive data about cloud services that a user has chosen to refer to from their account.</span></span>

## <a name="properties"></a><span data-ttu-id="3816c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3816c-105">Properties</span></span>

| <span data-ttu-id="3816c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3816c-106">Property</span></span>     | <span data-ttu-id="3816c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3816c-107">Type</span></span>        | <span data-ttu-id="3816c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3816c-108">Description</span></span>                                            |
|:-------------|:------------|:-------------------------------------------------------|
|<span data-ttu-id="3816c-109">name</span><span class="sxs-lookup"><span data-stu-id="3816c-109">name</span></span>          | <span data-ttu-id="3816c-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3816c-110">String</span></span>      | <span data-ttu-id="3816c-111">O nome do serviço de nuvem (por exemplo, Twitter, Instagram).</span><span class="sxs-lookup"><span data-stu-id="3816c-111">The name of the cloud service (for example, Twitter, Instagram).</span></span> |
|<span data-ttu-id="3816c-112">webUrl</span><span class="sxs-lookup"><span data-stu-id="3816c-112">webUrl</span></span>        | <span data-ttu-id="3816c-113">String</span><span class="sxs-lookup"><span data-stu-id="3816c-113">String</span></span>      | <span data-ttu-id="3816c-114">Contém a URL para o serviço que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="3816c-114">Contains the URL for the service being referenced.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="3816c-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3816c-115">JSON representation</span></span>

<span data-ttu-id="3816c-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3816c-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.serviceInformation",
  "baseType": null
}-->

```json
{
  "name": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "serviceInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
