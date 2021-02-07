---
title: Tipo de recurso localeInfo
description: Informações sobre a localidade, incluindo o idioma preferencial e o país/região do usuário conectado.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 893d0985d72eb74b6850652ae375f336df1abe1a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131667"
---
# <a name="localeinfo-resource-type"></a><span data-ttu-id="d8a75-103">Tipo de recurso localeInfo</span><span class="sxs-lookup"><span data-stu-id="d8a75-103">localeInfo resource type</span></span>

<span data-ttu-id="d8a75-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8a75-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d8a75-105">Informações sobre a localidade, incluindo o idioma preferencial e o país/região do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="d8a75-105">Information about the locale, including the preferred language and country/region, of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="d8a75-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8a75-106">Properties</span></span>
| <span data-ttu-id="d8a75-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8a75-107">Property</span></span>     | <span data-ttu-id="d8a75-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8a75-108">Type</span></span>   |<span data-ttu-id="d8a75-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8a75-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8a75-110">localidade</span><span class="sxs-lookup"><span data-stu-id="d8a75-110">locale</span></span>|<span data-ttu-id="d8a75-111">string</span><span class="sxs-lookup"><span data-stu-id="d8a75-111">string</span></span>|<span data-ttu-id="d8a75-p101">Uma representação da localidade do usuário, que inclui o idioma preferencial do usuário e o país/região. Por exemplo, "pt-br". O componente do idioma segue um padrão de código de duas letras, conforme definido na [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), e o componente do país segue um padrão de código de duas letras, conforme definido na [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span><span class="sxs-lookup"><span data-stu-id="d8a75-p101">A locale representation for the user, which includes the user's preferred language and country/region. For example, "en-us". The language component follows 2-letter codes as defined in [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), and the country component follows 2-letter codes as defined in [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span></span>|
|<span data-ttu-id="d8a75-115">displayName</span><span class="sxs-lookup"><span data-stu-id="d8a75-115">displayName</span></span>|<span data-ttu-id="d8a75-116">string</span><span class="sxs-lookup"><span data-stu-id="d8a75-116">string</span></span>|<span data-ttu-id="d8a75-117">Um nome que representa a localidade do usuário em seu idioma natural, por exemplo, "Português (Brasil)".</span><span class="sxs-lookup"><span data-stu-id="d8a75-117">A name representing the user's locale in natural language, for example, "English (United States)".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8a75-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8a75-118">JSON representation</span></span>

<span data-ttu-id="d8a75-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d8a75-119">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "localeInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

