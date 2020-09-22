---
title: tipo de recurso displayNameLocalization
description: Fornece a capacidade de um administrador personalizar a cadeia de caracteres usada em uma experiência compartilhada do Microsoft 365.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: e02af0d4fcd5cdf4ce08df4403736bd6b9c60a84
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010399"
---
# <a name="displaynamelocalization-resource-type"></a><span data-ttu-id="ddb62-103">tipo de recurso displayNameLocalization</span><span class="sxs-lookup"><span data-stu-id="ddb62-103">displayNameLocalization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddb62-104">Fornece a capacidade de um administrador personalizar a cadeia de caracteres usada em uma experiência compartilhada do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ddb62-104">Provides the ability for an administrator to customize the string used in a shared Microsoft 365 experience.</span></span>

## <a name="properties"></a><span data-ttu-id="ddb62-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ddb62-105">Properties</span></span>

| <span data-ttu-id="ddb62-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ddb62-106">Property</span></span>     | <span data-ttu-id="ddb62-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ddb62-107">Type</span></span>        | <span data-ttu-id="ddb62-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddb62-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ddb62-109">displayName</span><span class="sxs-lookup"><span data-stu-id="ddb62-109">displayName</span></span>   |<span data-ttu-id="ddb62-110">String</span><span class="sxs-lookup"><span data-stu-id="ddb62-110">String</span></span>       | <span data-ttu-id="ddb62-111">Se presente, o valor desse campo contém a cadeia de caracteres **DisplayName** que foi definida para o idioma presente no campo **languageTag** .</span><span class="sxs-lookup"><span data-stu-id="ddb62-111">If present, the value of this field contains the **displayName** string that has been set for the language present in the **languageTag** field.</span></span>|
|<span data-ttu-id="ddb62-112">languageTag</span><span class="sxs-lookup"><span data-stu-id="ddb62-112">languageTag</span></span>   |<span data-ttu-id="ddb62-113">String</span><span class="sxs-lookup"><span data-stu-id="ddb62-113">String</span></span>       | <span data-ttu-id="ddb62-114">Fornece o código de cultura de idioma e o nome amigável do idioma no qual o campo **DisplayName** foi fornecido.</span><span class="sxs-lookup"><span data-stu-id="ddb62-114">Provides the language culture-code and friendly name of the language that the **displayName** field has been provided in.</span></span>                  |

## <a name="json-representation"></a><span data-ttu-id="ddb62-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ddb62-115">JSON representation</span></span>

<span data-ttu-id="ddb62-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ddb62-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.displayNameLocalization",
  "baseType": null
}-->

```json
{
  "displayName": "string",
  "languageTag": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "displayNameLocalization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


