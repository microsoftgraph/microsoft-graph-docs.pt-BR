---
title: tipo de recurso displayNameLocalization
description: Fornece a capacidade de um administrador personalizar a cadeia de caracteres usada em uma experiência compartilhada do Microsoft 365.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 8ae6c62acfacfccd22cc9985386762a2f61a2bc7
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050852"
---
# <a name="displaynamelocalization-resource-type"></a><span data-ttu-id="508dc-103">tipo de recurso displayNameLocalization</span><span class="sxs-lookup"><span data-stu-id="508dc-103">displayNameLocalization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="508dc-104">Fornece a capacidade de um administrador personalizar a cadeia de caracteres usada em uma experiência compartilhada do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="508dc-104">Provides the ability for an administrator to customize the string used in a shared Microsoft 365 experience.</span></span>

## <a name="properties"></a><span data-ttu-id="508dc-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="508dc-105">Properties</span></span>

| <span data-ttu-id="508dc-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="508dc-106">Property</span></span>     | <span data-ttu-id="508dc-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="508dc-107">Type</span></span>        | <span data-ttu-id="508dc-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="508dc-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="508dc-109">displayName</span><span class="sxs-lookup"><span data-stu-id="508dc-109">displayName</span></span>   |<span data-ttu-id="508dc-110">String</span><span class="sxs-lookup"><span data-stu-id="508dc-110">String</span></span>       | <span data-ttu-id="508dc-111">Se presente, o valor desse campo contém a cadeia de caracteres **DisplayName** que foi definida para o idioma presente no campo **languageTag** .</span><span class="sxs-lookup"><span data-stu-id="508dc-111">If present, the value of this field contains the **displayName** string that has been set for the language present in the **languageTag** field.</span></span>|
|<span data-ttu-id="508dc-112">languageTag</span><span class="sxs-lookup"><span data-stu-id="508dc-112">languageTag</span></span>   |<span data-ttu-id="508dc-113">String</span><span class="sxs-lookup"><span data-stu-id="508dc-113">String</span></span>       | <span data-ttu-id="508dc-114">Fornece o código de cultura de idioma e o nome amigável do idioma no qual o campo **DisplayName** foi fornecido.</span><span class="sxs-lookup"><span data-stu-id="508dc-114">Provides the language culture-code and friendly name of the language that the **displayName** field has been provided in.</span></span>                  |

## <a name="json-representation"></a><span data-ttu-id="508dc-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="508dc-115">JSON representation</span></span>

<span data-ttu-id="508dc-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="508dc-116">The following is a JSON representation of the resource.</span></span>

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
