---
title: Tipo de recurso provisioningSystemDetails
description: Representa o sistema de onde um usuário foi provisionado.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 5400088c1f239bd73e093679bbc13b8034800f28
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135335"
---
# <a name="provisioningsystemdetails-resource-type"></a><span data-ttu-id="edc58-103">Tipo de recurso provisioningSystemDetails</span><span class="sxs-lookup"><span data-stu-id="edc58-103">provisioningSystemDetails resource type</span></span>

<span data-ttu-id="edc58-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edc58-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edc58-105">Representa o sistema de onde um usuário foi provisionado.</span><span class="sxs-lookup"><span data-stu-id="edc58-105">Represents the system that a user was provisioned to or from.</span></span> <span data-ttu-id="edc58-106">Por exemplo, ao provisionar um usuário do Azure Active Directory (Azure AD) para o ServiceNow, o sistema de origem é o Azure AD e o sistema de destino é o ServiceNow.</span><span class="sxs-lookup"><span data-stu-id="edc58-106">For example, when provisioning a user from Azure Active Directory (Azure AD) to ServiceNow, the source system is Azure AD, and the target system is ServiceNow.</span></span>

## <a name="properties"></a><span data-ttu-id="edc58-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="edc58-107">Properties</span></span>

| <span data-ttu-id="edc58-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="edc58-108">Property</span></span>     | <span data-ttu-id="edc58-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="edc58-109">Type</span></span>        | <span data-ttu-id="edc58-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="edc58-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="edc58-111">detalhes</span><span class="sxs-lookup"><span data-stu-id="edc58-111">details</span></span>|[<span data-ttu-id="edc58-112">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="edc58-112">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="edc58-113">Detalhes do sistema.</span><span class="sxs-lookup"><span data-stu-id="edc58-113">Details of the system.</span></span>|
|<span data-ttu-id="edc58-114">displayName</span><span class="sxs-lookup"><span data-stu-id="edc58-114">displayName</span></span>|<span data-ttu-id="edc58-115">String</span><span class="sxs-lookup"><span data-stu-id="edc58-115">String</span></span>|<span data-ttu-id="edc58-116">Nome do sistema de onde um usuário foi provisionado.</span><span class="sxs-lookup"><span data-stu-id="edc58-116">Name of the system that a user was provisioned to or from.</span></span>|
|<span data-ttu-id="edc58-117">id</span><span class="sxs-lookup"><span data-stu-id="edc58-117">id</span></span>|<span data-ttu-id="edc58-118">String</span><span class="sxs-lookup"><span data-stu-id="edc58-118">String</span></span>|<span data-ttu-id="edc58-119">Identificador do sistema de onde um usuário foi provisionado.</span><span class="sxs-lookup"><span data-stu-id="edc58-119">Identifier of the system that a user was provisioned to or from.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="edc58-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="edc58-120">JSON representation</span></span>

<span data-ttu-id="edc58-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="edc58-121">The following is a JSON representation of the resource.</span></span>

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


