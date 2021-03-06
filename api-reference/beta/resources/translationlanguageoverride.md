---
title: Tipo de recurso translationLanguageOverride
description: Um recurso que representa uma entrada na lista de substituição de idioma de conversão.
localization_priority: Normal
author: jasonbro
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 791908546c64cbb0ea7ee7434bece3dca5c894cc
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518138"
---
# <a name="translationlanguageoverride-resource-type"></a><span data-ttu-id="5633d-103">Tipo de recurso translationLanguageOverride</span><span class="sxs-lookup"><span data-stu-id="5633d-103">translationLanguageOverride resource type</span></span>

<span data-ttu-id="5633d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5633d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5633d-105">Representa qualquer substituição de conversão para um idioma.</span><span class="sxs-lookup"><span data-stu-id="5633d-105">Represents any translation override for a language.</span></span>

## <a name="properties"></a><span data-ttu-id="5633d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5633d-106">Properties</span></span>

|<span data-ttu-id="5633d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5633d-107">Property</span></span>             |<span data-ttu-id="5633d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5633d-108">Type</span></span>                                         |<span data-ttu-id="5633d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5633d-109">Description</span></span>                                                            |
|---------------------|-------------------------------------------------------------|-----------------------------------------------------------------------|
|<span data-ttu-id="5633d-110">languageTag</span><span class="sxs-lookup"><span data-stu-id="5633d-110">languageTag</span></span>          |<span data-ttu-id="5633d-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5633d-111">String</span></span>                                       |<span data-ttu-id="5633d-112">O idioma para aplicar a substituição.</span><span class="sxs-lookup"><span data-stu-id="5633d-112">The language to apply the override.</span></span><br><br><span data-ttu-id="5633d-113">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="5633d-113">Returned by default.</span></span> <span data-ttu-id="5633d-114">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="5633d-114">Not nullable.</span></span>       |                   
|<span data-ttu-id="5633d-115">translationBehavior</span><span class="sxs-lookup"><span data-stu-id="5633d-115">translationBehavior</span></span>  |[<span data-ttu-id="5633d-116">translationBehavior</span><span class="sxs-lookup"><span data-stu-id="5633d-116">translationBehavior</span></span>](translationPreferences.md#translationbehavior-values)        |<span data-ttu-id="5633d-117">O comportamento de substituição de conversão para o idioma, se for o caso.</span><span class="sxs-lookup"><span data-stu-id="5633d-117">The translation override behavior for the language, if any.</span></span><br><br><span data-ttu-id="5633d-118">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="5633d-118">Returned by default.</span></span> <span data-ttu-id="5633d-119">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="5633d-119">Not nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5633d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5633d-120">JSON representation</span></span>

<span data-ttu-id="5633d-121">A seguir está uma definição JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5633d-121">The following is a JSON definition of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.translationLanguageOverride"
}-->

```json
{
    "languageTag": "string",
    "translationBehavior": "string"
}
```
<!-- {
  "type": "#page.annotation",
  "description": translationLanguageOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


