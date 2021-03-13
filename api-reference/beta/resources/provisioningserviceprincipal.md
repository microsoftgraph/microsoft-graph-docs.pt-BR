---
title: Tipo de recurso provisioningServicePrincipal
description: Representa a entidade de serviço usada para provisionamento.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 5af9dc46de889eea780ca45eb25463ffafcf1260
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760992"
---
# <a name="provisioningserviceprincipal-resource-type"></a><span data-ttu-id="39b19-103">Tipo de recurso provisioningServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="39b19-103">provisioningServicePrincipal resource type</span></span>

<span data-ttu-id="39b19-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39b19-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39b19-105">Representa a entidade de serviço usada para provisionamento.</span><span class="sxs-lookup"><span data-stu-id="39b19-105">Represents the service principal used for provisioning.</span></span> 

## <a name="properties"></a><span data-ttu-id="39b19-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="39b19-106">Properties</span></span>

| <span data-ttu-id="39b19-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39b19-107">Property</span></span>     | <span data-ttu-id="39b19-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="39b19-108">Type</span></span>        | <span data-ttu-id="39b19-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="39b19-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="39b19-110">id</span><span class="sxs-lookup"><span data-stu-id="39b19-110">id</span></span>|<span data-ttu-id="39b19-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39b19-111">String</span></span>|<span data-ttu-id="39b19-112">Identifica exclusivamente o **servicePrincipal** usado para provisionamento.</span><span class="sxs-lookup"><span data-stu-id="39b19-112">Uniquely identifies the **servicePrincipal** used for provisioning.</span></span>|
|<span data-ttu-id="39b19-113">nome</span><span class="sxs-lookup"><span data-stu-id="39b19-113">name</span></span>|<span data-ttu-id="39b19-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39b19-114">String</span></span>| <span data-ttu-id="39b19-115">Nome definido pelo cliente para **o servicePrincipal**.</span><span class="sxs-lookup"><span data-stu-id="39b19-115">Customer-defined name for the **servicePrincipal**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="39b19-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="39b19-116">JSON representation</span></span>

<span data-ttu-id="39b19-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="39b19-117">The following is a JSON representation of the resource.</span></span>

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


