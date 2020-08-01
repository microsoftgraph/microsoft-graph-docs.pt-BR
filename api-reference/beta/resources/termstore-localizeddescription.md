---
title: tipo de recurso localizedDescription
description: Representa a descrição localizada usada para descrever um termo no repositório de termos.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 0bded2c1ad4804fb952ecfd9c75c87f3a8624c7e
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539128"
---
# <a name="localizeddescription-resource-type"></a><span data-ttu-id="e433c-103">tipo de recurso localizedDescription</span><span class="sxs-lookup"><span data-stu-id="e433c-103">localizedDescription resource type</span></span>

<span data-ttu-id="e433c-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="e433c-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e433c-105">Representa a descrição localizada usada para descrever um [termo] no [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="e433c-105">Represents the localized description used to describe a [term] in the term [store].</span></span>


## <a name="properties"></a><span data-ttu-id="e433c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e433c-106">Properties</span></span>
|<span data-ttu-id="e433c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e433c-107">Property</span></span>|<span data-ttu-id="e433c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e433c-108">Type</span></span>|<span data-ttu-id="e433c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e433c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e433c-110">description</span><span class="sxs-lookup"><span data-stu-id="e433c-110">description</span></span>|<span data-ttu-id="e433c-111">String</span><span class="sxs-lookup"><span data-stu-id="e433c-111">String</span></span>|<span data-ttu-id="e433c-112">A descrição no idioma localizado.</span><span class="sxs-lookup"><span data-stu-id="e433c-112">The description in the localized language.</span></span>|
|<span data-ttu-id="e433c-113">languageTag</span><span class="sxs-lookup"><span data-stu-id="e433c-113">languageTag</span></span>|<span data-ttu-id="e433c-114">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="e433c-114">String</span></span>|<span data-ttu-id="e433c-115">A marca de idioma do rótulo.</span><span class="sxs-lookup"><span data-stu-id="e433c-115">The language tag for the label.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e433c-116">Relações</span><span class="sxs-lookup"><span data-stu-id="e433c-116">Relationships</span></span>
<span data-ttu-id="e433c-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e433c-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e433c-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e433c-118">JSON representation</span></span>
<span data-ttu-id="e433c-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e433c-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.termStore.localizedDescription"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.localizedDescription",
  "description": "String",
  "languageTag": "String"
}
```

[microsoft.graph.termStore.term]: termStore-term.md
[microsoft.graph.termStore.store]: termStore-store.md
[terminal]: ../resources/termstore-term.md
[term]: ../resources/termstore-term.md
[Guarde]: ../resources/termstore-store.md
[store]: ../resources/termstore-store.md

<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedDescriptionFacet is the facet for containing the description of a set",
  "keywords": "termLocalizedDescriptionFacet,facet,resource",
  "section": "documentation",
  "tocPath": "TermLocalizedDescriptionFacet",
  "tocBookmarks": {
    "Resources/termStore.termLocalizedDescription": "#"
  },
  "suppressions": []
}
-->
