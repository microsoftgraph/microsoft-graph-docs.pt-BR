---
title: tipo de recurso educationSubmissionIndividualRecipient
description: 'Uma subclasse de educationSubmissionRecipient que indica que um envio é atribuído a um indivíduo na classe.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2eecdc7e7ddd30ecad9a520b42cd11df9565fa71
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972506"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a><span data-ttu-id="786f8-103">tipo de recurso educationSubmissionIndividualRecipient</span><span class="sxs-lookup"><span data-stu-id="786f8-103">educationSubmissionIndividualRecipient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="786f8-104">Uma subclasse de [educationSubmissionRecipient](educationsubmissionrecipient.md) que indica que um envio é atribuído a um indivíduo na classe.</span><span class="sxs-lookup"><span data-stu-id="786f8-104">A subclass of [educationSubmissionRecipient](educationsubmissionrecipient.md) that indicates that a submission is assigned to an individual in the class.</span></span>  


## <a name="properties"></a><span data-ttu-id="786f8-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="786f8-105">Properties</span></span>
| <span data-ttu-id="786f8-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="786f8-106">Property</span></span>     | <span data-ttu-id="786f8-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="786f8-107">Type</span></span>   |<span data-ttu-id="786f8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="786f8-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="786f8-109">userId</span><span class="sxs-lookup"><span data-stu-id="786f8-109">userId</span></span>|<span data-ttu-id="786f8-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="786f8-110">String</span></span>|<span data-ttu-id="786f8-111">ID de usuário do usuário para o qual o envio é atribuído.</span><span class="sxs-lookup"><span data-stu-id="786f8-111">User ID of the user to whom the submission is assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="786f8-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="786f8-112">JSON representation</span></span>

<span data-ttu-id="786f8-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="786f8-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmissionIndividualRecipient"
}-->

```json
{
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmissionIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
