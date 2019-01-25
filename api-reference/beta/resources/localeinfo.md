---
title: Tipo de recurso localeInfo
description: Informações sobre a localidade, incluindo o idioma preferencial e o país/região do usuário conectado.
localization_priority: Normal
ms.openlocfilehash: 7414130c1ed1e85353c653d9bbd36a0e488bcea9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520211"
---
# <a name="localeinfo-resource-type"></a><span data-ttu-id="c66d2-103">Tipo de recurso localeInfo</span><span class="sxs-lookup"><span data-stu-id="c66d2-103">localeInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c66d2-104">Informações sobre a localidade, incluindo o idioma preferencial e o país/região do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="c66d2-104">Information about the locale, including the preferred language and country/region, of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="c66d2-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c66d2-105">Properties</span></span>
| <span data-ttu-id="c66d2-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c66d2-106">Property</span></span>     | <span data-ttu-id="c66d2-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c66d2-107">Type</span></span>   |<span data-ttu-id="c66d2-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c66d2-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c66d2-109">localidade</span><span class="sxs-lookup"><span data-stu-id="c66d2-109">locale</span></span>|<span data-ttu-id="c66d2-110">string</span><span class="sxs-lookup"><span data-stu-id="c66d2-110">string</span></span>|<span data-ttu-id="c66d2-p101">Uma representação da localidade do usuário, que inclui o idioma preferencial do usuário e o país/região. Por exemplo, "pt-br". O componente do idioma segue um padrão de código de duas letras, conforme definido na [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), e o componente do país segue um padrão de código de duas letras, conforme definido na [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span><span class="sxs-lookup"><span data-stu-id="c66d2-p101">A locale representation for the user, which includes the user's preferred language and country/region. For example, "en-us". The language component follows 2-letter codes as defined in [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), and the country component follows 2-letter codes as defined in [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span></span>|
|<span data-ttu-id="c66d2-114">displayName</span><span class="sxs-lookup"><span data-stu-id="c66d2-114">displayName</span></span>|<span data-ttu-id="c66d2-115">string</span><span class="sxs-lookup"><span data-stu-id="c66d2-115">string</span></span>|<span data-ttu-id="c66d2-116">Um nome que representa a localidade do usuário em seu idioma natural, por exemplo, "Português (Brasil)".</span><span class="sxs-lookup"><span data-stu-id="c66d2-116">A name representing the user's locale in natural language, for example, "English (United States)".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c66d2-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c66d2-117">JSON representation</span></span>

<span data-ttu-id="c66d2-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c66d2-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.localeInfo"
}-->

```json
{
  "locale": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "localeInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/localeinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
