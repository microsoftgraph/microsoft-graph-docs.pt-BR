---
title: tipo de recurso de educationSubmissionIndividualRecipient
description: 'Uma subclasse de educationSubmissionRecipient que indica que um envio é atribuído a um indivíduo na classe.  '
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: 109919afbbc9fced24b46dede09c3a92df4f8c17
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866791"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a><span data-ttu-id="a6542-103">tipo de recurso de educationSubmissionIndividualRecipient</span><span class="sxs-lookup"><span data-stu-id="a6542-103">educationSubmissionIndividualRecipient resource type</span></span>

> <span data-ttu-id="a6542-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a6542-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6542-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a6542-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6542-106">Uma subclasse de [educationSubmissionRecipient](educationsubmissionrecipient.md) que indica que um envio é atribuído a um indivíduo na classe.</span><span class="sxs-lookup"><span data-stu-id="a6542-106">A subclass of [educationSubmissionRecipient](educationsubmissionrecipient.md) that indicates that a submission is assigned to an individual in the class.</span></span>  


## <a name="properties"></a><span data-ttu-id="a6542-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a6542-107">Properties</span></span>
| <span data-ttu-id="a6542-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6542-108">Property</span></span>     | <span data-ttu-id="a6542-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6542-109">Type</span></span>   |<span data-ttu-id="a6542-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6542-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6542-111">userId</span><span class="sxs-lookup"><span data-stu-id="a6542-111">userId</span></span>|<span data-ttu-id="a6542-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6542-112">String</span></span>|<span data-ttu-id="a6542-113">ID de usuário do usuário ao qual o envio é atribuído.</span><span class="sxs-lookup"><span data-stu-id="a6542-113">User ID of the user to whom the submission is assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6542-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a6542-114">JSON representation</span></span>

<span data-ttu-id="a6542-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a6542-115">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmissionIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
