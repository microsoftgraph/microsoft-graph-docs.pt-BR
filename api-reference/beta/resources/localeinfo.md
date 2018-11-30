---
title: Tipo de recurso localeInfo
description: Informações sobre a localidade, incluindo o idioma preferencial e o país/região do usuário conectado.
ms.openlocfilehash: 5dae464a4931fb094ae47cce600a95d55c6c3f93
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039463"
---
# <a name="localeinfo-resource-type"></a><span data-ttu-id="defa2-103">Tipo de recurso localeInfo</span><span class="sxs-lookup"><span data-stu-id="defa2-103">localeInfo resource type</span></span>

> <span data-ttu-id="defa2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="defa2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="defa2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="defa2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="defa2-106">Informações sobre a localidade, incluindo o idioma preferencial e o país/região do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="defa2-106">Information about the locale, including the preferred language and country/region, of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="defa2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="defa2-107">Properties</span></span>
| <span data-ttu-id="defa2-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="defa2-108">Property</span></span>     | <span data-ttu-id="defa2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="defa2-109">Type</span></span>   |<span data-ttu-id="defa2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="defa2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="defa2-111">localidade</span><span class="sxs-lookup"><span data-stu-id="defa2-111">locale</span></span>|<span data-ttu-id="defa2-112">string</span><span class="sxs-lookup"><span data-stu-id="defa2-112">string</span></span>|<span data-ttu-id="defa2-p102">Uma representação da localidade do usuário, que inclui o idioma preferencial do usuário e o país/região. Por exemplo, "pt-br". O componente do idioma segue um padrão de código de duas letras, conforme definido na [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), e o componente do país segue um padrão de código de duas letras, conforme definido na [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span><span class="sxs-lookup"><span data-stu-id="defa2-p102">A locale representation for the user, which includes the user's preferred language and country/region. For example, "en-us". The language component follows 2-letter codes as defined in [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), and the country component follows 2-letter codes as defined in [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span></span>|
|<span data-ttu-id="defa2-116">displayName</span><span class="sxs-lookup"><span data-stu-id="defa2-116">displayName</span></span>|<span data-ttu-id="defa2-117">string</span><span class="sxs-lookup"><span data-stu-id="defa2-117">string</span></span>|<span data-ttu-id="defa2-118">Um nome que representa a localidade do usuário em seu idioma natural, por exemplo, "Português (Brasil)".</span><span class="sxs-lookup"><span data-stu-id="defa2-118">A name representing the user's locale in natural language, for example, "English (United States)".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="defa2-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="defa2-119">JSON representation</span></span>

<span data-ttu-id="defa2-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="defa2-120">Here is a JSON representation of the resource.</span></span>

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