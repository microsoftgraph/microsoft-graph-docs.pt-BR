---
title: tipo de recurso provisioningServicePrincipal
description: Representa a entidade de serviço usada para provisionamento.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e163be94269ee6a75f148b460f728a36e8945645
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446573"
---
# <a name="provisioningserviceprincipal-resource-type"></a><span data-ttu-id="1eecb-103">tipo de recurso provisioningServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="1eecb-103">provisioningServicePrincipal resource type</span></span>

<span data-ttu-id="1eecb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1eecb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1eecb-105">Representa a entidade de serviço usada para provisionamento.</span><span class="sxs-lookup"><span data-stu-id="1eecb-105">Represents the service principal used for provisioning.</span></span> 

## <a name="properties"></a><span data-ttu-id="1eecb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1eecb-106">Properties</span></span>

| <span data-ttu-id="1eecb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1eecb-107">Property</span></span>     | <span data-ttu-id="1eecb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1eecb-108">Type</span></span>        | <span data-ttu-id="1eecb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1eecb-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1eecb-110">id</span><span class="sxs-lookup"><span data-stu-id="1eecb-110">id</span></span>|<span data-ttu-id="1eecb-111">String</span><span class="sxs-lookup"><span data-stu-id="1eecb-111">String</span></span>|<span data-ttu-id="1eecb-112">Identifica exclusivamente o **servicePrincipalName** usado para provisionamento.</span><span class="sxs-lookup"><span data-stu-id="1eecb-112">Uniquely identifies the **servicePrincipal** used for provisioning.</span></span>|
|<span data-ttu-id="1eecb-113">nome</span><span class="sxs-lookup"><span data-stu-id="1eecb-113">name</span></span>|<span data-ttu-id="1eecb-114">String</span><span class="sxs-lookup"><span data-stu-id="1eecb-114">String</span></span>| <span data-ttu-id="1eecb-115">Nome definido pelo cliente para o **servicePrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="1eecb-115">Customer-defined name for the **servicePrincipal**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1eecb-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1eecb-116">JSON representation</span></span>

<span data-ttu-id="1eecb-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1eecb-117">The following is a JSON representation of the resource.</span></span>

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
