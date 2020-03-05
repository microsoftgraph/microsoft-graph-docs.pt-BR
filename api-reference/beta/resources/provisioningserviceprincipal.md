---
title: tipo de recurso provisioningServicePrincipal
description: Representa a entidade de serviço usada para provisionamento.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fde8f4d41c7e2788c306fe0e0591b9ddb8ba031d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521331"
---
# <a name="provisioningserviceprincipal-resource-type"></a><span data-ttu-id="b9fcd-103">tipo de recurso provisioningServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="b9fcd-103">provisioningServicePrincipal resource type</span></span>

<span data-ttu-id="b9fcd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b9fcd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9fcd-105">Representa a entidade de serviço usada para provisionamento.</span><span class="sxs-lookup"><span data-stu-id="b9fcd-105">Represents the service principal used for provisioning.</span></span> 

## <a name="properties"></a><span data-ttu-id="b9fcd-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9fcd-106">Properties</span></span>

| <span data-ttu-id="b9fcd-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9fcd-107">Property</span></span>     | <span data-ttu-id="b9fcd-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9fcd-108">Type</span></span>        | <span data-ttu-id="b9fcd-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9fcd-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b9fcd-110">id</span><span class="sxs-lookup"><span data-stu-id="b9fcd-110">id</span></span>|<span data-ttu-id="b9fcd-111">String</span><span class="sxs-lookup"><span data-stu-id="b9fcd-111">String</span></span>|<span data-ttu-id="b9fcd-112">Identifica exclusivamente o **servicePrincipalName** usado para provisionamento.</span><span class="sxs-lookup"><span data-stu-id="b9fcd-112">Uniquely identifies the **servicePrincipal** used for provisioning.</span></span>|
|<span data-ttu-id="b9fcd-113">nome</span><span class="sxs-lookup"><span data-stu-id="b9fcd-113">name</span></span>|<span data-ttu-id="b9fcd-114">String</span><span class="sxs-lookup"><span data-stu-id="b9fcd-114">String</span></span>| <span data-ttu-id="b9fcd-115">Nome definido pelo cliente para o **servicePrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="b9fcd-115">Customer-defined name for the **servicePrincipal**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b9fcd-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9fcd-116">JSON representation</span></span>

<span data-ttu-id="b9fcd-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b9fcd-117">The following is a JSON representation of the resource.</span></span>

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
