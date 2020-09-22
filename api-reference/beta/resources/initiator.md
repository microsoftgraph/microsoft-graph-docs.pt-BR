---
title: tipo de recurso do iniciador
description: Descreve quem ou o que iniciou o evento de provisionamento.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c0b6b326925d0ca3f0dbf8c0c25df266834ecce6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021907"
---
# <a name="initiator-resource-type"></a><span data-ttu-id="d0596-103">tipo de recurso do iniciador</span><span class="sxs-lookup"><span data-stu-id="d0596-103">initiator resource type</span></span>

<span data-ttu-id="d0596-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0596-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0596-105">Descreve quem ou o que iniciou o evento de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="d0596-105">Describes who or what initiated the provisioning event.</span></span> 

## <a name="properties"></a><span data-ttu-id="d0596-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d0596-106">Properties</span></span>

| <span data-ttu-id="d0596-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0596-107">Property</span></span>     | <span data-ttu-id="d0596-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0596-108">Type</span></span>        | <span data-ttu-id="d0596-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0596-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d0596-110">displayName</span><span class="sxs-lookup"><span data-stu-id="d0596-110">displayName</span></span>|<span data-ttu-id="d0596-111">String</span><span class="sxs-lookup"><span data-stu-id="d0596-111">String</span></span>|<span data-ttu-id="d0596-112">Nome da pessoa ou serviço que iniciou o evento de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="d0596-112">Name of the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="d0596-113">id</span><span class="sxs-lookup"><span data-stu-id="d0596-113">id</span></span>|<span data-ttu-id="d0596-114">String</span><span class="sxs-lookup"><span data-stu-id="d0596-114">String</span></span>|<span data-ttu-id="d0596-115">Identifica exclusivamente a pessoa ou o serviço que iniciou o evento de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="d0596-115">Uniquely identifies the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="d0596-116">initiatortype</span><span class="sxs-lookup"><span data-stu-id="d0596-116">initiatorType</span></span>|<span data-ttu-id="d0596-117">String</span><span class="sxs-lookup"><span data-stu-id="d0596-117">String</span></span>| <span data-ttu-id="d0596-118">Tipo de iniciador.</span><span class="sxs-lookup"><span data-stu-id="d0596-118">Type of initiator.</span></span> <span data-ttu-id="d0596-119">Os valores possíveis são: `user`, `app`, `system`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d0596-119">Possible values are: `user`, `app`, `system`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d0596-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d0596-120">JSON representation</span></span>

<span data-ttu-id="d0596-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d0596-121">The following is a JSON representation of the resource.</span></span>

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


