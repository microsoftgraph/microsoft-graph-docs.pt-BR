---
author: daspek
description: O recurso contentTypeOrder especifica a ordem na qual o Content Type será exibido na seleção da interface do usuário.
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 464ac5978f505e74ca99226080c35574917fd550
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973191"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="ac593-103">Tipo de recurso ContentTypeOrder</span><span class="sxs-lookup"><span data-stu-id="ac593-103">ContentTypeOrder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac593-104">O recurso **contentTypeOrder** especifica a ordem na qual o Content Type será exibido na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="ac593-104">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac593-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac593-105">JSON representation</span></span>

<span data-ttu-id="ac593-106">Aqui está uma representação JSON de um recurso **contentTypeOrder**.</span><span class="sxs-lookup"><span data-stu-id="ac593-106">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="ac593-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac593-107">Properties</span></span>

| <span data-ttu-id="ac593-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ac593-108">Property name</span></span> | <span data-ttu-id="ac593-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac593-109">Type</span></span>    | <span data-ttu-id="ac593-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac593-110">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="ac593-111">**default**</span><span class="sxs-lookup"><span data-stu-id="ac593-111">**default**</span></span>   | <span data-ttu-id="ac593-112">booliano</span><span class="sxs-lookup"><span data-stu-id="ac593-112">boolean</span></span> | <span data-ttu-id="ac593-113">Se esse é o Content Type padrão</span><span class="sxs-lookup"><span data-stu-id="ac593-113">Whether this is the default Content Type</span></span>
| <span data-ttu-id="ac593-114">**position**</span><span class="sxs-lookup"><span data-stu-id="ac593-114">**position**</span></span>  | <span data-ttu-id="ac593-115">Int32</span><span class="sxs-lookup"><span data-stu-id="ac593-115">Int32</span></span>   | <span data-ttu-id="ac593-116">Especifica a posição em que o tipo de conteúdo aparece na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="ac593-116">Specifies the position in which the Content Type appears in the selection UI.</span></span>

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
