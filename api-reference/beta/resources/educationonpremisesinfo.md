---
title: tipo de recurso educationOnPremisesInfo
description: Informações adicionais usadas para associar uma conta de usuário local do Active Directory ao objeto de usuário do Azure AD.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c147755aea584674e17f2de913e039b7d3e0cf82
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764731"
---
# <a name="educationonpremisesinfo-resource-type"></a><span data-ttu-id="147aa-103">tipo de recurso educationOnPremisesInfo</span><span class="sxs-lookup"><span data-stu-id="147aa-103">educationOnPremisesInfo resource type</span></span>

<span data-ttu-id="147aa-104">Informações adicionais usadas para associar uma conta de usuário local do Active Directory ao objeto de usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="147aa-104">Additional information used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span>

## <a name="properties"></a><span data-ttu-id="147aa-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="147aa-105">Properties</span></span>

| <span data-ttu-id="147aa-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="147aa-106">Property</span></span>    | <span data-ttu-id="147aa-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="147aa-107">Type</span></span>   | <span data-ttu-id="147aa-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="147aa-108">Description</span></span>                                               |
| :---------- | :----- | :-------------------------------------------------------- |
| <span data-ttu-id="147aa-109">imutávelid</span><span class="sxs-lookup"><span data-stu-id="147aa-109">immutableId</span></span> | <span data-ttu-id="147aa-110">String</span><span class="sxs-lookup"><span data-stu-id="147aa-110">String</span></span> | <span data-ttu-id="147aa-111">Identificador exclusivo do objeto de usuário no Active Directory.</span><span class="sxs-lookup"><span data-stu-id="147aa-111">Unique identifier for the user object in Active Directory.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="147aa-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="147aa-112">JSON representation</span></span>

<span data-ttu-id="147aa-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="147aa-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOnPremisesInfo"
}-->

```json
{
  "immutableId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOnPremisesInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
