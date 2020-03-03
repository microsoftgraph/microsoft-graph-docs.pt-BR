---
title: tipo de recurso provisioningServicePrincipal
description: Representa a entidade de serviço usada para provisionamento.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 59dd514ff818ee37b462d8f21f3dce02d213eb20
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394651"
---
# <a name="provisioningserviceprincipal-resource-type"></a><span data-ttu-id="c624b-103">tipo de recurso provisioningServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="c624b-103">provisioningServicePrincipal resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c624b-104">Representa a entidade de serviço usada para provisionamento.</span><span class="sxs-lookup"><span data-stu-id="c624b-104">Represents the service principal used for provisioning.</span></span> 

## <a name="properties"></a><span data-ttu-id="c624b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c624b-105">Properties</span></span>

| <span data-ttu-id="c624b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c624b-106">Property</span></span>     | <span data-ttu-id="c624b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c624b-107">Type</span></span>        | <span data-ttu-id="c624b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c624b-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c624b-109">id</span><span class="sxs-lookup"><span data-stu-id="c624b-109">id</span></span>|<span data-ttu-id="c624b-110">String</span><span class="sxs-lookup"><span data-stu-id="c624b-110">String</span></span>|<span data-ttu-id="c624b-111">Identifica exclusivamente o **servicePrincipalName** usado para provisionamento.</span><span class="sxs-lookup"><span data-stu-id="c624b-111">Uniquely identifies the **servicePrincipal** used for provisioning.</span></span>|
|<span data-ttu-id="c624b-112">nome</span><span class="sxs-lookup"><span data-stu-id="c624b-112">name</span></span>|<span data-ttu-id="c624b-113">String</span><span class="sxs-lookup"><span data-stu-id="c624b-113">String</span></span>| <span data-ttu-id="c624b-114">Nome definido pelo cliente para o **servicePrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="c624b-114">Customer-defined name for the **servicePrincipal**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c624b-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c624b-115">JSON representation</span></span>

<span data-ttu-id="c624b-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c624b-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningServicePrincipal",
  "baseType": null
}-->

```json
{
  "id": "String",
  "name": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
