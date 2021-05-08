---
title: Tipo de recurso provisioningSystem
description: Representa o sistema de onde um usuário foi provisionado.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: d52429fbaa641b1ee0be5208ddf7d85e0830b6c6
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241477"
---
# <a name="provisioningsystem-resource-type"></a><span data-ttu-id="061c6-103">Tipo de recurso provisioningSystem</span><span class="sxs-lookup"><span data-stu-id="061c6-103">provisioningSystem resource type</span></span>

<span data-ttu-id="061c6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="061c6-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="061c6-105">Representa o sistema de onde um usuário foi provisionado.</span><span class="sxs-lookup"><span data-stu-id="061c6-105">Represents the system that a user was provisioned to or from.</span></span> <span data-ttu-id="061c6-106">Por exemplo, ao provisionar um usuário do Azure Active Directory (Azure AD) para ServiceNow, o sistema de origem é o Azure AD e o sistema de destino é ServiceNow.</span><span class="sxs-lookup"><span data-stu-id="061c6-106">For example, when provisioning a user from Azure Active Directory (Azure AD) to ServiceNow, the source system is Azure AD, and the target system is ServiceNow.</span></span>

## <a name="properties"></a><span data-ttu-id="061c6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="061c6-107">Properties</span></span>

| <span data-ttu-id="061c6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="061c6-108">Property</span></span>     | <span data-ttu-id="061c6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="061c6-109">Type</span></span>        | <span data-ttu-id="061c6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="061c6-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="061c6-111">detalhes</span><span class="sxs-lookup"><span data-stu-id="061c6-111">details</span></span>|[<span data-ttu-id="061c6-112">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="061c6-112">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="061c6-113">Detalhes do sistema.</span><span class="sxs-lookup"><span data-stu-id="061c6-113">Details of the system.</span></span>|
|<span data-ttu-id="061c6-114">displayName</span><span class="sxs-lookup"><span data-stu-id="061c6-114">displayName</span></span>|<span data-ttu-id="061c6-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="061c6-115">String</span></span>|<span data-ttu-id="061c6-116">Nome do sistema de onde um usuário foi provisionado.</span><span class="sxs-lookup"><span data-stu-id="061c6-116">Name of the system that a user was provisioned to or from.</span></span>|
|<span data-ttu-id="061c6-117">id</span><span class="sxs-lookup"><span data-stu-id="061c6-117">id</span></span>|<span data-ttu-id="061c6-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="061c6-118">String</span></span>|<span data-ttu-id="061c6-119">Identificador do sistema de onde um usuário foi provisionado.</span><span class="sxs-lookup"><span data-stu-id="061c6-119">Identifier of the system that a user was provisioned to or from.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="061c6-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="061c6-120">JSON representation</span></span>

<span data-ttu-id="061c6-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="061c6-121">The following is a JSON representation of the resource.</span></span>

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


