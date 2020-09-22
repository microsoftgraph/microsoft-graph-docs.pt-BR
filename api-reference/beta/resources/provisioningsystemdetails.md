---
title: tipo de recurso provisioningSystemDetails
description: Representa o sistema do qual um usuário foi provisionado ou de.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6880214614047000fcc5a793faf4be3e5a88a5e6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026443"
---
# <a name="provisioningsystemdetails-resource-type"></a><span data-ttu-id="c2696-103">tipo de recurso provisioningSystemDetails</span><span class="sxs-lookup"><span data-stu-id="c2696-103">provisioningSystemDetails resource type</span></span>

<span data-ttu-id="c2696-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2696-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2696-105">Representa o sistema do qual um usuário foi provisionado ou de.</span><span class="sxs-lookup"><span data-stu-id="c2696-105">Represents the system that a user was provisioned to or from.</span></span> <span data-ttu-id="c2696-106">Por exemplo, ao provisionar um usuário do Azure Active Directory (Azure AD) para o ServiceNow, o sistema de origem é o Azure AD e o sistema de destino é o ServiceNow.</span><span class="sxs-lookup"><span data-stu-id="c2696-106">For example, when provisioning a user from Azure Active Directory (Azure AD) to ServiceNow, the source system is Azure AD, and the target system is ServiceNow.</span></span>

## <a name="properties"></a><span data-ttu-id="c2696-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c2696-107">Properties</span></span>

| <span data-ttu-id="c2696-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c2696-108">Property</span></span>     | <span data-ttu-id="c2696-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2696-109">Type</span></span>        | <span data-ttu-id="c2696-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2696-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c2696-111">detalhes</span><span class="sxs-lookup"><span data-stu-id="c2696-111">details</span></span>|[<span data-ttu-id="c2696-112">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="c2696-112">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="c2696-113">Detalhes do sistema.</span><span class="sxs-lookup"><span data-stu-id="c2696-113">Details of the system.</span></span>|
|<span data-ttu-id="c2696-114">displayName</span><span class="sxs-lookup"><span data-stu-id="c2696-114">displayName</span></span>|<span data-ttu-id="c2696-115">String</span><span class="sxs-lookup"><span data-stu-id="c2696-115">String</span></span>|<span data-ttu-id="c2696-116">Nome do sistema no qual um usuário foi provisionado ou de.</span><span class="sxs-lookup"><span data-stu-id="c2696-116">Name of the system that a user was provisioned to or from.</span></span>|
|<span data-ttu-id="c2696-117">id</span><span class="sxs-lookup"><span data-stu-id="c2696-117">id</span></span>|<span data-ttu-id="c2696-118">String</span><span class="sxs-lookup"><span data-stu-id="c2696-118">String</span></span>|<span data-ttu-id="c2696-119">Identificador do sistema no qual um usuário foi provisionado ou de.</span><span class="sxs-lookup"><span data-stu-id="c2696-119">Identifier of the system that a user was provisioned to or from.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c2696-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c2696-120">JSON representation</span></span>

<span data-ttu-id="c2696-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c2696-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningSystemDetails",
  "baseType": null
}-->

```json
{
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "displayName": "String",
  "id": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningSystemDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


