---
title: Tipo de recurso provisioningSystem
description: Representa o sistema de onde um usuário foi provisionado.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 2dcc52e4b847648477313d61c8b69b168a8807b1
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232900"
---
# <a name="provisioningsystem-resource-type"></a><span data-ttu-id="a595f-103">Tipo de recurso provisioningSystem</span><span class="sxs-lookup"><span data-stu-id="a595f-103">provisioningSystem resource type</span></span>

<span data-ttu-id="a595f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a595f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a595f-105">Representa o sistema de onde um usuário foi provisionado.</span><span class="sxs-lookup"><span data-stu-id="a595f-105">Represents the system that a user was provisioned to or from.</span></span> <span data-ttu-id="a595f-106">Por exemplo, ao provisionar um usuário do Azure Active Directory (Azure AD) para ServiceNow, o sistema de origem é o Azure AD e o sistema de destino é ServiceNow.</span><span class="sxs-lookup"><span data-stu-id="a595f-106">For example, when provisioning a user from Azure Active Directory (Azure AD) to ServiceNow, the source system is Azure AD, and the target system is ServiceNow.</span></span>

## <a name="properties"></a><span data-ttu-id="a595f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a595f-107">Properties</span></span>

| <span data-ttu-id="a595f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a595f-108">Property</span></span>     | <span data-ttu-id="a595f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a595f-109">Type</span></span>        | <span data-ttu-id="a595f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a595f-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a595f-111">detalhes</span><span class="sxs-lookup"><span data-stu-id="a595f-111">details</span></span>|[<span data-ttu-id="a595f-112">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="a595f-112">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="a595f-113">Detalhes do sistema.</span><span class="sxs-lookup"><span data-stu-id="a595f-113">Details of the system.</span></span>|
|<span data-ttu-id="a595f-114">displayName</span><span class="sxs-lookup"><span data-stu-id="a595f-114">displayName</span></span>|<span data-ttu-id="a595f-115">String</span><span class="sxs-lookup"><span data-stu-id="a595f-115">String</span></span>|<span data-ttu-id="a595f-116">Nome do sistema de onde um usuário foi provisionado.</span><span class="sxs-lookup"><span data-stu-id="a595f-116">Name of the system that a user was provisioned to or from.</span></span>|
|<span data-ttu-id="a595f-117">id</span><span class="sxs-lookup"><span data-stu-id="a595f-117">id</span></span>|<span data-ttu-id="a595f-118">String</span><span class="sxs-lookup"><span data-stu-id="a595f-118">String</span></span>|<span data-ttu-id="a595f-119">Identificador do sistema de onde um usuário foi provisionado.</span><span class="sxs-lookup"><span data-stu-id="a595f-119">Identifier of the system that a user was provisioned to or from.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a595f-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a595f-120">JSON representation</span></span>

<span data-ttu-id="a595f-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a595f-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningSystem",
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
  "description": "provisioningSystem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


