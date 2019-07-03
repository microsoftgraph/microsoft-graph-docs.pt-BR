---
title: tipo de recurso userRegistrationCount
description: Representa a contagem de registro e o status de usuários em seu locatário.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 43f151864f7ca996602e7bd2fc42f3fa4ba743d1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477797"
---
# <a name="userregistrationcount-resource-type"></a><span data-ttu-id="4ac93-103">tipo de recurso userRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="4ac93-103">userRegistrationCount resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ac93-104">Representa a contagem de registro e o status de usuários em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="4ac93-104">Represents the registration count and status for users in your tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="4ac93-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ac93-105">Properties</span></span>

| <span data-ttu-id="4ac93-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ac93-106">Property</span></span>     | <span data-ttu-id="4ac93-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ac93-107">Type</span></span>        | <span data-ttu-id="4ac93-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ac93-108">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4ac93-109">registrationCount</span><span class="sxs-lookup"><span data-stu-id="4ac93-109">registrationCount</span></span> | <span data-ttu-id="4ac93-110">Int64</span><span class="sxs-lookup"><span data-stu-id="4ac93-110">Int64</span></span> | <span data-ttu-id="4ac93-111">Fornece a contagem de registro para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="4ac93-111">Provides the registration count for your tenant.</span></span> |
| <span data-ttu-id="4ac93-112">registrationStatus</span><span class="sxs-lookup"><span data-stu-id="4ac93-112">registrationStatus</span></span> | <span data-ttu-id="4ac93-113">String</span><span class="sxs-lookup"><span data-stu-id="4ac93-113">String</span></span> | <span data-ttu-id="4ac93-114">Representa o status do registro do usuário.</span><span class="sxs-lookup"><span data-stu-id="4ac93-114">Represents the status of user registration.</span></span> <span data-ttu-id="4ac93-115">Os valores possíveis são `registered`: `enabled`, `capable`,, `mfaRegistered`e.</span><span class="sxs-lookup"><span data-stu-id="4ac93-115">Possible values are: `registered`, `enabled`, `capable`, and `mfaRegistered`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4ac93-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ac93-116">JSON representation</span></span>

<span data-ttu-id="4ac93-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4ac93-117">The following is a JSON representation of the resource.</span></span>

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