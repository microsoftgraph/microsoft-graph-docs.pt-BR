---
title: tipo de recurso de educationIdentityMatchingOptions
description: Fornece um mapeamento entre uma propriedade de fonte e uma propriedade de destino para contas de usuário correspondentes. A propriedade source deve existir nos dados de origem. A propriedade de destino deve ser uma propriedade válida, no Windows Azure Active Directory (AD Azure).
author: mmast-msft
ms.openlocfilehash: bc2b99654d8e27d52ed92d9b55a32fdff8e730f4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325428"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="f3e53-105">tipo de recurso de educationIdentityMatchingOptions</span><span class="sxs-lookup"><span data-stu-id="f3e53-105">educationIdentityMatchingOptions resource type</span></span>

> <span data-ttu-id="f3e53-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f3e53-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3e53-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f3e53-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f3e53-108">Fornece um mapeamento entre uma propriedade de fonte e uma propriedade de destino para contas de usuário correspondentes.</span><span class="sxs-lookup"><span data-stu-id="f3e53-108">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="f3e53-109">A propriedade source deve existir nos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="f3e53-109">The source property should exist in the source data.</span></span> <span data-ttu-id="f3e53-110">A propriedade de destino deve ser uma propriedade válida, no Windows Azure Active Directory (AD Azure).</span><span class="sxs-lookup"><span data-stu-id="f3e53-110">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="f3e53-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f3e53-111">Properties</span></span>

| <span data-ttu-id="f3e53-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3e53-112">Property</span></span> | <span data-ttu-id="f3e53-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3e53-113">Type</span></span> | <span data-ttu-id="f3e53-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3e53-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="f3e53-115">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="f3e53-115">**appliesTo**</span></span> | <span data-ttu-id="f3e53-116">string</span><span class="sxs-lookup"><span data-stu-id="f3e53-116">string</span></span> |  <span data-ttu-id="f3e53-117">O tipo de função de usuário para atribuir da licença.</span><span class="sxs-lookup"><span data-stu-id="f3e53-117">The user role type to assign to the license.</span></span> <span data-ttu-id="f3e53-118">Os valores possíveis são: `student` e `teacher`.</span><span class="sxs-lookup"><span data-stu-id="f3e53-118">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="f3e53-119">**sourcePropertyName**</span><span class="sxs-lookup"><span data-stu-id="f3e53-119">**sourcePropertyName**</span></span> | <span data-ttu-id="f3e53-120">string</span><span class="sxs-lookup"><span data-stu-id="f3e53-120">string</span></span> |  <span data-ttu-id="f3e53-121">O nome da propriedade source, que deve ser um nome de campo nos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="f3e53-121">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="f3e53-122">Essa propriedade diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="f3e53-122">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="f3e53-123">**targetPropertyName**</span><span class="sxs-lookup"><span data-stu-id="f3e53-123">**targetPropertyName**</span></span> | <span data-ttu-id="f3e53-124">string</span><span class="sxs-lookup"><span data-stu-id="f3e53-124">string</span></span> |  <span data-ttu-id="f3e53-125">O nome da propriedade destino, que deve ser uma propriedade válida no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f3e53-125">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="f3e53-126">Essa propriedade diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="f3e53-126">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="f3e53-127">**targetDomain**</span><span class="sxs-lookup"><span data-stu-id="f3e53-127">**targetDomain**</span></span> | <span data-ttu-id="f3e53-128">string</span><span class="sxs-lookup"><span data-stu-id="f3e53-128">string</span></span> |  <span data-ttu-id="f3e53-129">O domínio ao sufixo com a propriedade source a correspondência de destino.</span><span class="sxs-lookup"><span data-stu-id="f3e53-129">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="f3e53-130">Caso seja fornecido como nulo, a propriedade source será usada para coincidir com a propriedade de destino.</span><span class="sxs-lookup"><span data-stu-id="f3e53-130">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="f3e53-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f3e53-131">JSON representation</span></span>
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
