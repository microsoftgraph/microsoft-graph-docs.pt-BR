---
title: Tipo de recurso educationExcelResource
description: Uma subclasse de educationResource. Esse tipo de recurso representa um Excel documento.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9345bb39f16066b4c5eee688d781e99563147ef2
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912112"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="41653-104">Tipo de recurso educationExcelResource</span><span class="sxs-lookup"><span data-stu-id="41653-104">educationExcelResource resource type</span></span>

<span data-ttu-id="41653-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41653-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="41653-106">Uma subclasse [de educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="41653-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="41653-107">Esse tipo de recurso representa um Excel documento.</span><span class="sxs-lookup"><span data-stu-id="41653-107">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="41653-108">**Observação:** O Excel arquivo deve estar na pasta de recursos associada ao objeto de atribuição ou envio ao qual esse recurso pertence.</span><span class="sxs-lookup"><span data-stu-id="41653-108">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="41653-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41653-109">Properties</span></span>
| <span data-ttu-id="41653-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41653-110">Property</span></span>     | <span data-ttu-id="41653-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="41653-111">Type</span></span>   |<span data-ttu-id="41653-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="41653-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41653-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="41653-113">fileUrl</span></span>|<span data-ttu-id="41653-114">String</span><span class="sxs-lookup"><span data-stu-id="41653-114">String</span></span>|<span data-ttu-id="41653-115">Ponteiro para o objeto Excel arquivo.</span><span class="sxs-lookup"><span data-stu-id="41653-115">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="41653-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41653-116">JSON representation</span></span>

<span data-ttu-id="41653-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="41653-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationExcelResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationExcelResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


