---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
ms.openlocfilehash: ccea5804c3f4eddb02b5d4163302362f29b5fbc8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561324"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="ac65f-102">Tipo de recurso ContentTypeOrder</span><span class="sxs-lookup"><span data-stu-id="ac65f-102">ContentTypeOrder resource type</span></span>

<span data-ttu-id="ac65f-103">O recurso **contentTypeOrder** especifica a ordem na qual o Content Type será exibido na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="ac65f-103">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac65f-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac65f-104">JSON representation</span></span>

<span data-ttu-id="ac65f-105">Aqui está uma representação JSON de um recurso **contentTypeOrder**.</span><span class="sxs-lookup"><span data-stu-id="ac65f-105">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="ac65f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac65f-106">Properties</span></span>

| <span data-ttu-id="ac65f-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ac65f-107">Property name</span></span> | <span data-ttu-id="ac65f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac65f-108">Type</span></span>    | <span data-ttu-id="ac65f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac65f-109">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="ac65f-110">**default**</span><span class="sxs-lookup"><span data-stu-id="ac65f-110">**default**</span></span>   | <span data-ttu-id="ac65f-111">booliano</span><span class="sxs-lookup"><span data-stu-id="ac65f-111">boolean</span></span> | <span data-ttu-id="ac65f-112">Se esse é o Content Type padrão</span><span class="sxs-lookup"><span data-stu-id="ac65f-112">Whether this is the default Content Type</span></span>
| <span data-ttu-id="ac65f-113">**position**</span><span class="sxs-lookup"><span data-stu-id="ac65f-113">**position**</span></span>  | <span data-ttu-id="ac65f-114">Int32</span><span class="sxs-lookup"><span data-stu-id="ac65f-114">Int32</span></span>   | <span data-ttu-id="ac65f-115">Especifica a posição em que o tipo de conteúdo aparece na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="ac65f-115">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
