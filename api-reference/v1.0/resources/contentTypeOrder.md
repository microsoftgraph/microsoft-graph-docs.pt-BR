---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
ms.openlocfilehash: fe7309373ded16fe2660e0c5a69773c18ffb581a
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="35636-102">Tipo de recurso ContentTypeOrder</span><span class="sxs-lookup"><span data-stu-id="35636-102">ContentTypeOrder resource type</span></span>

<span data-ttu-id="35636-103">O recurso **contentTypeOrder** especifica a ordem na qual o Content Type será exibido na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="35636-103">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="35636-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="35636-104">JSON representation</span></span>

<span data-ttu-id="35636-105">Aqui está uma representação JSON de um recurso **contentTypeOrder**.</span><span class="sxs-lookup"><span data-stu-id="35636-105">Here is a JSON representation of a **baseItem** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="35636-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="35636-106">Properties</span></span>

| <span data-ttu-id="35636-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="35636-107">Property name</span></span> | <span data-ttu-id="35636-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="35636-108">Type</span></span>    | <span data-ttu-id="35636-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="35636-109">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="35636-110">**default**</span><span class="sxs-lookup"><span data-stu-id="35636-110">**default**</span></span>   | <span data-ttu-id="35636-111">booliano</span><span class="sxs-lookup"><span data-stu-id="35636-111">boolean</span></span> | <span data-ttu-id="35636-112">Se esse é o Content Type padrão</span><span class="sxs-lookup"><span data-stu-id="35636-112">Whether this is the default Content Type</span></span>
| <span data-ttu-id="35636-113">**position**</span><span class="sxs-lookup"><span data-stu-id="35636-113">**position**</span></span>  | <span data-ttu-id="35636-114">Int32</span><span class="sxs-lookup"><span data-stu-id="35636-114">Int32</span></span>   | <span data-ttu-id="35636-115">Especifica a posição em que o tipo de conteúdo aparece na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="35636-115">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
