---
title: Tipo de recurso userRegistrationCount
description: Representa a contagem de registro e o status dos usuários em seu locatário.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 5cdcdb4cfd56c0828cfeb7e71defe4c7459e3133
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132948"
---
# <a name="userregistrationcount-resource-type"></a><span data-ttu-id="805f6-103">Tipo de recurso userRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="805f6-103">userRegistrationCount resource type</span></span>

<span data-ttu-id="805f6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="805f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="805f6-105">Representa a contagem de registro e o status dos usuários em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="805f6-105">Represents the registration count and status for users in your tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="805f6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="805f6-106">Properties</span></span>

| <span data-ttu-id="805f6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="805f6-107">Property</span></span>     | <span data-ttu-id="805f6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="805f6-108">Type</span></span>        | <span data-ttu-id="805f6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="805f6-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="805f6-110">registrationCount</span><span class="sxs-lookup"><span data-stu-id="805f6-110">registrationCount</span></span> | <span data-ttu-id="805f6-111">Int64</span><span class="sxs-lookup"><span data-stu-id="805f6-111">Int64</span></span> | <span data-ttu-id="805f6-112">Fornece a contagem de registro para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="805f6-112">Provides the registration count for your tenant.</span></span> |
| <span data-ttu-id="805f6-113">registrationStatus</span><span class="sxs-lookup"><span data-stu-id="805f6-113">registrationStatus</span></span> | <span data-ttu-id="805f6-114">String</span><span class="sxs-lookup"><span data-stu-id="805f6-114">String</span></span> | <span data-ttu-id="805f6-115">Representa o status do registro do usuário.</span><span class="sxs-lookup"><span data-stu-id="805f6-115">Represents the status of user registration.</span></span> <span data-ttu-id="805f6-116">Os valores possíveis `registered` são: `enabled` , e `capable` `mfaRegistered` .</span><span class="sxs-lookup"><span data-stu-id="805f6-116">Possible values are: `registered`, `enabled`, `capable`, and `mfaRegistered`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="805f6-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="805f6-117">JSON representation</span></span>

<span data-ttu-id="805f6-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="805f6-118">The following is a JSON representation of the resource.</span></span>

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

