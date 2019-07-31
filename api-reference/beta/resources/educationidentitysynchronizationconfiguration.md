---
title: tipo de recurso educationIdentitySynchronizationConfiguration
description: Classe abstrata de base para todas as configurações de sincronização de identidade de perfil de dados da escola. As classes derivadas definem o comportamento da sincronização de identidades. Estes são os tipos derivados.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e282a9701eaae04aae33d9fd9efc9b86f7df3635
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972674"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="37331-105">tipo de recurso educationIdentitySynchronizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="37331-105">educationIdentitySynchronizationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37331-106">Classe abstrata de base para todas as configurações de sincronização de identidade de perfil de dados da escola.</span><span class="sxs-lookup"><span data-stu-id="37331-106">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="37331-107">As classes derivadas definem o comportamento da sincronização de identidades.</span><span class="sxs-lookup"><span data-stu-id="37331-107">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="37331-108">Estes são os tipos derivados.</span><span class="sxs-lookup"><span data-stu-id="37331-108">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="37331-109">Tipos derivados</span><span class="sxs-lookup"><span data-stu-id="37331-109">Derived types</span></span>
| <span data-ttu-id="37331-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="37331-110">Type</span></span> | <span data-ttu-id="37331-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="37331-111">Description</span></span> |
|:-|:-|
| [<span data-ttu-id="37331-112">**educationIdentityMatchingConfiguration**</span><span class="sxs-lookup"><span data-stu-id="37331-112">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="37331-113">Use este tipo para fazer a correspondência de contas de usuário existentes no Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="37331-113">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="37331-114">**educationIdentityCreationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="37331-114">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="37331-115">Use este tipo para criar novas contas de usuário no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="37331-115">Use this type to create new user accounts in Azure AD.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="37331-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37331-116">JSON representation</span></span>
<!-- {
  "blockType": "resource",
   "isAbstract":true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
}-->

```json
{
}
```

