---
title: tipo de recurso relatedPerson
description: tipo de recurso relatedPerson
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 6be6300bc901305fb87b04e2482f145b9187f9fb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939233"
---
# <a name="relatedperson-resource-type"></a><span data-ttu-id="eba0d-103">tipo de recurso relatedPerson</span><span class="sxs-lookup"><span data-stu-id="eba0d-103">relatedPerson resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eba0d-104">Representa informações sobre as pessoas relacionadas às informações de uma determinada entidade em um [perfil](profile.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="eba0d-104">Represents information about people related to information within a given entity in a [profile](profile.md) for a user.</span></span>

## <a name="properties"></a><span data-ttu-id="eba0d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eba0d-105">Properties</span></span>

| <span data-ttu-id="eba0d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eba0d-106">Property</span></span>        | <span data-ttu-id="eba0d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="eba0d-107">Type</span></span>        | <span data-ttu-id="eba0d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="eba0d-108">Description</span></span>                                               |
|:----------------|:------------|:----------------------------------------------------------|
|<span data-ttu-id="eba0d-109">displayName</span><span class="sxs-lookup"><span data-stu-id="eba0d-109">displayName</span></span>      |<span data-ttu-id="eba0d-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eba0d-110">String</span></span>       | <span data-ttu-id="eba0d-111">Nome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="eba0d-111">Name of the person.</span></span>                                        |
|<span data-ttu-id="eba0d-112">relação</span><span class="sxs-lookup"><span data-stu-id="eba0d-112">relationship</span></span>     |<span data-ttu-id="eba0d-113">String</span><span class="sxs-lookup"><span data-stu-id="eba0d-113">String</span></span>       | <span data-ttu-id="eba0d-114">Os valores possíveis são: `manager`, `colleague`, `directReport`, `dotLineReport`, `assistant`, `dotLineManager`, `alternateContact`, `friend`, `spouse`, `sibling`, `child`, `parent`, `sponsor`, `emergencyContact`, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="eba0d-114">Possible values are: `manager`, `colleague`, `directReport`, `dotLineReport`, `assistant`, `dotLineManager`, `alternateContact`, `friend`, `spouse`, `sibling`, `child`, `parent`, `sponsor`, `emergencyContact`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="eba0d-115">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="eba0d-115">userPrincipalName</span></span>|<span data-ttu-id="eba0d-116">String</span><span class="sxs-lookup"><span data-stu-id="eba0d-116">String</span></span>       | <span data-ttu-id="eba0d-117">Endereço de email ou referência a uma pessoa na organização.</span><span class="sxs-lookup"><span data-stu-id="eba0d-117">Email address or reference to person within organization.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eba0d-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eba0d-118">JSON representation</span></span>

<span data-ttu-id="eba0d-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eba0d-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relatedPerson",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "relationship": "String",
  "userPrincipalName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "relatedPerson resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
