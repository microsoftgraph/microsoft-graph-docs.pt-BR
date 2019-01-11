---
title: " tipo de recurso de certificationControl"
description: Este recurso contém conformidade dados certificação associados a proteger o controle de pontuação.
localization_priority: Normal
ms.openlocfilehash: 6f8269a85a8d3cb032f3e58457df95f4dd432c11
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810385"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="add28-103">tipo de recurso de certificationControl</span><span class="sxs-lookup"><span data-stu-id="add28-103">certificationControl resource type</span></span>

<span data-ttu-id="add28-104">Conformidade de contém dados de certificação associados a proteger o controle de pontuação.</span><span class="sxs-lookup"><span data-stu-id="add28-104">Contains compliance certification data associated with secure score control.</span></span>

|<span data-ttu-id="add28-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="add28-105">Property</span></span> |<span data-ttu-id="add28-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="add28-106">Type</span></span> |<span data-ttu-id="add28-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="add28-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="add28-108">name</span><span class="sxs-lookup"><span data-stu-id="add28-108">name</span></span> | <span data-ttu-id="add28-109">string</span><span class="sxs-lookup"><span data-stu-id="add28-109">string</span></span> | <span data-ttu-id="add28-110">Nome do controle de certificação</span><span class="sxs-lookup"><span data-stu-id="add28-110">Certification control name</span></span> |
|<span data-ttu-id="add28-111">url</span><span class="sxs-lookup"><span data-stu-id="add28-111">url</span></span> | <span data-ttu-id="add28-112">string</span><span class="sxs-lookup"><span data-stu-id="add28-112">string</span></span> | <span data-ttu-id="add28-113">Portal de confiança de URL para o serviço da Microsoft</span><span class="sxs-lookup"><span data-stu-id="add28-113">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="add28-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="add28-114">JSON representation</span></span>

<span data-ttu-id="add28-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="add28-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificationControl"
}-->

```json
{
  "name": "String",
  "url": "Collection(microsoft.graph.certificationControl)"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "certificationControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
