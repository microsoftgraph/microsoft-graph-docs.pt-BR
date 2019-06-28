---
title: tipo de recurso provisionedIdentity
description: Descreve a identidade associada ao evento de resumo do objeto de provisionamento.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fb535bbba827f93b597c5e41efb128f2ad610ef2
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349315"
---
# <a name="provisionedidentity-resource-type"></a><span data-ttu-id="8bc52-103">tipo de recurso provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="8bc52-103">provisionedIdentity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bc52-104">Descreve a identidade associada ao evento de resumo do objeto de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="8bc52-104">Describes the identity associated with the provisioning object summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="8bc52-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8bc52-105">Properties</span></span>

| <span data-ttu-id="8bc52-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8bc52-106">Property</span></span>     | <span data-ttu-id="8bc52-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8bc52-107">Type</span></span>        | <span data-ttu-id="8bc52-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bc52-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8bc52-109">detalhes</span><span class="sxs-lookup"><span data-stu-id="8bc52-109">details</span></span>|[<span data-ttu-id="8bc52-110">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="8bc52-110">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="8bc52-111">Detalhes da identidade.</span><span class="sxs-lookup"><span data-stu-id="8bc52-111">Details of the identity.</span></span>|
|<span data-ttu-id="8bc52-112">displayName</span><span class="sxs-lookup"><span data-stu-id="8bc52-112">displayName</span></span>|<span data-ttu-id="8bc52-113">String</span><span class="sxs-lookup"><span data-stu-id="8bc52-113">String</span></span>|<span data-ttu-id="8bc52-114">Nome para exibição da identidade.</span><span class="sxs-lookup"><span data-stu-id="8bc52-114">Display name of the identity.</span></span> |
|<span data-ttu-id="8bc52-115">id</span><span class="sxs-lookup"><span data-stu-id="8bc52-115">id</span></span>|<span data-ttu-id="8bc52-116">String</span><span class="sxs-lookup"><span data-stu-id="8bc52-116">String</span></span>|<span data-ttu-id="8bc52-117">Identifica exclusivamente a identidade.</span><span class="sxs-lookup"><span data-stu-id="8bc52-117">Uniquely identifies the identity.</span></span>|
|<span data-ttu-id="8bc52-118">IdentityType</span><span class="sxs-lookup"><span data-stu-id="8bc52-118">identityType</span></span>|<span data-ttu-id="8bc52-119">String</span><span class="sxs-lookup"><span data-stu-id="8bc52-119">String</span></span>|<span data-ttu-id="8bc52-120">Tipo de identidade que foi provisionado, como ' usuário ' ou ' grupo '.</span><span class="sxs-lookup"><span data-stu-id="8bc52-120">Type of identity that has been provisioned, such as 'user' or 'group'.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8bc52-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8bc52-121">JSON representation</span></span>

<span data-ttu-id="8bc52-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8bc52-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedIdentity",
  "baseType": null
}-->

```json
{
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "displayName": "String",
  "id": "String",
  "identityType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisionedIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
