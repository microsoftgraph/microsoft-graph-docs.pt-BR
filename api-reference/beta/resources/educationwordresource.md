---
title: tipo de recurso educationWordResource
description: 'Uma subclasse de educationResource. Este é um recurso de documento do Word. O arquivo do Word deve ser carregado no diretório **fileresource** associado ao '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 06b1f097199bbf188c0bc0a538fe471b07cdec91
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499943"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="023d7-105">tipo de recurso educationWordResource</span><span class="sxs-lookup"><span data-stu-id="023d7-105">educationWordResource resource type</span></span>

<span data-ttu-id="023d7-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="023d7-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="023d7-107">Uma subclasse de [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="023d7-107">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="023d7-108">Este é um recurso de documento do Word.</span><span class="sxs-lookup"><span data-stu-id="023d7-108">This is a Word document resource.</span></span> <span data-ttu-id="023d7-109">O arquivo do Word deve ser carregado no diretório **fileresource** associado à atribuição ou ao envio.</span><span class="sxs-lookup"><span data-stu-id="023d7-109">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="023d7-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="023d7-110">Properties</span></span>
| <span data-ttu-id="023d7-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="023d7-111">Property</span></span>     | <span data-ttu-id="023d7-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="023d7-112">Type</span></span>   |<span data-ttu-id="023d7-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="023d7-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="023d7-114">fileUrl</span><span class="sxs-lookup"><span data-stu-id="023d7-114">fileUrl</span></span>|<span data-ttu-id="023d7-115">String</span><span class="sxs-lookup"><span data-stu-id="023d7-115">String</span></span>|<span data-ttu-id="023d7-116">Local do arquivo no disco.</span><span class="sxs-lookup"><span data-stu-id="023d7-116">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="023d7-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="023d7-117">JSON representation</span></span>

<span data-ttu-id="023d7-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="023d7-118">The following is a JSON representation of the resource.</span></span>

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
