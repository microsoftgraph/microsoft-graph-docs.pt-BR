---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
ms.openlocfilehash: 8cb47837d8df1c38ed25fc87d3b4d7da450fed1a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003640"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="454a3-102">Tipo de recurso ContentTypeOrder</span><span class="sxs-lookup"><span data-stu-id="454a3-102">ContentTypeOrder resource type</span></span>

<span data-ttu-id="454a3-103">O recurso **contentTypeOrder** especifica a ordem na qual o Content Type será exibido na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="454a3-103">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="454a3-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="454a3-104">JSON representation</span></span>

<span data-ttu-id="454a3-105">Aqui está uma representação JSON de um recurso **contentTypeOrder**.</span><span class="sxs-lookup"><span data-stu-id="454a3-105">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="454a3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="454a3-106">Properties</span></span>

| <span data-ttu-id="454a3-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="454a3-107">Property name</span></span> | <span data-ttu-id="454a3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="454a3-108">Type</span></span>    | <span data-ttu-id="454a3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="454a3-109">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="454a3-110">**default**</span><span class="sxs-lookup"><span data-stu-id="454a3-110">**default**</span></span>   | <span data-ttu-id="454a3-111">booliano</span><span class="sxs-lookup"><span data-stu-id="454a3-111">boolean</span></span> | <span data-ttu-id="454a3-112">Se esse é o Content Type padrão</span><span class="sxs-lookup"><span data-stu-id="454a3-112">Whether this is the default Content Type</span></span>
| <span data-ttu-id="454a3-113">**position**</span><span class="sxs-lookup"><span data-stu-id="454a3-113">**position**</span></span>  | <span data-ttu-id="454a3-114">Int32</span><span class="sxs-lookup"><span data-stu-id="454a3-114">Int32</span></span>   | <span data-ttu-id="454a3-115">Especifica a posição em que o tipo de conteúdo aparece na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="454a3-115">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
