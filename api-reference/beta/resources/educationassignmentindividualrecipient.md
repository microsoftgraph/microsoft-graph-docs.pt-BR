---
title: tipo de recurso educationAssignmentIndividualRecipient
description: 'Usada dentro da propriedade assignment. assignTo. Quando definido como lista de destinatários individuais, os alunos selecionados na classe serão '
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 695145ae8819efc66df29d752e7a95101c9fef9e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013710"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a><span data-ttu-id="16c9e-104">tipo de recurso educationAssignmentIndividualRecipient</span><span class="sxs-lookup"><span data-stu-id="16c9e-104">educationAssignmentIndividualRecipient resource type</span></span>

<span data-ttu-id="16c9e-105">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="16c9e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16c9e-106">Usada dentro da propriedade [assignment. assignTo](educationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="16c9e-106">Used inside the [assignment.assignTo](educationassignment.md) property.</span></span> <span data-ttu-id="16c9e-107">Quando definido como lista de destinatários individuais, os alunos selecionados na classe receberão um objeto de envio quando a atribuição for publicada.</span><span class="sxs-lookup"><span data-stu-id="16c9e-107">When set to individual recipient list, selected students in the class will receive a submission object when the assignment is published.</span></span>

<span data-ttu-id="16c9e-108">Esse recurso é uma subclasse de [educationAssignmentRecipient](educationassignmentrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="16c9e-108">This resource is a subclass of [educationAssignmentRecipient](educationassignmentrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="16c9e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="16c9e-109">Properties</span></span>
| <span data-ttu-id="16c9e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16c9e-110">Property</span></span>     | <span data-ttu-id="16c9e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="16c9e-111">Type</span></span>   |<span data-ttu-id="16c9e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="16c9e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16c9e-113">destinatários</span><span class="sxs-lookup"><span data-stu-id="16c9e-113">recipients</span></span>|<span data-ttu-id="16c9e-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="16c9e-114">String collection</span></span>|<span data-ttu-id="16c9e-115">Uma coleção de IDs dos destinatários.</span><span class="sxs-lookup"><span data-stu-id="16c9e-115">A collection of ids of the recipients.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="16c9e-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="16c9e-116">JSON representation</span></span>

<span data-ttu-id="16c9e-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="16c9e-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentIndividualRecipient"
}-->

```json
{
  "recipients": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


