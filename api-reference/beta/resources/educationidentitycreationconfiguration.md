---
title: tipo de recurso educationIdentityCreationConfiguration
description: Define as configurações de criação de identidades de perfis de dados escolares. Essas identidades incluem estudantes e professores. Com base nessas configurações, os usuários serão criados no diretório.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 92ad3c36a9379bb570f2a635038903e64a0309e8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507158"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a><span data-ttu-id="b93fa-105">tipo de recurso educationIdentityCreationConfiguration</span><span class="sxs-lookup"><span data-stu-id="b93fa-105">educationIdentityCreationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b93fa-106">Define as configurações de criação de identidades de perfis de dados escolares.</span><span class="sxs-lookup"><span data-stu-id="b93fa-106">Defines the settings on creation of school data profile identities.</span></span> <span data-ttu-id="b93fa-107">Essas identidades incluem estudantes e professores.</span><span class="sxs-lookup"><span data-stu-id="b93fa-107">These identities include students and teachers.</span></span> <span data-ttu-id="b93fa-108">Com base nessas configurações, os usuários serão criados no diretório.</span><span class="sxs-lookup"><span data-stu-id="b93fa-108">Based on these settings, the users will be created in the directory.</span></span>

> <span data-ttu-id="b93fa-109">**Observação:** Se você tiver a sincronização de diretório ativada para sincronizar entre o Active Directory local e o Azure Active Directory (Azure AD), use o recurso [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) em vez disso.</span><span class="sxs-lookup"><span data-stu-id="b93fa-109">**Note:** If you have directory sync turned on to sync between on-premises Active Directory and Azure Active Directory (Azure AD), use the [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) resource instead.</span></span>

<span data-ttu-id="b93fa-110">Derivado de [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b93fa-110">Derived from [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b93fa-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b93fa-111">Properties</span></span>

| <span data-ttu-id="b93fa-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b93fa-112">Property</span></span> | <span data-ttu-id="b93fa-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="b93fa-113">Type</span></span> | <span data-ttu-id="b93fa-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="b93fa-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="b93fa-115">**userDomains**</span><span class="sxs-lookup"><span data-stu-id="b93fa-115">**userDomains**</span></span> | <span data-ttu-id="b93fa-116">coleção [educationIdentityDomain](educationidentitydomain.md)</span><span class="sxs-lookup"><span data-stu-id="b93fa-116">[educationIdentityDomain](educationidentitydomain.md) collection</span></span> |  <span data-ttu-id="b93fa-117">Define a lista de domínios a serem usados por tipo de usuário.</span><span class="sxs-lookup"><span data-stu-id="b93fa-117">Sets the list of domains to use per user type.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="b93fa-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b93fa-118">JSON representation</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitycreationconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
