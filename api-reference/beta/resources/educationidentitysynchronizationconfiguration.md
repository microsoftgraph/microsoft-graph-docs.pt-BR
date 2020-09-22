---
title: tipo de recurso educationIdentitySynchronizationConfiguration
description: Classe abstrata de base para todas as configurações de sincronização de identidade de perfil de dados da escola. As classes derivadas definem o comportamento da sincronização de identidades. Estes são os tipos derivados.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8e193c798f1f3fbc5d4d1c9d8c7b96eed7d39cf9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095356"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="69125-105">tipo de recurso educationIdentitySynchronizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="69125-105">educationIdentitySynchronizationConfiguration resource type</span></span>

<span data-ttu-id="69125-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69125-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69125-107">Classe abstrata de base para todas as configurações de sincronização de identidade de perfil de dados da escola.</span><span class="sxs-lookup"><span data-stu-id="69125-107">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="69125-108">As classes derivadas definem o comportamento da sincronização de identidades.</span><span class="sxs-lookup"><span data-stu-id="69125-108">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="69125-109">Estes são os tipos derivados.</span><span class="sxs-lookup"><span data-stu-id="69125-109">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="69125-110">Tipos derivados</span><span class="sxs-lookup"><span data-stu-id="69125-110">Derived types</span></span>

| <span data-ttu-id="69125-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="69125-111">Type</span></span>                                                                                | <span data-ttu-id="69125-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="69125-112">Description</span></span>                                                                         |
| :---------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------- |
| [<span data-ttu-id="69125-113">educationIdentityMatchingConfiguration</span><span class="sxs-lookup"><span data-stu-id="69125-113">educationIdentityMatchingConfiguration</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="69125-114">Use este tipo para **fazer a correspondência** de contas de usuário existentes no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="69125-114">Use this type to **match existing** user accounts in Azure Active Directory.</span></span> |
| [<span data-ttu-id="69125-115">educationIdentityCreationConfiguration</span><span class="sxs-lookup"><span data-stu-id="69125-115">educationIdentityCreationConfiguration</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="69125-116">Use este tipo para **criar novas** contas de usuário no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="69125-116">Use this type to **create new** user accounts in Azure Active Directory.</span></span>                              |

## <a name="json-representation"></a><span data-ttu-id="69125-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69125-117">JSON representation</span></span>

<!-- {
  "blockType": "resource",
   "isAbstract":true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
}-->

```json
{}
```


