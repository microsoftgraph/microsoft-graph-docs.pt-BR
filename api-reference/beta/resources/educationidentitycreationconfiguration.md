---
title: tipo de recurso educationIdentityCreationConfiguration
description: Define as configurações de criação de identidades de perfis de dados escolares. Essas identidades incluem estudantes e professores. Com base nessas configurações, os usuários serão criados no diretório.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5f4dc03514e3d62f0dca096b0e669ada9247ff39
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095398"
---
# <a name="educationidentitycreationconfiguration-resource-type"></a><span data-ttu-id="d2b62-105">tipo de recurso educationIdentityCreationConfiguration</span><span class="sxs-lookup"><span data-stu-id="d2b62-105">educationIdentityCreationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2b62-106">Define as configurações de criação de identidades de perfis de dados escolares.</span><span class="sxs-lookup"><span data-stu-id="d2b62-106">Defines the settings on creation of school data profile identities.</span></span> <span data-ttu-id="d2b62-107">Essas identidades incluem estudantes e professores.</span><span class="sxs-lookup"><span data-stu-id="d2b62-107">These identities include students and teachers.</span></span> <span data-ttu-id="d2b62-108">Com base nessas configurações, os usuários serão criados no diretório.</span><span class="sxs-lookup"><span data-stu-id="d2b62-108">Based on these settings, the users will be created in the directory.</span></span>

> [!WARNING]
> <span data-ttu-id="d2b62-109">Se você tiver a sincronização de diretório ativada para sincronizar entre o Active Directory local e o Azure Active Directory (Azure AD), use o recurso [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) em vez disso.</span><span class="sxs-lookup"><span data-stu-id="d2b62-109">If you have directory sync turned on to sync between on-premises Active Directory and Azure Active Directory (Azure AD), use the [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) resource instead.</span></span>

<span data-ttu-id="d2b62-110">Derivado de [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d2b62-110">Derived from [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d2b62-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2b62-111">Properties</span></span>

| <span data-ttu-id="d2b62-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2b62-112">Property</span></span>    | <span data-ttu-id="d2b62-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2b62-113">Type</span></span>                                                             | <span data-ttu-id="d2b62-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2b62-114">Description</span></span>                                    |
| :---------- | :--------------------------------------------------------------- | :--------------------------------------------- |
| <span data-ttu-id="d2b62-115">userdomains</span><span class="sxs-lookup"><span data-stu-id="d2b62-115">userDomains</span></span> | <span data-ttu-id="d2b62-116">coleção [educationIdentityDomain](educationidentitydomain.md)</span><span class="sxs-lookup"><span data-stu-id="d2b62-116">[educationIdentityDomain](educationidentitydomain.md) collection</span></span> | <span data-ttu-id="d2b62-117">Define a lista de domínios a serem usados por tipo de usuário.</span><span class="sxs-lookup"><span data-stu-id="d2b62-117">Sets the list of domains to use per user type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d2b62-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2b62-118">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationIdentityCreationConfiguration",
  "userDomains": [
    {
      "@odata.type": "microsoft.graph.educationIdentityDomain"
    }
  ]
}
```


