---
title: tipo de recurso educationAssignmentIndividualRecipient
description: 'Usada dentro da propriedade assignment. assignTo. Quando definido como lista de destinatários individuais, os alunos selecionados na classe serão '
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 7408382cadcb53d857bb36b06702f7857d64a8f4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006448"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a><span data-ttu-id="1414d-104">tipo de recurso educationAssignmentIndividualRecipient</span><span class="sxs-lookup"><span data-stu-id="1414d-104">educationAssignmentIndividualRecipient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1414d-105">Usada dentro da propriedade [assignment.](educationassignment.md) assignTo.</span><span class="sxs-lookup"><span data-stu-id="1414d-105">Used inside the [assignment.assignTo](educationassignment.md) property.</span></span> <span data-ttu-id="1414d-106">Quando definido como lista de destinatários individuais, os alunos selecionados na classe receberão um objeto de envio quando a atribuição for publicada.</span><span class="sxs-lookup"><span data-stu-id="1414d-106">When set to individual recipient list, selected students in the class will receive a submission object when the assignment is published.</span></span>

<span data-ttu-id="1414d-107">Esse recurso é uma subclasse de [educationAssignmentRecipient](educationassignmentrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="1414d-107">This resource is a subclass of [educationAssignmentRecipient](educationassignmentrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1414d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1414d-108">Properties</span></span>
| <span data-ttu-id="1414d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1414d-109">Property</span></span>     | <span data-ttu-id="1414d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1414d-110">Type</span></span>   |<span data-ttu-id="1414d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1414d-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1414d-112">recipients</span><span class="sxs-lookup"><span data-stu-id="1414d-112">recipients</span></span>|<span data-ttu-id="1414d-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1414d-113">String collection</span></span>|<span data-ttu-id="1414d-114">Uma coleção de IDs dos destinatários.</span><span class="sxs-lookup"><span data-stu-id="1414d-114">A collection of ids of the recipients.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1414d-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1414d-115">JSON representation</span></span>

<span data-ttu-id="1414d-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1414d-116">The following is a JSON representation of the resource.</span></span>

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
