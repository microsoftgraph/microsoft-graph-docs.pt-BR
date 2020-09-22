---
title: tipo de recurso educationWordResource
description: 'Uma subclasse de educationResource. Este é um recurso de documento do Word. O arquivo do Word deve ser carregado no diretório **fileresource** associado ao '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 69339b3192a37c286f430a4b65c1aee64a9cbab5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055565"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="d2bbd-105">tipo de recurso educationWordResource</span><span class="sxs-lookup"><span data-stu-id="d2bbd-105">educationWordResource resource type</span></span>

<span data-ttu-id="d2bbd-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2bbd-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2bbd-107">Uma subclasse de [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="d2bbd-107">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="d2bbd-108">Este é um recurso de documento do Word.</span><span class="sxs-lookup"><span data-stu-id="d2bbd-108">This is a Word document resource.</span></span> <span data-ttu-id="d2bbd-109">O arquivo do Word deve ser carregado no diretório **fileresource** associado à atribuição ou ao envio.</span><span class="sxs-lookup"><span data-stu-id="d2bbd-109">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="d2bbd-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2bbd-110">Properties</span></span>
| <span data-ttu-id="d2bbd-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2bbd-111">Property</span></span>     | <span data-ttu-id="d2bbd-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2bbd-112">Type</span></span>   |<span data-ttu-id="d2bbd-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2bbd-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2bbd-114">fileUrl</span><span class="sxs-lookup"><span data-stu-id="d2bbd-114">fileUrl</span></span>|<span data-ttu-id="d2bbd-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2bbd-115">String</span></span>|<span data-ttu-id="d2bbd-116">Local do arquivo no disco.</span><span class="sxs-lookup"><span data-stu-id="d2bbd-116">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d2bbd-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2bbd-117">JSON representation</span></span>

<span data-ttu-id="d2bbd-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d2bbd-118">The following is a JSON representation of the resource.</span></span>

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


