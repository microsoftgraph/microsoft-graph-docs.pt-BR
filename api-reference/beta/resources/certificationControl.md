---
title: " tipo de recurso certificationControl"
description: Este recurso contém dados de certificação de conformidade associados ao controle de Pontuação segura.
localization_priority: Normal
ms.openlocfilehash: 6f8269a85a8d3cb032f3e58457df95f4dd432c11
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535410"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="297d4-103">tipo de recurso certificationControl</span><span class="sxs-lookup"><span data-stu-id="297d4-103">certificationControl resource type</span></span>

<span data-ttu-id="297d4-104">Contém dados de certificação de conformidade associados ao controle de Pontuação segura.</span><span class="sxs-lookup"><span data-stu-id="297d4-104">Contains compliance certification data associated with secure score control.</span></span>

|<span data-ttu-id="297d4-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="297d4-105">Property</span></span> |<span data-ttu-id="297d4-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="297d4-106">Type</span></span> |<span data-ttu-id="297d4-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="297d4-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="297d4-108">name</span><span class="sxs-lookup"><span data-stu-id="297d4-108">name</span></span> | <span data-ttu-id="297d4-109">string</span><span class="sxs-lookup"><span data-stu-id="297d4-109">string</span></span> | <span data-ttu-id="297d4-110">Nome do controle de certificação</span><span class="sxs-lookup"><span data-stu-id="297d4-110">Certification control name</span></span> |
|<span data-ttu-id="297d4-111">url</span><span class="sxs-lookup"><span data-stu-id="297d4-111">url</span></span> | <span data-ttu-id="297d4-112">string</span><span class="sxs-lookup"><span data-stu-id="297d4-112">string</span></span> | <span data-ttu-id="297d4-113">URL para o portal de confiança do serviço Microsoft</span><span class="sxs-lookup"><span data-stu-id="297d4-113">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="297d4-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="297d4-114">JSON representation</span></span>

<span data-ttu-id="297d4-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="297d4-115">The following is a JSON representation of the resource.</span></span>

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
