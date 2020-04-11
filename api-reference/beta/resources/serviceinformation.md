---
title: tipo de recurso do minhas informações
description: tipo de recurso do minhas informações
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: daca733578e5415fc777bc01a8ef1272cfdcc681
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228877"
---
# <a name="serviceinformation-resource-type"></a><span data-ttu-id="b958c-103">tipo de recurso do minhas informações</span><span class="sxs-lookup"><span data-stu-id="b958c-103">serviceInformation resource type</span></span>

<span data-ttu-id="b958c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b958c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b958c-105">Representa dados descritivos básicos sobre os serviços de nuvem que um usuário optou por consultar de sua conta.</span><span class="sxs-lookup"><span data-stu-id="b958c-105">Represents basic descriptive data about cloud services that a user has chosen to refer to from their account.</span></span>

## <a name="properties"></a><span data-ttu-id="b958c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b958c-106">Properties</span></span>

| <span data-ttu-id="b958c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b958c-107">Property</span></span>     | <span data-ttu-id="b958c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b958c-108">Type</span></span>        | <span data-ttu-id="b958c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b958c-109">Description</span></span>                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|<span data-ttu-id="b958c-110">nome</span><span class="sxs-lookup"><span data-stu-id="b958c-110">name</span></span>          | <span data-ttu-id="b958c-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b958c-111">String</span></span>      | <span data-ttu-id="b958c-112">O nome do serviço de nuvem (por exemplo, Twitter, Instagram).</span><span class="sxs-lookup"><span data-stu-id="b958c-112">The name of the cloud service (for example, Twitter, Instagram).</span></span> |
|<span data-ttu-id="b958c-113">webUrl</span><span class="sxs-lookup"><span data-stu-id="b958c-113">webUrl</span></span>        | <span data-ttu-id="b958c-114">String</span><span class="sxs-lookup"><span data-stu-id="b958c-114">String</span></span>      | <span data-ttu-id="b958c-115">Contém a URL para o serviço que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="b958c-115">Contains the URL for the service being referenced.</span></span>               |

## <a name="json-representation"></a><span data-ttu-id="b958c-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b958c-116">JSON representation</span></span>

<span data-ttu-id="b958c-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b958c-117">The following is a JSON representation of the resource.</span></span>

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
