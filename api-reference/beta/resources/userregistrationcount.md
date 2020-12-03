---
title: tipo de recurso userRegistrationCount
description: Representa a contagem de registro e o status de usuários em seu locatário.
localization_priority: Normal
author: besiler
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 3e3a5e7e3925f5528d5ce73a15233cea8e50eebd
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524180"
---
# <a name="userregistrationcount-resource-type"></a><span data-ttu-id="7d0c6-103">tipo de recurso userRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="7d0c6-103">userRegistrationCount resource type</span></span>

<span data-ttu-id="7d0c6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d0c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d0c6-105">Representa a contagem de registro e o status de usuários em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="7d0c6-105">Represents the registration count and status for users in your tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="7d0c6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7d0c6-106">Properties</span></span>

| <span data-ttu-id="7d0c6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d0c6-107">Property</span></span>     | <span data-ttu-id="7d0c6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d0c6-108">Type</span></span>        | <span data-ttu-id="7d0c6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d0c6-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7d0c6-110">registrationCount</span><span class="sxs-lookup"><span data-stu-id="7d0c6-110">registrationCount</span></span> | <span data-ttu-id="7d0c6-111">Int64</span><span class="sxs-lookup"><span data-stu-id="7d0c6-111">Int64</span></span> | <span data-ttu-id="7d0c6-112">Fornece a contagem de registro para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="7d0c6-112">Provides the registration count for your tenant.</span></span> |
| <span data-ttu-id="7d0c6-113">registrationStatus</span><span class="sxs-lookup"><span data-stu-id="7d0c6-113">registrationStatus</span></span> | <span data-ttu-id="7d0c6-114">String</span><span class="sxs-lookup"><span data-stu-id="7d0c6-114">String</span></span> | <span data-ttu-id="7d0c6-115">Representa o status do registro do usuário.</span><span class="sxs-lookup"><span data-stu-id="7d0c6-115">Represents the status of user registration.</span></span> <span data-ttu-id="7d0c6-116">Os valores possíveis são: `registered` , `enabled` , `capable` , e `mfaRegistered` .</span><span class="sxs-lookup"><span data-stu-id="7d0c6-116">Possible values are: `registered`, `enabled`, `capable`, and `mfaRegistered`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7d0c6-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7d0c6-117">JSON representation</span></span>

<span data-ttu-id="7d0c6-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7d0c6-118">The following is a JSON representation of the resource.</span></span>

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

