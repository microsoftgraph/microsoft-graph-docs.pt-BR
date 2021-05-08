---
title: Tipo de recurso iniciador
description: Descreve quem ou o que iniciou o evento de provisionamento.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: f1085b6a9b04ef2ad3cd584ac9e0d4dc6c88f037
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232057"
---
# <a name="initiator-resource-type"></a><span data-ttu-id="b1048-103">Tipo de recurso iniciador</span><span class="sxs-lookup"><span data-stu-id="b1048-103">initiator resource type</span></span>

<span data-ttu-id="b1048-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1048-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1048-105">Descreve quem ou o que iniciou o evento de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="b1048-105">Describes who or what initiated the provisioning event.</span></span> 

## <a name="properties"></a><span data-ttu-id="b1048-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1048-106">Properties</span></span>

| <span data-ttu-id="b1048-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1048-107">Property</span></span>     | <span data-ttu-id="b1048-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1048-108">Type</span></span>        | <span data-ttu-id="b1048-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1048-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b1048-110">displayName</span><span class="sxs-lookup"><span data-stu-id="b1048-110">displayName</span></span>|<span data-ttu-id="b1048-111">String</span><span class="sxs-lookup"><span data-stu-id="b1048-111">String</span></span>|<span data-ttu-id="b1048-112">Nome da pessoa ou serviço que iniciou o evento de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="b1048-112">Name of the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="b1048-113">id</span><span class="sxs-lookup"><span data-stu-id="b1048-113">id</span></span>|<span data-ttu-id="b1048-114">String</span><span class="sxs-lookup"><span data-stu-id="b1048-114">String</span></span>|<span data-ttu-id="b1048-115">Identifica exclusivamente a pessoa ou serviço que iniciou o evento de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="b1048-115">Uniquely identifies the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="b1048-116">initiatorType</span><span class="sxs-lookup"><span data-stu-id="b1048-116">initiatorType</span></span>|<span data-ttu-id="b1048-117">String</span><span class="sxs-lookup"><span data-stu-id="b1048-117">String</span></span>| <span data-ttu-id="b1048-118">Tipo de iniciador.</span><span class="sxs-lookup"><span data-stu-id="b1048-118">Type of initiator.</span></span> <span data-ttu-id="b1048-119">Os valores possíveis são: `user`, `application`, `system`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b1048-119">Possible values are: `user`, `application`, `system`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b1048-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1048-120">JSON representation</span></span>

<span data-ttu-id="b1048-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1048-121">The following is a JSON representation of the resource.</span></span>

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


