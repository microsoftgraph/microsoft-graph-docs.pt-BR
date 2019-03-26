---
title: tipo de recurso educationFormResource
description: Uma subclasse de educationResource. Este recurso é um formulário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5e0b03eeea8c0e9d22a9f7279c821f6d90211470
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/26/2019
ms.locfileid: "30800951"
---
# <a name="educationformresource-resource-type"></a><span data-ttu-id="f95bd-104">tipo de recurso educationFormResource</span><span class="sxs-lookup"><span data-stu-id="f95bd-104">educationFormResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f95bd-105">Uma subclasse de [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="f95bd-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="f95bd-106">Este recurso é um formulário.</span><span class="sxs-lookup"><span data-stu-id="f95bd-106">This resource is a form.</span></span>


## <a name="properties"></a><span data-ttu-id="f95bd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f95bd-107">Properties</span></span>
| <span data-ttu-id="f95bd-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f95bd-108">Property</span></span>     | <span data-ttu-id="f95bd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f95bd-109">Type</span></span>   |<span data-ttu-id="f95bd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f95bd-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f95bd-111">originalFormId</span><span class="sxs-lookup"><span data-stu-id="f95bd-111">originalFormId</span></span>|<span data-ttu-id="f95bd-112">String</span><span class="sxs-lookup"><span data-stu-id="f95bd-112">String</span></span>|<span data-ttu-id="f95bd-113">ID original do formulário.</span><span class="sxs-lookup"><span data-stu-id="f95bd-113">Original id of the Form.</span></span>|
|<span data-ttu-id="f95bd-114">formId</span><span class="sxs-lookup"><span data-stu-id="f95bd-114">formId</span></span>|<span data-ttu-id="f95bd-115">String</span><span class="sxs-lookup"><span data-stu-id="f95bd-115">String</span></span>|<span data-ttu-id="f95bd-116">ID do formulário.</span><span class="sxs-lookup"><span data-stu-id="f95bd-116">Id of the Form.</span></span>|
|<span data-ttu-id="f95bd-117">isGroupForm</span><span class="sxs-lookup"><span data-stu-id="f95bd-117">isGroupForm</span></span>|<span data-ttu-id="f95bd-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="f95bd-118">Boolean</span></span>|<span data-ttu-id="f95bd-119">Se o formulário pertence a um grupo de classe.</span><span class="sxs-lookup"><span data-stu-id="f95bd-119">Whether the Form belongs to a class group.</span></span>|
|<span data-ttu-id="f95bd-120">viewUrl</span><span class="sxs-lookup"><span data-stu-id="f95bd-120">viewUrl</span></span>|<span data-ttu-id="f95bd-121">String</span><span class="sxs-lookup"><span data-stu-id="f95bd-121">String</span></span>|<span data-ttu-id="f95bd-122">URL do aluno para o formulário.</span><span class="sxs-lookup"><span data-stu-id="f95bd-122">Student URL for the Form.</span></span>|
|<span data-ttu-id="f95bd-123">viewUrl</span><span class="sxs-lookup"><span data-stu-id="f95bd-123">viewUrl</span></span>|<span data-ttu-id="f95bd-124">String</span><span class="sxs-lookup"><span data-stu-id="f95bd-124">String</span></span>|<span data-ttu-id="f95bd-125">URL do aluno para o formulário.</span><span class="sxs-lookup"><span data-stu-id="f95bd-125">Student URL for the Form.</span></span>|
|<span data-ttu-id="f95bd-126">editUrl</span><span class="sxs-lookup"><span data-stu-id="f95bd-126">editUrl</span></span>|<span data-ttu-id="f95bd-127">String</span><span class="sxs-lookup"><span data-stu-id="f95bd-127">String</span></span>|<span data-ttu-id="f95bd-128">URL do professor para o formulário.</span><span class="sxs-lookup"><span data-stu-id="f95bd-128">Teacher URL for the Form.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f95bd-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f95bd-129">JSON representation</span></span>

<span data-ttu-id="f95bd-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f95bd-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFormResource"
}-->

```json
{
  "originalFormId": "String"
  "formId": "String"
  "isGroupForm": "Boolean"
  "viewUrl": "String"
  "editUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationFormResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationformresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
