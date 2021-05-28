---
title: Tipo de recurso localizedLabel
description: Representa o rótulo de um termo no armazenamento de termos.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 4d7de3c9567c20659af4c863d2cf1ac248beff6b
ms.sourcegitcommit: a9a035e7cf7b500aebe5477c05361552e7c3a7ab
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696307"
---
# <a name="localizedlabel-resource-type"></a><span data-ttu-id="a2652-103">Tipo de recurso localizedLabel</span><span class="sxs-lookup"><span data-stu-id="a2652-103">localizedLabel resource type</span></span>

<span data-ttu-id="a2652-104">Namespace: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="a2652-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2652-105">Representa o rótulo de [um termo] no armazenamento de [termos.]</span><span class="sxs-lookup"><span data-stu-id="a2652-105">Represents the label for a [term] in the term [store].</span></span>

<span data-ttu-id="a2652-106">Identifica os rótulos associados a um determinado termo.</span><span class="sxs-lookup"><span data-stu-id="a2652-106">Identifies the labels associated with a given term.</span></span>

## <a name="properties"></a><span data-ttu-id="a2652-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2652-107">Properties</span></span>
|<span data-ttu-id="a2652-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2652-108">Property</span></span>|<span data-ttu-id="a2652-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2652-109">Type</span></span>|<span data-ttu-id="a2652-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2652-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2652-111">isDefault</span><span class="sxs-lookup"><span data-stu-id="a2652-111">isDefault</span></span>|<span data-ttu-id="a2652-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="a2652-112">Boolean</span></span>|<span data-ttu-id="a2652-113">Indica se o rótulo é o rótulo padrão.</span><span class="sxs-lookup"><span data-stu-id="a2652-113">Indicates whether the label is the default label.</span></span>|
|<span data-ttu-id="a2652-114">languageTag</span><span class="sxs-lookup"><span data-stu-id="a2652-114">languageTag</span></span>|<span data-ttu-id="a2652-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2652-115">String</span></span>|<span data-ttu-id="a2652-116">A marca de idioma do rótulo.</span><span class="sxs-lookup"><span data-stu-id="a2652-116">The language tag for the label.</span></span>|
|<span data-ttu-id="a2652-117">nome</span><span class="sxs-lookup"><span data-stu-id="a2652-117">name</span></span>|<span data-ttu-id="a2652-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2652-118">String</span></span>|<span data-ttu-id="a2652-119">O nome do rótulo.</span><span class="sxs-lookup"><span data-stu-id="a2652-119">The name of the label.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2652-120">Relações</span><span class="sxs-lookup"><span data-stu-id="a2652-120">Relationships</span></span>
<span data-ttu-id="a2652-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a2652-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2652-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2652-122">JSON representation</span></span>
<span data-ttu-id="a2652-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a2652-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.termStore.localizedLabel"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.localizedLabel",
  "name": "String",
  "isDefault": "Boolean",
  "languageTag": "String"
}
```


[microsoft.graph.termStore.term]: termstore-term.md
[microsoft.graph.termStore.localizedName]: termstore-localizedname.md
[microsoft.graph.termStore.store]: termstore-store.md
[term]: ../resources/termstore-term.md
[store]: ../resources/termstore-store.md


<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedLabelFacet is the facet for containing the label of a term",
  "keywords": "termLocalizedLabelFacet,facet,resource",
  "section": "documentation",
  "tocPath": "termstorelocalizedlabel",
  "tocBookmarks": {
    "Resources/termStore.termstorelocalizedlabel&quot;: &quot;#"
  },
  "suppressions": []
}
-->


