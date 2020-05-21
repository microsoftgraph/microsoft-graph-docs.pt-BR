---
title: tipo de recurso educationIdentityCreationConfiguration
description: Define as configurações de criação de identidades de perfis de dados escolares. Essas identidades incluem estudantes e professores. Com base nessas configurações, os usuários serão criados no diretório.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 80c564999ca0e414c6475f858c5d3ebe5e037e4b
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336018"
---
# <a name="educationidentitycreationconfiguration-resource-type"></a><span data-ttu-id="f0f8b-105">tipo de recurso educationIdentityCreationConfiguration</span><span class="sxs-lookup"><span data-stu-id="f0f8b-105">educationIdentityCreationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0f8b-106">Define as configurações de criação de identidades de perfis de dados escolares.</span><span class="sxs-lookup"><span data-stu-id="f0f8b-106">Defines the settings on creation of school data profile identities.</span></span> <span data-ttu-id="f0f8b-107">Essas identidades incluem estudantes e professores.</span><span class="sxs-lookup"><span data-stu-id="f0f8b-107">These identities include students and teachers.</span></span> <span data-ttu-id="f0f8b-108">Com base nessas configurações, os usuários serão criados no diretório.</span><span class="sxs-lookup"><span data-stu-id="f0f8b-108">Based on these settings, the users will be created in the directory.</span></span>

> <span data-ttu-id="f0f8b-109">**Observação:** Se você tiver a sincronização de diretório ativada para sincronizar entre o Active Directory local e o Azure Active Directory (Azure AD), use o recurso [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) em vez disso.</span><span class="sxs-lookup"><span data-stu-id="f0f8b-109">**Note:** If you have directory sync turned on to sync between on-premises Active Directory and Azure Active Directory (Azure AD), use the [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) resource instead.</span></span>

<span data-ttu-id="f0f8b-110">Derivado de [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0f8b-110">Derived from [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f0f8b-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0f8b-111">Properties</span></span>

| <span data-ttu-id="f0f8b-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0f8b-112">Property</span></span> | <span data-ttu-id="f0f8b-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0f8b-113">Type</span></span> | <span data-ttu-id="f0f8b-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0f8b-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="f0f8b-115">**userdomains**</span><span class="sxs-lookup"><span data-stu-id="f0f8b-115">**userDomains**</span></span> | <span data-ttu-id="f0f8b-116">coleção [educationIdentityDomain](educationidentitydomain.md)</span><span class="sxs-lookup"><span data-stu-id="f0f8b-116">[educationIdentityDomain](educationidentitydomain.md) collection</span></span> |  <span data-ttu-id="f0f8b-117">Define a lista de domínios a serem usados por tipo de usuário.</span><span class="sxs-lookup"><span data-stu-id="f0f8b-117">Sets the list of domains to use per user type.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="f0f8b-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0f8b-118">JSON representation</span></span>
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
            "@odata.type": "microsoft.graph.educationIdentityDomain",
        }
    ]
}
```
