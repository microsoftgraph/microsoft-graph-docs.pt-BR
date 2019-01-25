---
title: tipo de recurso de educationIdentityMatchingConfiguration
description: Define as configurações para a correspondência de identidades de perfil de dados escola. Essas identidades incluem alunos e professores. Com base nessas configurações, os usuários serão atualizados no diretório.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: f8712cedf6cd8bd748b8bc29a17bea0779bbe253
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520309"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a><span data-ttu-id="da347-105">tipo de recurso de educationIdentityMatchingConfiguration</span><span class="sxs-lookup"><span data-stu-id="da347-105">educationIdentityMatchingConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da347-106">Define as configurações para a correspondência de identidades de perfil de dados escola.</span><span class="sxs-lookup"><span data-stu-id="da347-106">Defines the settings for matching school data profile identities.</span></span> <span data-ttu-id="da347-107">Essas identidades incluem alunos e professores.</span><span class="sxs-lookup"><span data-stu-id="da347-107">These identities include students and teachers.</span></span> <span data-ttu-id="da347-108">Com base nessas configurações, os usuários serão atualizados no diretório.</span><span class="sxs-lookup"><span data-stu-id="da347-108">Based on these settings, the users will be updated in the directory.</span></span>

> <span data-ttu-id="da347-109">**Observação:** Nenhum usuário é criado quando este recurso for selecionado.</span><span class="sxs-lookup"><span data-stu-id="da347-109">**Note:** No users are created when this resource is selected.</span></span>

## <a name="properties"></a><span data-ttu-id="da347-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da347-110">Properties</span></span>

| <span data-ttu-id="da347-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da347-111">Property</span></span> | <span data-ttu-id="da347-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="da347-112">Type</span></span> | <span data-ttu-id="da347-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="da347-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="da347-114">**matchingOptions**</span><span class="sxs-lookup"><span data-stu-id="da347-114">**matchingOptions**</span></span> | <span data-ttu-id="da347-115">coleção [microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md)</span><span class="sxs-lookup"><span data-stu-id="da347-115">[microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md) collection</span></span> | <span data-ttu-id="da347-116">Mapeamento entre a conta de usuário e as opções utilizado para identificar exclusivamente o usuário a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="da347-116">Mapping between the user account and the options to use to uniquely identify the user to update.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="da347-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da347-117">JSON representation</span></span>
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
