---
title: tipo de recurso educationOnPremisesInfo
description: Informações adicionais usadas para associar uma conta de usuário local do Active Directory ao objeto de usuário do Azure AD.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6695f1cd92ccde1fb26a581fce49c0c233deb141
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501511"
---
# <a name="educationonpremisesinfo-resource-type"></a><span data-ttu-id="674ad-103">tipo de recurso educationOnPremisesInfo</span><span class="sxs-lookup"><span data-stu-id="674ad-103">educationOnPremisesInfo resource type</span></span>

<span data-ttu-id="674ad-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="674ad-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="674ad-105">Informações adicionais usadas para associar uma conta de usuário local do Active Directory ao objeto de usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="674ad-105">Additional information used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span>

## <a name="properties"></a><span data-ttu-id="674ad-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="674ad-106">Properties</span></span>

| <span data-ttu-id="674ad-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="674ad-107">Property</span></span>    | <span data-ttu-id="674ad-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="674ad-108">Type</span></span>   | <span data-ttu-id="674ad-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="674ad-109">Description</span></span>                                               |
| :---------- | :----- | :-------------------------------------------------------- |
| <span data-ttu-id="674ad-110">imutávelid</span><span class="sxs-lookup"><span data-stu-id="674ad-110">immutableId</span></span> | <span data-ttu-id="674ad-111">String</span><span class="sxs-lookup"><span data-stu-id="674ad-111">String</span></span> | <span data-ttu-id="674ad-112">Identificador exclusivo do objeto de usuário no Active Directory.</span><span class="sxs-lookup"><span data-stu-id="674ad-112">Unique identifier for the user object in Active Directory.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="674ad-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="674ad-113">JSON representation</span></span>

<span data-ttu-id="674ad-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="674ad-114">The following is a JSON representation of the resource.</span></span>

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
