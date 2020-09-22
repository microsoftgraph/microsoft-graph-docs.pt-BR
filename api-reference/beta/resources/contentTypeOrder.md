---
author: daspek
description: O recurso contentTypeOrder especifica a ordem na qual o Content Type será exibido na seleção da interface do usuário.
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e7adde2a0452e9fe13a8f547eeec6fed957460da
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998898"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="49a53-103">Tipo de recurso ContentTypeOrder</span><span class="sxs-lookup"><span data-stu-id="49a53-103">ContentTypeOrder resource type</span></span>

<span data-ttu-id="49a53-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49a53-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49a53-105">O recurso **contentTypeOrder** especifica a ordem na qual o Content Type será exibido na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="49a53-105">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="49a53-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="49a53-106">JSON representation</span></span>

<span data-ttu-id="49a53-107">Aqui está uma representação JSON de um recurso **contentTypeOrder**.</span><span class="sxs-lookup"><span data-stu-id="49a53-107">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="49a53-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="49a53-108">Properties</span></span>

| <span data-ttu-id="49a53-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="49a53-109">Property name</span></span> | <span data-ttu-id="49a53-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="49a53-110">Type</span></span>    | <span data-ttu-id="49a53-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="49a53-111">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="49a53-112">**default**</span><span class="sxs-lookup"><span data-stu-id="49a53-112">**default**</span></span>   | <span data-ttu-id="49a53-113">booliano</span><span class="sxs-lookup"><span data-stu-id="49a53-113">boolean</span></span> | <span data-ttu-id="49a53-114">Se esse é o Content Type padrão</span><span class="sxs-lookup"><span data-stu-id="49a53-114">Whether this is the default Content Type</span></span>
| <span data-ttu-id="49a53-115">**position**</span><span class="sxs-lookup"><span data-stu-id="49a53-115">**position**</span></span>  | <span data-ttu-id="49a53-116">Int32</span><span class="sxs-lookup"><span data-stu-id="49a53-116">Int32</span></span>   | <span data-ttu-id="49a53-117">Especifica a posição em que o tipo de conteúdo aparece na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="49a53-117">Specifies the position in which the Content Type appears in the selection UI.</span></span>

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


