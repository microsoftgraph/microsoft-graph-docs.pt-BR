---
title: tipo de recurso educationIdentitySynchronizationConfiguration
description: Classe abstrata de base para todas as configurações de sincronização de identidade de perfil de dados da escola. As classes derivadas definem o comportamento da sincronização de identidades. Estes são os tipos derivados.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1ffa1bbcd3f96c86818c68d350236086d0975187
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501791"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="deb90-105">tipo de recurso educationIdentitySynchronizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="deb90-105">educationIdentitySynchronizationConfiguration resource type</span></span>

<span data-ttu-id="deb90-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="deb90-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="deb90-107">Classe abstrata de base para todas as configurações de sincronização de identidade de perfil de dados da escola.</span><span class="sxs-lookup"><span data-stu-id="deb90-107">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="deb90-108">As classes derivadas definem o comportamento da sincronização de identidades.</span><span class="sxs-lookup"><span data-stu-id="deb90-108">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="deb90-109">Estes são os tipos derivados.</span><span class="sxs-lookup"><span data-stu-id="deb90-109">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="deb90-110">Tipos derivados</span><span class="sxs-lookup"><span data-stu-id="deb90-110">Derived types</span></span>
| <span data-ttu-id="deb90-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="deb90-111">Type</span></span> | <span data-ttu-id="deb90-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="deb90-112">Description</span></span> |
|:-|:-|
| [<span data-ttu-id="deb90-113">**educationIdentityMatchingConfiguration**</span><span class="sxs-lookup"><span data-stu-id="deb90-113">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="deb90-114">Use este tipo para fazer a correspondência de contas de usuário existentes no Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="deb90-114">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="deb90-115">**educationIdentityCreationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="deb90-115">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="deb90-116">Use este tipo para criar novas contas de usuário no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="deb90-116">Use this type to create new user accounts in Azure AD.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="deb90-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="deb90-117">JSON representation</span></span>
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

