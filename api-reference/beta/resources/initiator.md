---
title: tipo de recurso do iniciador
description: Descreve quem ou o que iniciou o evento de provisionamento.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 909849775e5bf35c9a29902efbbc3975177956d1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496009"
---
# <a name="initiator-resource-type"></a><span data-ttu-id="33375-103">tipo de recurso do iniciador</span><span class="sxs-lookup"><span data-stu-id="33375-103">initiator resource type</span></span>

<span data-ttu-id="33375-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="33375-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33375-105">Descreve quem ou o que iniciou o evento de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="33375-105">Describes who or what initiated the provisioning event.</span></span> 

## <a name="properties"></a><span data-ttu-id="33375-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="33375-106">Properties</span></span>

| <span data-ttu-id="33375-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33375-107">Property</span></span>     | <span data-ttu-id="33375-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="33375-108">Type</span></span>        | <span data-ttu-id="33375-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="33375-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="33375-110">displayName</span><span class="sxs-lookup"><span data-stu-id="33375-110">displayName</span></span>|<span data-ttu-id="33375-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="33375-111">String</span></span>|<span data-ttu-id="33375-112">Nome da pessoa ou serviço que iniciou o evento de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="33375-112">Name of the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="33375-113">id</span><span class="sxs-lookup"><span data-stu-id="33375-113">id</span></span>|<span data-ttu-id="33375-114">String</span><span class="sxs-lookup"><span data-stu-id="33375-114">String</span></span>|<span data-ttu-id="33375-115">Identifica exclusivamente a pessoa ou o serviço que iniciou o evento de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="33375-115">Uniquely identifies the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="33375-116">initiatortype</span><span class="sxs-lookup"><span data-stu-id="33375-116">initiatorType</span></span>|<span data-ttu-id="33375-117">String</span><span class="sxs-lookup"><span data-stu-id="33375-117">String</span></span>| <span data-ttu-id="33375-118">Tipo de iniciador.</span><span class="sxs-lookup"><span data-stu-id="33375-118">Type of initiator.</span></span> <span data-ttu-id="33375-119">Os valores possíveis são: `user`, `app`, `system`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="33375-119">Possible values are: `user`, `app`, `system`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="33375-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="33375-120">JSON representation</span></span>

<span data-ttu-id="33375-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="33375-121">The following is a JSON representation of the resource.</span></span>

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
