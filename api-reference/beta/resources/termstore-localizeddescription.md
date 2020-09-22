---
title: tipo de recurso localizedDescription
description: Representa a descrição localizada usada para descrever um termo no repositório de termos.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 738555750c22f3ffdd5fbd43c8b1849888e0a40f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973614"
---
# <a name="localizeddescription-resource-type"></a><span data-ttu-id="4e6ba-103">tipo de recurso localizedDescription</span><span class="sxs-lookup"><span data-stu-id="4e6ba-103">localizedDescription resource type</span></span>

<span data-ttu-id="4e6ba-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="4e6ba-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e6ba-105">Representa a descrição localizada usada para descrever um [termo] no [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="4e6ba-105">Represents the localized description used to describe a [term] in the term [store].</span></span>


## <a name="properties"></a><span data-ttu-id="4e6ba-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4e6ba-106">Properties</span></span>
|<span data-ttu-id="4e6ba-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e6ba-107">Property</span></span>|<span data-ttu-id="4e6ba-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e6ba-108">Type</span></span>|<span data-ttu-id="4e6ba-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e6ba-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e6ba-110">description</span><span class="sxs-lookup"><span data-stu-id="4e6ba-110">description</span></span>|<span data-ttu-id="4e6ba-111">String</span><span class="sxs-lookup"><span data-stu-id="4e6ba-111">String</span></span>|<span data-ttu-id="4e6ba-112">A descrição no idioma localizado.</span><span class="sxs-lookup"><span data-stu-id="4e6ba-112">The description in the localized language.</span></span>|
|<span data-ttu-id="4e6ba-113">languageTag</span><span class="sxs-lookup"><span data-stu-id="4e6ba-113">languageTag</span></span>|<span data-ttu-id="4e6ba-114">String</span><span class="sxs-lookup"><span data-stu-id="4e6ba-114">String</span></span>|<span data-ttu-id="4e6ba-115">A marca de idioma do rótulo.</span><span class="sxs-lookup"><span data-stu-id="4e6ba-115">The language tag for the label.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e6ba-116">Relações</span><span class="sxs-lookup"><span data-stu-id="4e6ba-116">Relationships</span></span>
<span data-ttu-id="4e6ba-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4e6ba-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e6ba-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4e6ba-118">JSON representation</span></span>
<span data-ttu-id="4e6ba-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4e6ba-119">The following is a JSON representation of the resource.</span></span>
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


