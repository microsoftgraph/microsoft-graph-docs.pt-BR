---
title: tipo de recurso provisionedIdentity
description: Descreve a identidade associada ao evento de resumo do objeto de provisionamento.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5fde45d8e9baf28fddfe9935d71689d24059dfa3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43371392"
---
# <a name="provisionedidentity-resource-type"></a><span data-ttu-id="898ca-103">tipo de recurso provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="898ca-103">provisionedIdentity resource type</span></span>

<span data-ttu-id="898ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="898ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="898ca-105">Descreve a identidade associada ao evento de resumo do objeto de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="898ca-105">Describes the identity associated with the provisioning object summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="898ca-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="898ca-106">Properties</span></span>

| <span data-ttu-id="898ca-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="898ca-107">Property</span></span>     | <span data-ttu-id="898ca-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="898ca-108">Type</span></span>        | <span data-ttu-id="898ca-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="898ca-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="898ca-110">detalhes</span><span class="sxs-lookup"><span data-stu-id="898ca-110">details</span></span>|[<span data-ttu-id="898ca-111">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="898ca-111">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="898ca-112">Detalhes da identidade.</span><span class="sxs-lookup"><span data-stu-id="898ca-112">Details of the identity.</span></span>|
|<span data-ttu-id="898ca-113">displayName</span><span class="sxs-lookup"><span data-stu-id="898ca-113">displayName</span></span>|<span data-ttu-id="898ca-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="898ca-114">String</span></span>|<span data-ttu-id="898ca-115">Nome para exibição da identidade.</span><span class="sxs-lookup"><span data-stu-id="898ca-115">Display name of the identity.</span></span> |
|<span data-ttu-id="898ca-116">id</span><span class="sxs-lookup"><span data-stu-id="898ca-116">id</span></span>|<span data-ttu-id="898ca-117">String</span><span class="sxs-lookup"><span data-stu-id="898ca-117">String</span></span>|<span data-ttu-id="898ca-118">Identifica exclusivamente a identidade.</span><span class="sxs-lookup"><span data-stu-id="898ca-118">Uniquely identifies the identity.</span></span>|
|<span data-ttu-id="898ca-119">IdentityType</span><span class="sxs-lookup"><span data-stu-id="898ca-119">identityType</span></span>|<span data-ttu-id="898ca-120">String</span><span class="sxs-lookup"><span data-stu-id="898ca-120">String</span></span>|<span data-ttu-id="898ca-121">Tipo de identidade que foi provisionado, como ' usuário ' ou ' grupo '.</span><span class="sxs-lookup"><span data-stu-id="898ca-121">Type of identity that has been provisioned, such as 'user' or 'group'.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="898ca-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="898ca-122">JSON representation</span></span>

<span data-ttu-id="898ca-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="898ca-123">The following is a JSON representation of the resource.</span></span>

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
