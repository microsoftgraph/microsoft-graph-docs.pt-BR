---
title: tipo de recurso de educationExcelResource
description: 'Uma subclasse de educationResource. Esse tipo de recurso representa um documento do Excel.  '
ms.openlocfilehash: cdd86cf1048863ac3def2ae6be13c3f39b37e642
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040152"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="36050-104">tipo de recurso de educationExcelResource</span><span class="sxs-lookup"><span data-stu-id="36050-104">educationExcelResource resource type</span></span>

> <span data-ttu-id="36050-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="36050-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="36050-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="36050-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="36050-107">Uma subclasse de [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="36050-107">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="36050-108">Esse tipo de recurso representa um documento do Excel.</span><span class="sxs-lookup"><span data-stu-id="36050-108">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="36050-109">**Observação:** O arquivo do Excel deve estar na pasta de recursos associada ao objeto de envio ou atribuição ao qual este recurso pertence.</span><span class="sxs-lookup"><span data-stu-id="36050-109">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="36050-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="36050-110">Properties</span></span>
| <span data-ttu-id="36050-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36050-111">Property</span></span>     | <span data-ttu-id="36050-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="36050-112">Type</span></span>   |<span data-ttu-id="36050-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="36050-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36050-114">fileUrl</span><span class="sxs-lookup"><span data-stu-id="36050-114">fileUrl</span></span>|<span data-ttu-id="36050-115">String</span><span class="sxs-lookup"><span data-stu-id="36050-115">String</span></span>|<span data-ttu-id="36050-116">Ponteiro para o objeto de arquivo do Excel.</span><span class="sxs-lookup"><span data-stu-id="36050-116">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36050-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="36050-117">JSON representation</span></span>

<span data-ttu-id="36050-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="36050-118">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationExcelResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->