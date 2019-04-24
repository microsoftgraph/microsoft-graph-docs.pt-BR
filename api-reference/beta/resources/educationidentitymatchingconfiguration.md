---
title: tipo de recurso educationIdentityMatchingConfiguration
description: Define as configurações para as identidades correspondentes de perfil de dados da escola. Essas identidades incluem estudantes e professores. Com base nessas configurações, os usuários serão atualizados no diretório.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: f8712cedf6cd8bd748b8bc29a17bea0779bbe253
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507111"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a><span data-ttu-id="d8bb7-105">tipo de recurso educationIdentityMatchingConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8bb7-105">educationIdentityMatchingConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8bb7-106">Define as configurações para as identidades correspondentes de perfil de dados da escola.</span><span class="sxs-lookup"><span data-stu-id="d8bb7-106">Defines the settings for matching school data profile identities.</span></span> <span data-ttu-id="d8bb7-107">Essas identidades incluem estudantes e professores.</span><span class="sxs-lookup"><span data-stu-id="d8bb7-107">These identities include students and teachers.</span></span> <span data-ttu-id="d8bb7-108">Com base nessas configurações, os usuários serão atualizados no diretório.</span><span class="sxs-lookup"><span data-stu-id="d8bb7-108">Based on these settings, the users will be updated in the directory.</span></span>

> <span data-ttu-id="d8bb7-109">**Observação:** Nenhum usuário é criado quando esse recurso é selecionado.</span><span class="sxs-lookup"><span data-stu-id="d8bb7-109">**Note:** No users are created when this resource is selected.</span></span>

## <a name="properties"></a><span data-ttu-id="d8bb7-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8bb7-110">Properties</span></span>

| <span data-ttu-id="d8bb7-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8bb7-111">Property</span></span> | <span data-ttu-id="d8bb7-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8bb7-112">Type</span></span> | <span data-ttu-id="d8bb7-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8bb7-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="d8bb7-114">**matchoptions**</span><span class="sxs-lookup"><span data-stu-id="d8bb7-114">**matchingOptions**</span></span> | <span data-ttu-id="d8bb7-115">coleção [Microsoft. Graph. educationIdentityMatchingOptions](educationidentitymatchingoptions.md)</span><span class="sxs-lookup"><span data-stu-id="d8bb7-115">[microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md) collection</span></span> | <span data-ttu-id="d8bb7-116">Mapeamento entre a conta de usuário e as opções a serem usadas para identificar exclusivamente o usuário a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="d8bb7-116">Mapping between the user account and the options to use to uniquely identify the user to update.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d8bb7-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8bb7-117">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingConfiguration"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationIdentityMatchingConfiguration",
    "matchingOptions": [
        {
            "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
            "sourcePropertyName": "String",
            "targetPropertyName": "String",
            "targetDomain": "String"
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitymatchingconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
