---
title: tipo de recurso do iniciador
description: Descreve quem ou o que iniciou o evento de provisionamento.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2846c247d4a0d196d4c620f447b40d47cd486c81
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349334"
---
# <a name="initiator-resource-type"></a><span data-ttu-id="9221b-103">tipo de recurso do iniciador</span><span class="sxs-lookup"><span data-stu-id="9221b-103">initiator resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9221b-104">Descreve quem ou o que iniciou o evento de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="9221b-104">Describes who or what initiated the provisioning event.</span></span> 

## <a name="properties"></a><span data-ttu-id="9221b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9221b-105">Properties</span></span>

| <span data-ttu-id="9221b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9221b-106">Property</span></span>     | <span data-ttu-id="9221b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="9221b-107">Type</span></span>        | <span data-ttu-id="9221b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9221b-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9221b-109">displayName</span><span class="sxs-lookup"><span data-stu-id="9221b-109">displayName</span></span>|<span data-ttu-id="9221b-110">String</span><span class="sxs-lookup"><span data-stu-id="9221b-110">String</span></span>|<span data-ttu-id="9221b-111">Nome da pessoa ou serviço que iniciou o evento de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="9221b-111">Name of the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="9221b-112">id</span><span class="sxs-lookup"><span data-stu-id="9221b-112">id</span></span>|<span data-ttu-id="9221b-113">String</span><span class="sxs-lookup"><span data-stu-id="9221b-113">String</span></span>|<span data-ttu-id="9221b-114">Identifica exclusivamente a pessoa ou o serviço que iniciou o evento de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="9221b-114">Uniquely identifies the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="9221b-115">initiatortype</span><span class="sxs-lookup"><span data-stu-id="9221b-115">initiatorType</span></span>|<span data-ttu-id="9221b-116">String</span><span class="sxs-lookup"><span data-stu-id="9221b-116">String</span></span>| <span data-ttu-id="9221b-117">Tipo de iniciador.</span><span class="sxs-lookup"><span data-stu-id="9221b-117">Type of initiator.</span></span> <span data-ttu-id="9221b-118">Os valores possíveis são: `user`, `app`, `system`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="9221b-118">Possible values are: `user`, `app`, `system`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9221b-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9221b-119">JSON representation</span></span>

<span data-ttu-id="9221b-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9221b-120">The following is a JSON representation of the resource.</span></span>

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
