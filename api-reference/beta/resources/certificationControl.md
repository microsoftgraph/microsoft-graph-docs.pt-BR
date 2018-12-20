---
title: " tipo de recurso de certificationControl"
description: Este recurso contém conformidade dados certificação associados a proteger o controle de pontuação.
ms.openlocfilehash: 62b6627a9bb1a012d6d7e542d87abbaddb0e279a
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380942"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="b6596-103">tipo de recurso de certificationControl</span><span class="sxs-lookup"><span data-stu-id="b6596-103">certificationControl resource type</span></span>

<span data-ttu-id="b6596-104">Conformidade de contém dados de certificação associados a proteger o controle de pontuação.</span><span class="sxs-lookup"><span data-stu-id="b6596-104">Contains compliance certification data associated with secure score control.</span></span>

|<span data-ttu-id="b6596-105">Propriedade	</span><span class="sxs-lookup"><span data-stu-id="b6596-105">Property</span></span> |<span data-ttu-id="b6596-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6596-106">Type</span></span> |<span data-ttu-id="b6596-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6596-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="b6596-108">name</span><span class="sxs-lookup"><span data-stu-id="b6596-108">name</span></span> | <span data-ttu-id="b6596-109">string</span><span class="sxs-lookup"><span data-stu-id="b6596-109">string</span></span> | <span data-ttu-id="b6596-110">Nome do controle de certificação</span><span class="sxs-lookup"><span data-stu-id="b6596-110">Certification control name</span></span> |
|<span data-ttu-id="b6596-111">url</span><span class="sxs-lookup"><span data-stu-id="b6596-111">url</span></span> | <span data-ttu-id="b6596-112">string</span><span class="sxs-lookup"><span data-stu-id="b6596-112">string</span></span> | <span data-ttu-id="b6596-113">Portal de confiança de URL para o serviço da Microsoft</span><span class="sxs-lookup"><span data-stu-id="b6596-113">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b6596-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b6596-114">JSON representation</span></span>

<span data-ttu-id="b6596-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b6596-115">The following is a JSON representation of the resource.</span></span>

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
