---
title: tipo de recurso do minhas informações
description: tipo de recurso do minhas informações
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 39382b0fb17795bde26b4e54f629b2e4281f81db
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070438"
---
# <a name="serviceinformation-resource-type"></a><span data-ttu-id="372ef-103">tipo de recurso do minhas informações</span><span class="sxs-lookup"><span data-stu-id="372ef-103">serviceInformation resource type</span></span>

<span data-ttu-id="372ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="372ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="372ef-105">Representa dados descritivos básicos sobre os serviços de nuvem que um usuário optou por consultar de sua conta.</span><span class="sxs-lookup"><span data-stu-id="372ef-105">Represents basic descriptive data about cloud services that a user has chosen to refer to from their account.</span></span>

## <a name="properties"></a><span data-ttu-id="372ef-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="372ef-106">Properties</span></span>

| <span data-ttu-id="372ef-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="372ef-107">Property</span></span>     | <span data-ttu-id="372ef-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="372ef-108">Type</span></span>        | <span data-ttu-id="372ef-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="372ef-109">Description</span></span>                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|<span data-ttu-id="372ef-110">name</span><span class="sxs-lookup"><span data-stu-id="372ef-110">name</span></span>          | <span data-ttu-id="372ef-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="372ef-111">String</span></span>      | <span data-ttu-id="372ef-112">O nome do serviço de nuvem (por exemplo, Twitter, Instagram).</span><span class="sxs-lookup"><span data-stu-id="372ef-112">The name of the cloud service (for example, Twitter, Instagram).</span></span> |
|<span data-ttu-id="372ef-113">webUrl</span><span class="sxs-lookup"><span data-stu-id="372ef-113">webUrl</span></span>        | <span data-ttu-id="372ef-114">String</span><span class="sxs-lookup"><span data-stu-id="372ef-114">String</span></span>      | <span data-ttu-id="372ef-115">Contém a URL para o serviço que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="372ef-115">Contains the URL for the service being referenced.</span></span>               |

## <a name="json-representation"></a><span data-ttu-id="372ef-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="372ef-116">JSON representation</span></span>

<span data-ttu-id="372ef-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="372ef-117">The following is a JSON representation of the resource.</span></span>

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


