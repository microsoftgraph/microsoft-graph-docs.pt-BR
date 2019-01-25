---
title: tipo de recurso de educationIdentityMatchingOptions
description: Fornece um mapeamento entre uma propriedade de fonte e uma propriedade de destino para contas de usuário correspondentes. A propriedade source deve existir nos dados de origem. A propriedade de destino deve ser uma propriedade válida, no Windows Azure Active Directory (AD Azure).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 723a74cff1d5a660272d3456e9f54de8a54e21bc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513701"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="1b4f6-105">tipo de recurso de educationIdentityMatchingOptions</span><span class="sxs-lookup"><span data-stu-id="1b4f6-105">educationIdentityMatchingOptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b4f6-106">Fornece um mapeamento entre uma propriedade de fonte e uma propriedade de destino para contas de usuário correspondentes.</span><span class="sxs-lookup"><span data-stu-id="1b4f6-106">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="1b4f6-107">A propriedade source deve existir nos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="1b4f6-107">The source property should exist in the source data.</span></span> <span data-ttu-id="1b4f6-108">A propriedade de destino deve ser uma propriedade válida, no Windows Azure Active Directory (AD Azure).</span><span class="sxs-lookup"><span data-stu-id="1b4f6-108">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="1b4f6-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b4f6-109">Properties</span></span>

| <span data-ttu-id="1b4f6-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b4f6-110">Property</span></span> | <span data-ttu-id="1b4f6-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b4f6-111">Type</span></span> | <span data-ttu-id="1b4f6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b4f6-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="1b4f6-113">appliesTo</span><span class="sxs-lookup"><span data-stu-id="1b4f6-113">**appliesTo**</span></span> | <span data-ttu-id="1b4f6-114">string</span><span class="sxs-lookup"><span data-stu-id="1b4f6-114">string</span></span> |  <span data-ttu-id="1b4f6-115">O tipo de função de usuário para atribuir da licença.</span><span class="sxs-lookup"><span data-stu-id="1b4f6-115">The user role type to assign to the license.</span></span> <span data-ttu-id="1b4f6-116">Os valores possíveis são: `student` e `teacher`.</span><span class="sxs-lookup"><span data-stu-id="1b4f6-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="1b4f6-117">**sourcePropertyName**</span><span class="sxs-lookup"><span data-stu-id="1b4f6-117">**sourcePropertyName**</span></span> | <span data-ttu-id="1b4f6-118">string</span><span class="sxs-lookup"><span data-stu-id="1b4f6-118">string</span></span> |  <span data-ttu-id="1b4f6-119">O nome da propriedade source, que deve ser um nome de campo nos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="1b4f6-119">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="1b4f6-120">Essa propriedade diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="1b4f6-120">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="1b4f6-121">**targetPropertyName**</span><span class="sxs-lookup"><span data-stu-id="1b4f6-121">**targetPropertyName**</span></span> | <span data-ttu-id="1b4f6-122">string</span><span class="sxs-lookup"><span data-stu-id="1b4f6-122">string</span></span> |  <span data-ttu-id="1b4f6-123">O nome da propriedade destino, que deve ser uma propriedade válida no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1b4f6-123">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="1b4f6-124">Essa propriedade diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="1b4f6-124">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="1b4f6-125">**targetDomain**</span><span class="sxs-lookup"><span data-stu-id="1b4f6-125">**targetDomain**</span></span> | <span data-ttu-id="1b4f6-126">string</span><span class="sxs-lookup"><span data-stu-id="1b4f6-126">string</span></span> |  <span data-ttu-id="1b4f6-127">O domínio ao sufixo com a propriedade source a correspondência de destino.</span><span class="sxs-lookup"><span data-stu-id="1b4f6-127">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="1b4f6-128">Caso seja fornecido como nulo, a propriedade source será usada para coincidir com a propriedade de destino.</span><span class="sxs-lookup"><span data-stu-id="1b4f6-128">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="1b4f6-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b4f6-129">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "sourcePropertyName": "String",
    "targetPropertyName": "String",
    "targetDomain": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitymatchingoptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
