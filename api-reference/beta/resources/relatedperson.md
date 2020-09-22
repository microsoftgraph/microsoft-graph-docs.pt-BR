---
title: tipo de recurso relatedPerson
description: tipo de recurso relatedPerson
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 88d7283d1eac1f3b7bcc7d947fa1961494a58041
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033570"
---
# <a name="relatedperson-resource-type"></a><span data-ttu-id="f6d8f-103">tipo de recurso relatedPerson</span><span class="sxs-lookup"><span data-stu-id="f6d8f-103">relatedPerson resource type</span></span>

<span data-ttu-id="f6d8f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6d8f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6d8f-105">Representa informações sobre as pessoas relacionadas às informações de uma determinada entidade em um [perfil](profile.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f6d8f-105">Represents information about people related to information within a given entity in a [profile](profile.md) for a user.</span></span>

## <a name="properties"></a><span data-ttu-id="f6d8f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f6d8f-106">Properties</span></span>

| <span data-ttu-id="f6d8f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f6d8f-107">Property</span></span>        | <span data-ttu-id="f6d8f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6d8f-108">Type</span></span>        | <span data-ttu-id="f6d8f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6d8f-109">Description</span></span>                                                                                                                                                                                                                                     |
|:----------------|:------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="f6d8f-110">displayName</span><span class="sxs-lookup"><span data-stu-id="f6d8f-110">displayName</span></span>      |<span data-ttu-id="f6d8f-111">String</span><span class="sxs-lookup"><span data-stu-id="f6d8f-111">String</span></span>       | <span data-ttu-id="f6d8f-112">Nome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="f6d8f-112">Name of the person.</span></span>                                                                                                                                                                                                                             |
|<span data-ttu-id="f6d8f-113">relação</span><span class="sxs-lookup"><span data-stu-id="f6d8f-113">relationship</span></span>     |<span data-ttu-id="f6d8f-114">String</span><span class="sxs-lookup"><span data-stu-id="f6d8f-114">String</span></span>       | <span data-ttu-id="f6d8f-115">Os valores possíveis são: `manager`, `colleague`, `directReport`, `dotLineReport`, `assistant`, `dotLineManager`, `alternateContact`, `friend`, `spouse`, `sibling`, `child`, `parent`, `sponsor`, `emergencyContact`, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f6d8f-115">Possible values are: `manager`, `colleague`, `directReport`, `dotLineReport`, `assistant`, `dotLineManager`, `alternateContact`, `friend`, `spouse`, `sibling`, `child`, `parent`, `sponsor`, `emergencyContact`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="f6d8f-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f6d8f-116">userPrincipalName</span></span>|<span data-ttu-id="f6d8f-117">String</span><span class="sxs-lookup"><span data-stu-id="f6d8f-117">String</span></span>       | <span data-ttu-id="f6d8f-118">Endereço de email ou referência a uma pessoa na organização.</span><span class="sxs-lookup"><span data-stu-id="f6d8f-118">Email address or reference to person within organization.</span></span>                                                                                                                                                                                       |

## <a name="json-representation"></a><span data-ttu-id="f6d8f-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f6d8f-119">JSON representation</span></span>

<span data-ttu-id="f6d8f-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f6d8f-120">The following is a JSON representation of the resource.</span></span>

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


