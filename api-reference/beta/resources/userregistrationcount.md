---
title: tipo de recurso userRegistrationCount
description: Representa a contagem de registro e o status de usuários em seu locatário.
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 5aa86a0b490ddb2cd68a504f5a4879f922fa0cf2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057819"
---
# <a name="userregistrationcount-resource-type"></a><span data-ttu-id="92ae4-103">tipo de recurso userRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="92ae4-103">userRegistrationCount resource type</span></span>

<span data-ttu-id="92ae4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92ae4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92ae4-105">Representa a contagem de registro e o status de usuários em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="92ae4-105">Represents the registration count and status for users in your tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="92ae4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="92ae4-106">Properties</span></span>

| <span data-ttu-id="92ae4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92ae4-107">Property</span></span>     | <span data-ttu-id="92ae4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="92ae4-108">Type</span></span>        | <span data-ttu-id="92ae4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="92ae4-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="92ae4-110">registrationCount</span><span class="sxs-lookup"><span data-stu-id="92ae4-110">registrationCount</span></span> | <span data-ttu-id="92ae4-111">Int64</span><span class="sxs-lookup"><span data-stu-id="92ae4-111">Int64</span></span> | <span data-ttu-id="92ae4-112">Fornece a contagem de registro para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="92ae4-112">Provides the registration count for your tenant.</span></span> |
| <span data-ttu-id="92ae4-113">registrationStatus</span><span class="sxs-lookup"><span data-stu-id="92ae4-113">registrationStatus</span></span> | <span data-ttu-id="92ae4-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92ae4-114">String</span></span> | <span data-ttu-id="92ae4-115">Representa o status do registro do usuário.</span><span class="sxs-lookup"><span data-stu-id="92ae4-115">Represents the status of user registration.</span></span> <span data-ttu-id="92ae4-116">Os valores possíveis são: `registered` , `enabled` , `capable` , e `mfaRegistered` .</span><span class="sxs-lookup"><span data-stu-id="92ae4-116">Possible values are: `registered`, `enabled`, `capable`, and `mfaRegistered`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="92ae4-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="92ae4-117">JSON representation</span></span>

<span data-ttu-id="92ae4-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="92ae4-118">The following is a JSON representation of the resource.</span></span>

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

