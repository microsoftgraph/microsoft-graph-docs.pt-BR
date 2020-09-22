---
title: tipo de recurso educationFileResource
description: Uma subclasse de educationResource que representa um objeto File associado à atribuição ou ao envio.  Nesse caso, o arquivo não é um dos arquivos especiais (Word, Excel e assim por diante), mas é um arquivo que não tem tratamento especial no sistema. O recurso de arquivo deve ser armazenado no **resourceFolder** que está associado à atribuição ou ao envio ao qual este recurso está anexado.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: cafef836f1e6f6fb4c2e379f9b9ad618f2519f72
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095435"
---
# <a name="educationfileresource-resource-type"></a><span data-ttu-id="6b4dd-105">tipo de recurso educationFileResource</span><span class="sxs-lookup"><span data-stu-id="6b4dd-105">educationFileResource resource type</span></span>

<span data-ttu-id="6b4dd-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b4dd-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b4dd-107">Uma subclasse de [educationResource](educationresource.md) que representa um objeto File associado à atribuição ou ao envio.</span><span class="sxs-lookup"><span data-stu-id="6b4dd-107">A subclass of [educationResource](educationresource.md) that represents a file object that is associated with the assignment or submission.</span></span>  <span data-ttu-id="6b4dd-108">Nesse caso, o arquivo não é um dos arquivos especiais (Word, Excel e assim por diante), mas é um arquivo que não tem tratamento especial no sistema.</span><span class="sxs-lookup"><span data-stu-id="6b4dd-108">In this case, the file is not one of the special files (Word, Excel, and so on) but is a file that does not have special handling within the system.</span></span> <span data-ttu-id="6b4dd-109">O recurso de arquivo deve ser armazenado no **resourceFolder** que está associado à atribuição ou ao envio ao qual este recurso está anexado.</span><span class="sxs-lookup"><span data-stu-id="6b4dd-109">The file resource must be stored in the **resourceFolder** that is associated with the assignment or submission this resource is attached to.</span></span>

## <a name="properties"></a><span data-ttu-id="6b4dd-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b4dd-110">Properties</span></span>
| <span data-ttu-id="6b4dd-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b4dd-111">Property</span></span>     | <span data-ttu-id="6b4dd-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b4dd-112">Type</span></span>   |<span data-ttu-id="6b4dd-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b4dd-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b4dd-114">fileUrl</span><span class="sxs-lookup"><span data-stu-id="6b4dd-114">fileUrl</span></span>|<span data-ttu-id="6b4dd-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b4dd-115">String</span></span>|<span data-ttu-id="6b4dd-116">Local no disco do recurso de arquivo.</span><span class="sxs-lookup"><span data-stu-id="6b4dd-116">Location on disk of the file resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b4dd-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b4dd-117">JSON representation</span></span>

<span data-ttu-id="6b4dd-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6b4dd-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileResource"
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
  "description": "educationFileResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


