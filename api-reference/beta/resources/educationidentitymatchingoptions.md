---
title: tipo de recurso de educationIdentityMatchingOptions
description: Fornece um mapeamento entre uma propriedade de fonte e uma propriedade de destino para contas de usuário correspondentes. A propriedade source deve existir nos dados de origem. A propriedade de destino deve ser uma propriedade válida, no Windows Azure Active Directory (AD Azure).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 624e2717387c5cc8994596fd83d5a6856ac6082b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978253"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="9bd9d-105">tipo de recurso de educationIdentityMatchingOptions</span><span class="sxs-lookup"><span data-stu-id="9bd9d-105">educationIdentityMatchingOptions resource type</span></span>

> <span data-ttu-id="9bd9d-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9bd9d-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9bd9d-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9bd9d-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9bd9d-108">Fornece um mapeamento entre uma propriedade de fonte e uma propriedade de destino para contas de usuário correspondentes.</span><span class="sxs-lookup"><span data-stu-id="9bd9d-108">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="9bd9d-109">A propriedade source deve existir nos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="9bd9d-109">The source property should exist in the source data.</span></span> <span data-ttu-id="9bd9d-110">A propriedade de destino deve ser uma propriedade válida, no Windows Azure Active Directory (AD Azure).</span><span class="sxs-lookup"><span data-stu-id="9bd9d-110">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="9bd9d-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9bd9d-111">Properties</span></span>

| <span data-ttu-id="9bd9d-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9bd9d-112">Property</span></span> | <span data-ttu-id="9bd9d-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bd9d-113">Type</span></span> | <span data-ttu-id="9bd9d-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bd9d-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="9bd9d-115">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="9bd9d-115">**appliesTo**</span></span> | <span data-ttu-id="9bd9d-116">string</span><span class="sxs-lookup"><span data-stu-id="9bd9d-116">string</span></span> |  <span data-ttu-id="9bd9d-117">O tipo de função de usuário para atribuir da licença.</span><span class="sxs-lookup"><span data-stu-id="9bd9d-117">The user role type to assign to the license.</span></span> <span data-ttu-id="9bd9d-118">Os valores possíveis são: `student` e `teacher`.</span><span class="sxs-lookup"><span data-stu-id="9bd9d-118">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="9bd9d-119">**sourcePropertyName**</span><span class="sxs-lookup"><span data-stu-id="9bd9d-119">**sourcePropertyName**</span></span> | <span data-ttu-id="9bd9d-120">string</span><span class="sxs-lookup"><span data-stu-id="9bd9d-120">string</span></span> |  <span data-ttu-id="9bd9d-121">O nome da propriedade source, que deve ser um nome de campo nos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="9bd9d-121">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="9bd9d-122">Essa propriedade diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9bd9d-122">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="9bd9d-123">**targetPropertyName**</span><span class="sxs-lookup"><span data-stu-id="9bd9d-123">**targetPropertyName**</span></span> | <span data-ttu-id="9bd9d-124">string</span><span class="sxs-lookup"><span data-stu-id="9bd9d-124">string</span></span> |  <span data-ttu-id="9bd9d-125">O nome da propriedade destino, que deve ser uma propriedade válida no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9bd9d-125">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="9bd9d-126">Essa propriedade diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9bd9d-126">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="9bd9d-127">**targetDomain**</span><span class="sxs-lookup"><span data-stu-id="9bd9d-127">**targetDomain**</span></span> | <span data-ttu-id="9bd9d-128">string</span><span class="sxs-lookup"><span data-stu-id="9bd9d-128">string</span></span> |  <span data-ttu-id="9bd9d-129">O domínio ao sufixo com a propriedade source a correspondência de destino.</span><span class="sxs-lookup"><span data-stu-id="9bd9d-129">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="9bd9d-130">Caso seja fornecido como nulo, a propriedade source será usada para coincidir com a propriedade de destino.</span><span class="sxs-lookup"><span data-stu-id="9bd9d-130">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="9bd9d-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9bd9d-131">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "sourcePropertyName": "String",
    "targetPropertyName": "String",
    "targetDomain": "String"
}
```
