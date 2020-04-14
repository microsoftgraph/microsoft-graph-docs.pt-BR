---
title: tipo de recurso userRegistrationCount
description: Representa a contagem de registro e o status de usuários em seu locatário.
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: e322f073655ffaa975464d666a365410138f6e51
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43384976"
---
# <a name="userregistrationcount-resource-type"></a><span data-ttu-id="12770-103">tipo de recurso userRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="12770-103">userRegistrationCount resource type</span></span>

<span data-ttu-id="12770-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12770-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12770-105">Representa a contagem de registro e o status de usuários em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="12770-105">Represents the registration count and status for users in your tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="12770-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12770-106">Properties</span></span>

| <span data-ttu-id="12770-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12770-107">Property</span></span>     | <span data-ttu-id="12770-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="12770-108">Type</span></span>        | <span data-ttu-id="12770-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="12770-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="12770-110">registrationCount</span><span class="sxs-lookup"><span data-stu-id="12770-110">registrationCount</span></span> | <span data-ttu-id="12770-111">Int64</span><span class="sxs-lookup"><span data-stu-id="12770-111">Int64</span></span> | <span data-ttu-id="12770-112">Fornece a contagem de registro para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="12770-112">Provides the registration count for your tenant.</span></span> |
| <span data-ttu-id="12770-113">registrationStatus</span><span class="sxs-lookup"><span data-stu-id="12770-113">registrationStatus</span></span> | <span data-ttu-id="12770-114">String</span><span class="sxs-lookup"><span data-stu-id="12770-114">String</span></span> | <span data-ttu-id="12770-115">Representa o status do registro do usuário.</span><span class="sxs-lookup"><span data-stu-id="12770-115">Represents the status of user registration.</span></span> <span data-ttu-id="12770-116">Os valores possíveis são `registered`: `enabled`, `capable`,, `mfaRegistered`e.</span><span class="sxs-lookup"><span data-stu-id="12770-116">Possible values are: `registered`, `enabled`, `capable`, and `mfaRegistered`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="12770-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12770-117">JSON representation</span></span>

<span data-ttu-id="12770-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="12770-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userRegistrationCount",
  "baseType": null
}-->

```json
{ 
  "registrationStatus":"String", 
  "registrationCount": 23423
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userRegistrationCount resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->