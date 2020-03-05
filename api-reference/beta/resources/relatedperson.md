---
title: tipo de recurso relatedPerson
description: tipo de recurso relatedPerson
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 507746674f17a7bf8255ccddc53ea14fe2ca5a26
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521177"
---
# <a name="relatedperson-resource-type"></a><span data-ttu-id="4148b-103">tipo de recurso relatedPerson</span><span class="sxs-lookup"><span data-stu-id="4148b-103">relatedPerson resource type</span></span>

<span data-ttu-id="4148b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4148b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4148b-105">Representa informações sobre as pessoas relacionadas às informações de uma determinada entidade em um [perfil](profile.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="4148b-105">Represents information about people related to information within a given entity in a [profile](profile.md) for a user.</span></span>

## <a name="properties"></a><span data-ttu-id="4148b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4148b-106">Properties</span></span>

| <span data-ttu-id="4148b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4148b-107">Property</span></span>        | <span data-ttu-id="4148b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4148b-108">Type</span></span>        | <span data-ttu-id="4148b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4148b-109">Description</span></span>                                               |
|:----------------|:------------|:----------------------------------------------------------|
|<span data-ttu-id="4148b-110">displayName</span><span class="sxs-lookup"><span data-stu-id="4148b-110">displayName</span></span>      |<span data-ttu-id="4148b-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4148b-111">String</span></span>       | <span data-ttu-id="4148b-112">Nome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="4148b-112">Name of the person.</span></span>                                        |
|<span data-ttu-id="4148b-113">relação</span><span class="sxs-lookup"><span data-stu-id="4148b-113">relationship</span></span>     |<span data-ttu-id="4148b-114">String</span><span class="sxs-lookup"><span data-stu-id="4148b-114">String</span></span>       | <span data-ttu-id="4148b-115">Os valores possíveis são: `manager`, `colleague`, `directReport`, `dotLineReport`, `assistant`, `dotLineManager`, `alternateContact`, `friend`, `spouse`, `sibling`, `child`, `parent`, `sponsor`, `emergencyContact`, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="4148b-115">Possible values are: `manager`, `colleague`, `directReport`, `dotLineReport`, `assistant`, `dotLineManager`, `alternateContact`, `friend`, `spouse`, `sibling`, `child`, `parent`, `sponsor`, `emergencyContact`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="4148b-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4148b-116">userPrincipalName</span></span>|<span data-ttu-id="4148b-117">String</span><span class="sxs-lookup"><span data-stu-id="4148b-117">String</span></span>       | <span data-ttu-id="4148b-118">Endereço de email ou referência a uma pessoa na organização.</span><span class="sxs-lookup"><span data-stu-id="4148b-118">Email address or reference to person within organization.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4148b-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4148b-119">JSON representation</span></span>

<span data-ttu-id="4148b-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4148b-120">The following is a JSON representation of the resource.</span></span>

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
