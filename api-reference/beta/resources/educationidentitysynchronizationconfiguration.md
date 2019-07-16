---
title: tipo de recurso educationIdentitySynchronizationConfiguration
description: Classe abstrata de base para todas as configurações de sincronização de identidade de perfil de dados da escola. As classes derivadas definem o comportamento da sincronização de identidades. Estes são os tipos derivados.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 713bb285e739d9182a982f02975a9b9f46761e3a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736513"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="67e43-105">tipo de recurso educationIdentitySynchronizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="67e43-105">educationIdentitySynchronizationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67e43-106">Classe abstrata de base para todas as configurações de sincronização de identidade de perfil de dados da escola.</span><span class="sxs-lookup"><span data-stu-id="67e43-106">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="67e43-107">As classes derivadas definem o comportamento da sincronização de identidades.</span><span class="sxs-lookup"><span data-stu-id="67e43-107">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="67e43-108">Estes são os tipos derivados.</span><span class="sxs-lookup"><span data-stu-id="67e43-108">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="67e43-109">Tipos derivados</span><span class="sxs-lookup"><span data-stu-id="67e43-109">Derived types</span></span>
| <span data-ttu-id="67e43-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="67e43-110">Type</span></span> | <span data-ttu-id="67e43-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="67e43-111">Description</span></span> |
|:-|:-|
| [<span data-ttu-id="67e43-112">**educationIdentityMatchingConfiguration**</span><span class="sxs-lookup"><span data-stu-id="67e43-112">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="67e43-113">Use este tipo para fazer a correspondência de contas de usuário existentes no Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="67e43-113">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="67e43-114">**educationIdentityCreationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="67e43-114">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="67e43-115">Use este tipo para criar novas contas de usuário no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="67e43-115">Use this type to create new user accounts in Azure AD.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="67e43-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="67e43-116">JSON representation</span></span>
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

