---
title: tipo de recurso educationIdentityMatchingConfiguration
description: Define as configurações para as identidades correspondentes de perfil de dados da escola. Essas identidades incluem estudantes e professores. Com base nessas configurações, os usuários serão atualizados no diretório.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 0384fa269fd4304272d719df5860296d5f788c19
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340473"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a><span data-ttu-id="fd1d0-105">tipo de recurso educationIdentityMatchingConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd1d0-105">educationIdentityMatchingConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd1d0-106">Define as configurações para as identidades correspondentes de perfil de dados da escola.</span><span class="sxs-lookup"><span data-stu-id="fd1d0-106">Defines the settings for matching school data profile identities.</span></span> <span data-ttu-id="fd1d0-107">Essas identidades incluem estudantes e professores.</span><span class="sxs-lookup"><span data-stu-id="fd1d0-107">These identities include students and teachers.</span></span> <span data-ttu-id="fd1d0-108">Com base nessas configurações, os usuários serão atualizados no diretório.</span><span class="sxs-lookup"><span data-stu-id="fd1d0-108">Based on these settings, the users will be updated in the directory.</span></span>

> <span data-ttu-id="fd1d0-109">**Observação:** Nenhum usuário é criado quando esse recurso é selecionado.</span><span class="sxs-lookup"><span data-stu-id="fd1d0-109">**Note:** No users are created when this resource is selected.</span></span>

## <a name="properties"></a><span data-ttu-id="fd1d0-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fd1d0-110">Properties</span></span>

| <span data-ttu-id="fd1d0-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd1d0-111">Property</span></span> | <span data-ttu-id="fd1d0-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd1d0-112">Type</span></span> | <span data-ttu-id="fd1d0-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd1d0-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="fd1d0-114">**matchoptions**</span><span class="sxs-lookup"><span data-stu-id="fd1d0-114">**matchingOptions**</span></span> | <span data-ttu-id="fd1d0-115">coleção [Microsoft. Graph. educationIdentityMatchingOptions](educationidentitymatchingoptions.md)</span><span class="sxs-lookup"><span data-stu-id="fd1d0-115">[microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md) collection</span></span> | <span data-ttu-id="fd1d0-116">Mapeamento entre a conta de usuário e as opções a serem usadas para identificar exclusivamente o usuário a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="fd1d0-116">Mapping between the user account and the options to use to uniquely identify the user to update.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fd1d0-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fd1d0-117">JSON representation</span></span>
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
