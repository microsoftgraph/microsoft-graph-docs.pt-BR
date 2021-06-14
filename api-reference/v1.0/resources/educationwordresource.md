---
title: Tipo de recurso educationWordResource
description: Uma subclasse de educationResource.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1d28d37f34073488f7022d19ae227bb2af2fd306
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912179"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="ed25e-103">Tipo de recurso educationWordResource</span><span class="sxs-lookup"><span data-stu-id="ed25e-103">educationWordResource resource type</span></span>

<span data-ttu-id="ed25e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed25e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ed25e-105">Uma subclasse [de educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="ed25e-105">A subclass of [educationResource](educationresource.md).</span></span> 

<span data-ttu-id="ed25e-106">Este é um recurso de documento do Word.</span><span class="sxs-lookup"><span data-stu-id="ed25e-106">This is a Word document resource.</span></span> <span data-ttu-id="ed25e-107">O arquivo word deve ser carregado no **diretório fileResource** associado à atribuição ou ao envio.</span><span class="sxs-lookup"><span data-stu-id="ed25e-107">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="ed25e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed25e-108">Properties</span></span>
| <span data-ttu-id="ed25e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed25e-109">Property</span></span>     | <span data-ttu-id="ed25e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed25e-110">Type</span></span>   |<span data-ttu-id="ed25e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed25e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed25e-112">fileUrl</span><span class="sxs-lookup"><span data-stu-id="ed25e-112">fileUrl</span></span>|<span data-ttu-id="ed25e-113">String</span><span class="sxs-lookup"><span data-stu-id="ed25e-113">String</span></span>|<span data-ttu-id="ed25e-114">Local do arquivo no disco.</span><span class="sxs-lookup"><span data-stu-id="ed25e-114">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ed25e-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed25e-115">JSON representation</span></span>

<span data-ttu-id="ed25e-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed25e-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationWordResource"
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
  "description": "educationWordResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


