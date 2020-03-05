---
title: tipo de recurso educationSubmissionIndividualRecipient
description: 'Uma subclasse de educationSubmissionRecipient que indica que um envio é atribuído a um indivíduo na classe.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2954e511cee6929a66bb593c4f449f7410852c7f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500720"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a><span data-ttu-id="9af01-103">tipo de recurso educationSubmissionIndividualRecipient</span><span class="sxs-lookup"><span data-stu-id="9af01-103">educationSubmissionIndividualRecipient resource type</span></span>

<span data-ttu-id="9af01-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9af01-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9af01-105">Uma subclasse de [educationSubmissionRecipient](educationsubmissionrecipient.md) que indica que um envio é atribuído a um indivíduo na classe.</span><span class="sxs-lookup"><span data-stu-id="9af01-105">A subclass of [educationSubmissionRecipient](educationsubmissionrecipient.md) that indicates that a submission is assigned to an individual in the class.</span></span>  


## <a name="properties"></a><span data-ttu-id="9af01-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9af01-106">Properties</span></span>
| <span data-ttu-id="9af01-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9af01-107">Property</span></span>     | <span data-ttu-id="9af01-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9af01-108">Type</span></span>   |<span data-ttu-id="9af01-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9af01-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9af01-110">userId</span><span class="sxs-lookup"><span data-stu-id="9af01-110">userId</span></span>|<span data-ttu-id="9af01-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9af01-111">String</span></span>|<span data-ttu-id="9af01-112">ID de usuário do usuário para o qual o envio é atribuído.</span><span class="sxs-lookup"><span data-stu-id="9af01-112">User ID of the user to whom the submission is assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9af01-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9af01-113">JSON representation</span></span>

<span data-ttu-id="9af01-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9af01-114">The following is a JSON representation of the resource.</span></span>

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
