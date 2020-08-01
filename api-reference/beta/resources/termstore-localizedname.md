---
title: tipo de recurso localizadoname
description: Representa o nome localizado usado no repositório de termos, que identifica o nome no idioma localizado.
author: mohitpcad
ms.author: mopathak
localization_priority: Normal
ms.prod: sharepoint-taxonomy
doc_type: resourcePageType
ms.openlocfilehash: cc29deb6e6db5f5664e6fb6bed69195b7183e026
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539127"
---
# <a name="localizedname-resource-type"></a><span data-ttu-id="65240-103">tipo de recurso localizadoname</span><span class="sxs-lookup"><span data-stu-id="65240-103">localizedName resource type</span></span>

<span data-ttu-id="65240-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="65240-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65240-105">Representa o nome localizado usado no [repositório]de termos, que identifica o nome no idioma localizado.</span><span class="sxs-lookup"><span data-stu-id="65240-105">Represents the localized name used in the term [store], which identifies the name in the localized language.</span></span> <span data-ttu-id="65240-106">Para obter mais informações, consulte [localizedLabel].</span><span class="sxs-lookup"><span data-stu-id="65240-106">For more information, see [localizedLabel].</span></span>

## <a name="properties"></a><span data-ttu-id="65240-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="65240-107">Properties</span></span>
|<span data-ttu-id="65240-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65240-108">Property</span></span>|<span data-ttu-id="65240-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="65240-109">Type</span></span>|<span data-ttu-id="65240-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="65240-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65240-111">languageTag</span><span class="sxs-lookup"><span data-stu-id="65240-111">languageTag</span></span>|<span data-ttu-id="65240-112">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="65240-112">String</span></span>|<span data-ttu-id="65240-113">A marca de idioma do rótulo.</span><span class="sxs-lookup"><span data-stu-id="65240-113">The language tag for the label.</span></span>|
|<span data-ttu-id="65240-114">nome</span><span class="sxs-lookup"><span data-stu-id="65240-114">name</span></span>|<span data-ttu-id="65240-115">String</span><span class="sxs-lookup"><span data-stu-id="65240-115">String</span></span>|<span data-ttu-id="65240-116">O nome no idioma localizado.</span><span class="sxs-lookup"><span data-stu-id="65240-116">The name in the localized language.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65240-117">Relações</span><span class="sxs-lookup"><span data-stu-id="65240-117">Relationships</span></span>
<span data-ttu-id="65240-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="65240-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="65240-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="65240-119">JSON representation</span></span>
<span data-ttu-id="65240-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="65240-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.termStore.localizedName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.localizedName",
  "name": "String",
  "languageTag": "String"
}
```

[microsoft.graph.termStore.localizedLabel]: termstore-localizedlabel.md
[microsoft.graph.termstore.store]: termstore-store.md
[Guarde]: ../resources/termstore-store.md
[store]: ../resources/termstore-store.md
[localizedLabel]: ../resources/termstore-localizedlabel.md

<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedName is the facet for containing the name of termGroup",
  "keywords": "termLocalizedLNameFacet,facet,resource",
  "section": "documentation",
  "tocPath": "TermLocalizedNameFacet",
  "tocBookmarks": {
    "Resources/termStore.termLocalizedName": "#"
  },
  "suppressions": []
}
-->
