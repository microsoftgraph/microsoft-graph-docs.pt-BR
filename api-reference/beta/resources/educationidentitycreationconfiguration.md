---
title: tipo de recurso de educationIdentityCreationConfiguration
description: Define as configurações na criação das identidades de perfil de dados escola. Essas identidades incluem alunos e professores. Com base nessas configurações, os usuários serão criados no diretório.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 92ad3c36a9379bb570f2a635038903e64a0309e8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511398"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a><span data-ttu-id="07daf-105">tipo de recurso de educationIdentityCreationConfiguration</span><span class="sxs-lookup"><span data-stu-id="07daf-105">educationIdentityCreationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07daf-106">Define as configurações na criação das identidades de perfil de dados escola.</span><span class="sxs-lookup"><span data-stu-id="07daf-106">Defines the settings on creation of school data profile identities.</span></span> <span data-ttu-id="07daf-107">Essas identidades incluem alunos e professores.</span><span class="sxs-lookup"><span data-stu-id="07daf-107">These identities include students and teachers.</span></span> <span data-ttu-id="07daf-108">Com base nessas configurações, os usuários serão criados no diretório.</span><span class="sxs-lookup"><span data-stu-id="07daf-108">Based on these settings, the users will be created in the directory.</span></span>

> <span data-ttu-id="07daf-109">**Observação:** Se você tiver ativada a sincronização entre o local do Active Directory e o Azure Active Directory (AD Azure) de sincronização de diretório, use o recurso de [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="07daf-109">**Note:** If you have directory sync turned on to sync between on-premises Active Directory and Azure Active Directory (Azure AD), use the [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) resource instead.</span></span>

<span data-ttu-id="07daf-110">Derivado do [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07daf-110">Derived from [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="07daf-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07daf-111">Properties</span></span>

| <span data-ttu-id="07daf-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07daf-112">Property</span></span> | <span data-ttu-id="07daf-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="07daf-113">Type</span></span> | <span data-ttu-id="07daf-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="07daf-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="07daf-115">**userDomains**</span><span class="sxs-lookup"><span data-stu-id="07daf-115">**userDomains**</span></span> | <span data-ttu-id="07daf-116">coleção [educationIdentityDomain](educationidentitydomain.md)</span><span class="sxs-lookup"><span data-stu-id="07daf-116">[educationIdentityDomain](educationidentitydomain.md) collection</span></span> |  <span data-ttu-id="07daf-117">Define a lista de domínios a serem utilizadas por tipo de usuário.</span><span class="sxs-lookup"><span data-stu-id="07daf-117">Sets the list of domains to use per user type.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="07daf-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07daf-118">JSON representation</span></span>
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
