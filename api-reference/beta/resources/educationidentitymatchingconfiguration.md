---
title: tipo de recurso educationIdentityMatchingConfiguration
description: Define as configurações para as identidades correspondentes de perfil de dados da escola. Essas identidades incluem estudantes e professores. Com base nessas configurações, os usuários serão atualizados no diretório.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 7c26ef1447272b88c59ec6992e41ae051439645e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095386"
---
# <a name="educationidentitymatchingconfiguration-resource-type"></a><span data-ttu-id="a4441-105">tipo de recurso educationIdentityMatchingConfiguration</span><span class="sxs-lookup"><span data-stu-id="a4441-105">educationIdentityMatchingConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4441-106">Define as configurações para as identidades correspondentes de perfil de dados da escola.</span><span class="sxs-lookup"><span data-stu-id="a4441-106">Defines the settings for matching school data profile identities.</span></span> <span data-ttu-id="a4441-107">Essas identidades incluem estudantes e professores.</span><span class="sxs-lookup"><span data-stu-id="a4441-107">These identities include students and teachers.</span></span> <span data-ttu-id="a4441-108">Com base nessas configurações, os usuários serão atualizados no diretório.</span><span class="sxs-lookup"><span data-stu-id="a4441-108">Based on these settings, the users will be updated in the directory.</span></span>

> [!NOTE]
> <span data-ttu-id="a4441-109">Nenhum usuário é criado quando esse recurso é selecionado.</span><span class="sxs-lookup"><span data-stu-id="a4441-109">No Users are created when this resource is selected.</span></span>

## <a name="properties"></a><span data-ttu-id="a4441-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a4441-110">Properties</span></span>

| <span data-ttu-id="a4441-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a4441-111">Property</span></span>        | <span data-ttu-id="a4441-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4441-112">Type</span></span>                                                                                               | <span data-ttu-id="a4441-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4441-113">Description</span></span>                                                                                      |
| :-------------- | :------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------- |
| <span data-ttu-id="a4441-114">matchoptions</span><span class="sxs-lookup"><span data-stu-id="a4441-114">matchingOptions</span></span> | <span data-ttu-id="a4441-115">coleção [Microsoft. Graph. educationIdentityMatchingOptions](educationidentitymatchingoptions.md)</span><span class="sxs-lookup"><span data-stu-id="a4441-115">[microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md) collection</span></span> | <span data-ttu-id="a4441-116">Mapeamento entre a conta de usuário e as opções a serem usadas para identificar exclusivamente o usuário a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="a4441-116">Mapping between the user account and the options to use to uniquely identify the user to update.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a4441-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a4441-117">JSON representation</span></span>

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
      "appliesTo": { "@odata.type": "microsoft.graph.educationUserRole" },
      "sourcePropertyName": "String",
      "targetPropertyName": "String",
      "targetDomain": "String"
    }
  ]
}
```


