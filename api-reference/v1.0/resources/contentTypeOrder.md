---
author: daspek
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
description: O recurso contentTypeOrder especifica a ordem na qual o Content Type será exibido na seleção da interface do usuário.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e25025e86c03d7c94ed88a94ad390a56db4a44b0
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238502"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="50621-103">Tipo de recurso ContentTypeOrder</span><span class="sxs-lookup"><span data-stu-id="50621-103">ContentTypeOrder resource type</span></span>

<span data-ttu-id="50621-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50621-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="50621-105">O recurso **contentTypeOrder** especifica a ordem na qual o Content Type será exibido na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="50621-105">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="50621-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50621-106">JSON representation</span></span>

<span data-ttu-id="50621-107">Aqui está uma representação JSON de um recurso **contentTypeOrder**.</span><span class="sxs-lookup"><span data-stu-id="50621-107">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="50621-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50621-108">Properties</span></span>

| <span data-ttu-id="50621-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="50621-109">Property name</span></span> | <span data-ttu-id="50621-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="50621-110">Type</span></span>    | <span data-ttu-id="50621-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="50621-111">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="50621-112">**default**</span><span class="sxs-lookup"><span data-stu-id="50621-112">**default**</span></span>   | <span data-ttu-id="50621-113">booliano</span><span class="sxs-lookup"><span data-stu-id="50621-113">boolean</span></span> | <span data-ttu-id="50621-114">Se esse é o Content Type padrão</span><span class="sxs-lookup"><span data-stu-id="50621-114">Whether this is the default Content Type</span></span>
| <span data-ttu-id="50621-115">**position**</span><span class="sxs-lookup"><span data-stu-id="50621-115">**position**</span></span>  | <span data-ttu-id="50621-116">Int32</span><span class="sxs-lookup"><span data-stu-id="50621-116">Int32</span></span>   | <span data-ttu-id="50621-117">Especifica a posição em que o tipo de conteúdo aparece na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="50621-117">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->

