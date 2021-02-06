---
title: tipo de recurso iniciador
description: Descreve quem ou o que iniciou o evento de provisionamento.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 2aa8c3f365402569d7a9987d9152bae5e4e3c580
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130240"
---
# <a name="initiator-resource-type"></a><span data-ttu-id="f4ee3-103">tipo de recurso iniciador</span><span class="sxs-lookup"><span data-stu-id="f4ee3-103">initiator resource type</span></span>

<span data-ttu-id="f4ee3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4ee3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4ee3-105">Descreve quem ou o que iniciou o evento de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="f4ee3-105">Describes who or what initiated the provisioning event.</span></span> 

## <a name="properties"></a><span data-ttu-id="f4ee3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4ee3-106">Properties</span></span>

| <span data-ttu-id="f4ee3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4ee3-107">Property</span></span>     | <span data-ttu-id="f4ee3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4ee3-108">Type</span></span>        | <span data-ttu-id="f4ee3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4ee3-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f4ee3-110">displayName</span><span class="sxs-lookup"><span data-stu-id="f4ee3-110">displayName</span></span>|<span data-ttu-id="f4ee3-111">String</span><span class="sxs-lookup"><span data-stu-id="f4ee3-111">String</span></span>|<span data-ttu-id="f4ee3-112">Nome da pessoa ou serviço que iniciou o evento de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="f4ee3-112">Name of the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="f4ee3-113">id</span><span class="sxs-lookup"><span data-stu-id="f4ee3-113">id</span></span>|<span data-ttu-id="f4ee3-114">String</span><span class="sxs-lookup"><span data-stu-id="f4ee3-114">String</span></span>|<span data-ttu-id="f4ee3-115">Identifica exclusivamente a pessoa ou serviço que iniciou o evento de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="f4ee3-115">Uniquely identifies the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="f4ee3-116">initiatorType</span><span class="sxs-lookup"><span data-stu-id="f4ee3-116">initiatorType</span></span>|<span data-ttu-id="f4ee3-117">String</span><span class="sxs-lookup"><span data-stu-id="f4ee3-117">String</span></span>| <span data-ttu-id="f4ee3-118">Tipo de iniciador.</span><span class="sxs-lookup"><span data-stu-id="f4ee3-118">Type of initiator.</span></span> <span data-ttu-id="f4ee3-119">Os valores possíveis são: `user`, `app`, `system`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f4ee3-119">Possible values are: `user`, `app`, `system`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4ee3-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4ee3-120">JSON representation</span></span>

<span data-ttu-id="f4ee3-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f4ee3-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.initiator",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "id": "String",
  "initiatorType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "initiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


