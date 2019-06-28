---
title: tipo de recurso provisioningSystemDetails
description: Representa o sistema do qual um usuário foi provisionado ou de.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e84af77ac7d2b14fb25ce07939bc1a542102fb19
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349327"
---
# <a name="provisioningsystemdetails-resource-type"></a><span data-ttu-id="59cf8-103">tipo de recurso provisioningSystemDetails</span><span class="sxs-lookup"><span data-stu-id="59cf8-103">provisioningSystemDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59cf8-104">Representa o sistema do qual um usuário foi provisionado ou de.</span><span class="sxs-lookup"><span data-stu-id="59cf8-104">Represents the system that a user was provisioned to or from.</span></span> <span data-ttu-id="59cf8-105">Por exemplo, ao provisionar um usuário do Azure Active Directory (Azure AD) para o ServiceNow, o sistema de origem é o Azure AD e o sistema de destino é o ServiceNow.</span><span class="sxs-lookup"><span data-stu-id="59cf8-105">For example, when provisioning a user from Azure Active Directory (Azure AD) to ServiceNow, the source system is Azure AD, and the target system is ServiceNow.</span></span>

## <a name="properties"></a><span data-ttu-id="59cf8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="59cf8-106">Properties</span></span>

| <span data-ttu-id="59cf8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59cf8-107">Property</span></span>     | <span data-ttu-id="59cf8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="59cf8-108">Type</span></span>        | <span data-ttu-id="59cf8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="59cf8-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="59cf8-110">detalhes</span><span class="sxs-lookup"><span data-stu-id="59cf8-110">details</span></span>|[<span data-ttu-id="59cf8-111">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="59cf8-111">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="59cf8-112">Detalhes do sistema.</span><span class="sxs-lookup"><span data-stu-id="59cf8-112">Details of the system.</span></span>|
|<span data-ttu-id="59cf8-113">displayName</span><span class="sxs-lookup"><span data-stu-id="59cf8-113">displayName</span></span>|<span data-ttu-id="59cf8-114">String</span><span class="sxs-lookup"><span data-stu-id="59cf8-114">String</span></span>|<span data-ttu-id="59cf8-115">Nome do sistema no qual um usuário foi provisionado ou de.</span><span class="sxs-lookup"><span data-stu-id="59cf8-115">Name of the system that a user was provisioned to or from.</span></span>|
|<span data-ttu-id="59cf8-116">id</span><span class="sxs-lookup"><span data-stu-id="59cf8-116">id</span></span>|<span data-ttu-id="59cf8-117">String</span><span class="sxs-lookup"><span data-stu-id="59cf8-117">String</span></span>|<span data-ttu-id="59cf8-118">Identificador do sistema no qual um usuário foi provisionado ou de.</span><span class="sxs-lookup"><span data-stu-id="59cf8-118">Identifier of the system that a user was provisioned to or from.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="59cf8-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="59cf8-119">JSON representation</span></span>

<span data-ttu-id="59cf8-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="59cf8-120">The following is a JSON representation of the resource.</span></span>

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
