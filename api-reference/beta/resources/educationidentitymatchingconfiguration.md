---
title: tipo de recurso de educationIdentityMatchingConfiguration
description: Define as configurações para a correspondência de identidades de perfil de dados escola. Essas identidades incluem alunos e professores. Com base nessas configurações, os usuários serão atualizados no diretório.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9ded27e432219a247bf9c03c21f8ebd0054183eb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411327"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a><span data-ttu-id="c711f-105">tipo de recurso de educationIdentityMatchingConfiguration</span><span class="sxs-lookup"><span data-stu-id="c711f-105">educationIdentityMatchingConfiguration resource type</span></span>

> <span data-ttu-id="c711f-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c711f-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c711f-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c711f-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c711f-108">Define as configurações para a correspondência de identidades de perfil de dados escola.</span><span class="sxs-lookup"><span data-stu-id="c711f-108">Defines the settings for matching school data profile identities.</span></span> <span data-ttu-id="c711f-109">Essas identidades incluem alunos e professores.</span><span class="sxs-lookup"><span data-stu-id="c711f-109">These identities include students and teachers.</span></span> <span data-ttu-id="c711f-110">Com base nessas configurações, os usuários serão atualizados no diretório.</span><span class="sxs-lookup"><span data-stu-id="c711f-110">Based on these settings, the users will be updated in the directory.</span></span>

> <span data-ttu-id="c711f-111">**Observação:** Nenhum usuário é criado quando este recurso for selecionado.</span><span class="sxs-lookup"><span data-stu-id="c711f-111">**Note:** No users are created when this resource is selected.</span></span>

## <a name="properties"></a><span data-ttu-id="c711f-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c711f-112">Properties</span></span>

| <span data-ttu-id="c711f-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c711f-113">Property</span></span> | <span data-ttu-id="c711f-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="c711f-114">Type</span></span> | <span data-ttu-id="c711f-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="c711f-115">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="c711f-116">**matchingOptions**</span><span class="sxs-lookup"><span data-stu-id="c711f-116">**matchingOptions**</span></span> | <span data-ttu-id="c711f-117">coleção [microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md)</span><span class="sxs-lookup"><span data-stu-id="c711f-117">[microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md) collection</span></span> | <span data-ttu-id="c711f-118">Mapeamento entre a conta de usuário e as opções utilizado para identificar exclusivamente o usuário a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="c711f-118">Mapping between the user account and the options to use to uniquely identify the user to update.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c711f-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c711f-119">JSON representation</span></span>
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
