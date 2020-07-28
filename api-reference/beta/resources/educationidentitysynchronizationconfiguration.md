---
title: tipo de recurso educationIdentitySynchronizationConfiguration
description: Classe abstrata de base para todas as configurações de sincronização de identidade de perfil de dados da escola. As classes derivadas definem o comportamento da sincronização de identidades. Estes são os tipos derivados.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1c3531999065abc22cc0ecb1870b4bd1bb5f45b7
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45435016"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="968ce-105">tipo de recurso educationIdentitySynchronizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="968ce-105">educationIdentitySynchronizationConfiguration resource type</span></span>

<span data-ttu-id="968ce-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="968ce-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="968ce-107">Classe abstrata de base para todas as configurações de sincronização de identidade de perfil de dados da escola.</span><span class="sxs-lookup"><span data-stu-id="968ce-107">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="968ce-108">As classes derivadas definem o comportamento da sincronização de identidades.</span><span class="sxs-lookup"><span data-stu-id="968ce-108">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="968ce-109">Estes são os tipos derivados.</span><span class="sxs-lookup"><span data-stu-id="968ce-109">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="968ce-110">Tipos derivados</span><span class="sxs-lookup"><span data-stu-id="968ce-110">Derived types</span></span>

| <span data-ttu-id="968ce-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="968ce-111">Type</span></span>                                                                                | <span data-ttu-id="968ce-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="968ce-112">Description</span></span>                                                                         |
| :---------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------- |
| [<span data-ttu-id="968ce-113">educationIdentityMatchingConfiguration</span><span class="sxs-lookup"><span data-stu-id="968ce-113">educationIdentityMatchingConfiguration</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="968ce-114">Use este tipo para **fazer a correspondência** de contas de usuário existentes no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="968ce-114">Use this type to **match existing** user accounts in Azure Active Directory.</span></span> |
| [<span data-ttu-id="968ce-115">educationIdentityCreationConfiguration</span><span class="sxs-lookup"><span data-stu-id="968ce-115">educationIdentityCreationConfiguration</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="968ce-116">Use este tipo para **criar novas** contas de usuário no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="968ce-116">Use this type to **create new** user accounts in Azure Active Directory.</span></span>                              |

## <a name="json-representation"></a><span data-ttu-id="968ce-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="968ce-117">JSON representation</span></span>

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
