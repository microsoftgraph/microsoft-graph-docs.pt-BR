---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
ms.openlocfilehash: 32cca632933cf2b0fad1f8e9149973d95b4322d3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341224"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="826f1-102">Tipo de recurso ContentTypeOrder</span><span class="sxs-lookup"><span data-stu-id="826f1-102">ContentTypeOrder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="826f1-103">O recurso **contentTypeOrder** especifica a ordem na qual o Content Type será exibido na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="826f1-103">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="826f1-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="826f1-104">JSON representation</span></span>

<span data-ttu-id="826f1-105">Aqui está uma representação JSON de um recurso **contentTypeOrder**.</span><span class="sxs-lookup"><span data-stu-id="826f1-105">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="826f1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="826f1-106">Properties</span></span>

| <span data-ttu-id="826f1-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="826f1-107">Property name</span></span> | <span data-ttu-id="826f1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="826f1-108">Type</span></span>    | <span data-ttu-id="826f1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="826f1-109">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="826f1-110">**default**</span><span class="sxs-lookup"><span data-stu-id="826f1-110">**default**</span></span>   | <span data-ttu-id="826f1-111">booliano</span><span class="sxs-lookup"><span data-stu-id="826f1-111">boolean</span></span> | <span data-ttu-id="826f1-112">Se esse é o Content Type padrão</span><span class="sxs-lookup"><span data-stu-id="826f1-112">Whether this is the default Content Type</span></span>
| <span data-ttu-id="826f1-113">**position**</span><span class="sxs-lookup"><span data-stu-id="826f1-113">**position**</span></span>  | <span data-ttu-id="826f1-114">Int32</span><span class="sxs-lookup"><span data-stu-id="826f1-114">Int32</span></span>   | <span data-ttu-id="826f1-115">Especifica a posição em que o tipo de conteúdo aparece na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="826f1-115">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder",
  "suppressions": []
}
-->
