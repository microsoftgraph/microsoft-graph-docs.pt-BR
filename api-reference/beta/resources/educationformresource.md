---
title: tipo de recurso educationFormResource
description: Uma subclasse de educationResource. Este recurso é um formulário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d2e10ea6db0236b7deff3581c2e1b4f97c589045
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972709"
---
# <a name="educationformresource-resource-type"></a><span data-ttu-id="68988-104">tipo de recurso educationFormResource</span><span class="sxs-lookup"><span data-stu-id="68988-104">educationFormResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68988-105">Uma subclasse de [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="68988-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="68988-106">Este recurso é um formulário.</span><span class="sxs-lookup"><span data-stu-id="68988-106">This resource is a form.</span></span>


## <a name="properties"></a><span data-ttu-id="68988-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="68988-107">Properties</span></span>
| <span data-ttu-id="68988-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68988-108">Property</span></span>     | <span data-ttu-id="68988-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="68988-109">Type</span></span>   |<span data-ttu-id="68988-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="68988-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68988-111">originalFormId</span><span class="sxs-lookup"><span data-stu-id="68988-111">originalFormId</span></span>|<span data-ttu-id="68988-112">String</span><span class="sxs-lookup"><span data-stu-id="68988-112">String</span></span>|<span data-ttu-id="68988-113">ID original do formulário.</span><span class="sxs-lookup"><span data-stu-id="68988-113">Original id of the Form.</span></span>|
|<span data-ttu-id="68988-114">formId</span><span class="sxs-lookup"><span data-stu-id="68988-114">formId</span></span>|<span data-ttu-id="68988-115">String</span><span class="sxs-lookup"><span data-stu-id="68988-115">String</span></span>|<span data-ttu-id="68988-116">ID do formulário.</span><span class="sxs-lookup"><span data-stu-id="68988-116">Id of the Form.</span></span>|
|<span data-ttu-id="68988-117">isGroupForm</span><span class="sxs-lookup"><span data-stu-id="68988-117">isGroupForm</span></span>|<span data-ttu-id="68988-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="68988-118">Boolean</span></span>|<span data-ttu-id="68988-119">Se o formulário pertence a um grupo de classe.</span><span class="sxs-lookup"><span data-stu-id="68988-119">Whether the Form belongs to a class group.</span></span>|
|<span data-ttu-id="68988-120">viewUrl</span><span class="sxs-lookup"><span data-stu-id="68988-120">viewUrl</span></span>|<span data-ttu-id="68988-121">String</span><span class="sxs-lookup"><span data-stu-id="68988-121">String</span></span>|<span data-ttu-id="68988-122">URL do aluno para o formulário.</span><span class="sxs-lookup"><span data-stu-id="68988-122">Student URL for the Form.</span></span>|
|<span data-ttu-id="68988-123">viewUrl</span><span class="sxs-lookup"><span data-stu-id="68988-123">viewUrl</span></span>|<span data-ttu-id="68988-124">String</span><span class="sxs-lookup"><span data-stu-id="68988-124">String</span></span>|<span data-ttu-id="68988-125">URL do aluno para o formulário.</span><span class="sxs-lookup"><span data-stu-id="68988-125">Student URL for the Form.</span></span>|
|<span data-ttu-id="68988-126">editUrl</span><span class="sxs-lookup"><span data-stu-id="68988-126">editUrl</span></span>|<span data-ttu-id="68988-127">String</span><span class="sxs-lookup"><span data-stu-id="68988-127">String</span></span>|<span data-ttu-id="68988-128">URL do professor para o formulário.</span><span class="sxs-lookup"><span data-stu-id="68988-128">Teacher URL for the Form.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="68988-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="68988-129">JSON representation</span></span>

<span data-ttu-id="68988-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="68988-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFormResource"
}-->

```json
{
  "originalFormId": "String",
  "formId": "String",
  "isGroupForm": "Boolean",
  "viewUrl": "String",
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
  "suppressions": []
}
-->
