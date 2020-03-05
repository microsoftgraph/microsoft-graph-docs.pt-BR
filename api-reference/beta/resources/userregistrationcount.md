---
title: tipo de recurso userRegistrationCount
description: Representa a contagem de registro e o status de usuários em seu locatário.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 2b1a7d2c34ff21c8efd57b358864c4d218630594
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519516"
---
# <a name="userregistrationcount-resource-type"></a><span data-ttu-id="20628-103">tipo de recurso userRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="20628-103">userRegistrationCount resource type</span></span>

<span data-ttu-id="20628-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="20628-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20628-105">Representa a contagem de registro e o status de usuários em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="20628-105">Represents the registration count and status for users in your tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="20628-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20628-106">Properties</span></span>

| <span data-ttu-id="20628-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20628-107">Property</span></span>     | <span data-ttu-id="20628-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="20628-108">Type</span></span>        | <span data-ttu-id="20628-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="20628-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="20628-110">registrationCount</span><span class="sxs-lookup"><span data-stu-id="20628-110">registrationCount</span></span> | <span data-ttu-id="20628-111">Int64</span><span class="sxs-lookup"><span data-stu-id="20628-111">Int64</span></span> | <span data-ttu-id="20628-112">Fornece a contagem de registro para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="20628-112">Provides the registration count for your tenant.</span></span> |
| <span data-ttu-id="20628-113">registrationStatus</span><span class="sxs-lookup"><span data-stu-id="20628-113">registrationStatus</span></span> | <span data-ttu-id="20628-114">String</span><span class="sxs-lookup"><span data-stu-id="20628-114">String</span></span> | <span data-ttu-id="20628-115">Representa o status do registro do usuário.</span><span class="sxs-lookup"><span data-stu-id="20628-115">Represents the status of user registration.</span></span> <span data-ttu-id="20628-116">Os valores possíveis são `registered`: `enabled`, `capable`,, `mfaRegistered`e.</span><span class="sxs-lookup"><span data-stu-id="20628-116">Possible values are: `registered`, `enabled`, `capable`, and `mfaRegistered`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="20628-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20628-117">JSON representation</span></span>

<span data-ttu-id="20628-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="20628-118">The following is a JSON representation of the resource.</span></span>

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