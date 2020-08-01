---
title: tipo de recurso localizedLabel
description: Representa o rótulo de um termo no repositório de termos.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: dbd067dbd3447691fd7fbd8e51670cceb46d64da
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539140"
---
# <a name="localizedlabel-resource-type"></a><span data-ttu-id="23760-103">tipo de recurso localizedLabel</span><span class="sxs-lookup"><span data-stu-id="23760-103">localizedLabel resource type</span></span>

<span data-ttu-id="23760-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="23760-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23760-105">Representa o rótulo de um [termo] no [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="23760-105">Represents the label for a [term] in the term [store].</span></span>

<span data-ttu-id="23760-106">Identifica os rótulos associados a um determinado termo.</span><span class="sxs-lookup"><span data-stu-id="23760-106">Identifies the labels associated with a given term.</span></span>

## <a name="properties"></a><span data-ttu-id="23760-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23760-107">Properties</span></span>
|<span data-ttu-id="23760-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23760-108">Property</span></span>|<span data-ttu-id="23760-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="23760-109">Type</span></span>|<span data-ttu-id="23760-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="23760-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23760-111">isDefault</span><span class="sxs-lookup"><span data-stu-id="23760-111">isDefault</span></span>|<span data-ttu-id="23760-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="23760-112">Boolean</span></span>|<span data-ttu-id="23760-113">Indica se o rótulo é o rótulo padrão.</span><span class="sxs-lookup"><span data-stu-id="23760-113">Indicates whether the label is the default label.</span></span>|
|<span data-ttu-id="23760-114">languageTag</span><span class="sxs-lookup"><span data-stu-id="23760-114">languageTag</span></span>|<span data-ttu-id="23760-115">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="23760-115">String</span></span>|<span data-ttu-id="23760-116">A marca anguage do rótulo.</span><span class="sxs-lookup"><span data-stu-id="23760-116">The anguage tag for the label.</span></span>|
|<span data-ttu-id="23760-117">nome</span><span class="sxs-lookup"><span data-stu-id="23760-117">name</span></span>|<span data-ttu-id="23760-118">String</span><span class="sxs-lookup"><span data-stu-id="23760-118">String</span></span>|<span data-ttu-id="23760-119">O nome do rótulo.</span><span class="sxs-lookup"><span data-stu-id="23760-119">The name of the label.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23760-120">Relações</span><span class="sxs-lookup"><span data-stu-id="23760-120">Relationships</span></span>
<span data-ttu-id="23760-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23760-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="23760-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23760-122">JSON representation</span></span>
<span data-ttu-id="23760-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23760-123">The following is a JSON representation of the resource.</span></span>
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
[terminal]: ../resources/termstore-term.md
[term]: ../resources/termstore-term.md
[Guarde]: ../resources/termstore-store.md
[store]: ../resources/termstore-store.md


<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedLabelFacet is the facet for containing the label of a term",
  "keywords": "termLocalizedLabelFacet,facet,resource",
  "section": "documentation",
  "tocPath": "termstorelocalizedlabel",
  "tocBookmarks": {
    "Resources/termStore.termstorelocalizedlabel": "#"
  },
  "suppressions": []
}
-->
