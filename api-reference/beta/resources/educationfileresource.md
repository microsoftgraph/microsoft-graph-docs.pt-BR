---
title: tipo de recurso de educationFileResource
description: Uma subclasse de educationResource que representa um objeto de arquivo que está associado a atribuição ou o envio.  Nesse caso, o arquivo não é um dos arquivos especiais (Word, Excel e assim por diante), mas é um arquivo que não tem manipulação especial dentro do sistema. O recurso de arquivo deve ser armazenado em **resourceFolder** que está associado a atribuição ou o envio que este recurso está anexado.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 15ca31576618f15e64b85d860077785160c25989
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520792"
---
# <a name="educationfileresource-resource-type"></a><span data-ttu-id="86892-105">tipo de recurso de educationFileResource</span><span class="sxs-lookup"><span data-stu-id="86892-105">educationFileResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86892-106">Uma subclasse de [educationResource](educationresource.md) que representa um objeto de arquivo que está associado a atribuição ou o envio.</span><span class="sxs-lookup"><span data-stu-id="86892-106">A subclass of [educationResource](educationresource.md) that represents a file object that is associated with the assignment or submission.</span></span>  <span data-ttu-id="86892-107">Nesse caso, o arquivo não é um dos arquivos especiais (Word, Excel e assim por diante), mas é um arquivo que não tem manipulação especial dentro do sistema.</span><span class="sxs-lookup"><span data-stu-id="86892-107">In this case, the file is not one of the special files (Word, Excel, and so on) but is a file that does not have special handling within the system.</span></span> <span data-ttu-id="86892-108">O recurso de arquivo deve ser armazenado em **resourceFolder** que está associado a atribuição ou o envio que este recurso está anexado.</span><span class="sxs-lookup"><span data-stu-id="86892-108">The file resource must be stored in the **resourceFolder** that is associated with the assignment or submission this resource is attached to.</span></span>

## <a name="properties"></a><span data-ttu-id="86892-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="86892-109">Properties</span></span>
| <span data-ttu-id="86892-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86892-110">Property</span></span>     | <span data-ttu-id="86892-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="86892-111">Type</span></span>   |<span data-ttu-id="86892-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="86892-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86892-113">FileURL</span><span class="sxs-lookup"><span data-stu-id="86892-113">fileUrl</span></span>|<span data-ttu-id="86892-114">String</span><span class="sxs-lookup"><span data-stu-id="86892-114">String</span></span>|<span data-ttu-id="86892-115">Local no disco do recurso de arquivo.</span><span class="sxs-lookup"><span data-stu-id="86892-115">Location on disk of the file resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="86892-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="86892-116">JSON representation</span></span>

<span data-ttu-id="86892-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="86892-117">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationfileresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
