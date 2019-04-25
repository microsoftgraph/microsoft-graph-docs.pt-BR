---
title: tipo de recurso educationFileResource
description: Uma subclasse de educationResource que representa um objeto File associado à atribuição ou ao envio.  Nesse caso, o arquivo não é um dos arquivos especiais (Word, Excel e assim por diante), mas é um arquivo que não tem tratamento especial no sistema. O recurso de arquivo deve ser armazenado no **resourceFolder** que está associado à atribuição ou ao envio ao qual este recurso está anexado.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 15ca31576618f15e64b85d860077785160c25989
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542850"
---
# <a name="educationfileresource-resource-type"></a><span data-ttu-id="ac357-105">tipo de recurso educationFileResource</span><span class="sxs-lookup"><span data-stu-id="ac357-105">educationFileResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac357-106">Uma subclasse de [educationResource](educationresource.md) que representa um objeto File associado à atribuição ou ao envio.</span><span class="sxs-lookup"><span data-stu-id="ac357-106">A subclass of [educationResource](educationresource.md) that represents a file object that is associated with the assignment or submission.</span></span>  <span data-ttu-id="ac357-107">Nesse caso, o arquivo não é um dos arquivos especiais (Word, Excel e assim por diante), mas é um arquivo que não tem tratamento especial no sistema.</span><span class="sxs-lookup"><span data-stu-id="ac357-107">In this case, the file is not one of the special files (Word, Excel, and so on) but is a file that does not have special handling within the system.</span></span> <span data-ttu-id="ac357-108">O recurso de arquivo deve ser armazenado no **resourceFolder** que está associado à atribuição ou ao envio ao qual este recurso está anexado.</span><span class="sxs-lookup"><span data-stu-id="ac357-108">The file resource must be stored in the **resourceFolder** that is associated with the assignment or submission this resource is attached to.</span></span>

## <a name="properties"></a><span data-ttu-id="ac357-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac357-109">Properties</span></span>
| <span data-ttu-id="ac357-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac357-110">Property</span></span>     | <span data-ttu-id="ac357-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac357-111">Type</span></span>   |<span data-ttu-id="ac357-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac357-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac357-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="ac357-113">fileUrl</span></span>|<span data-ttu-id="ac357-114">String</span><span class="sxs-lookup"><span data-stu-id="ac357-114">String</span></span>|<span data-ttu-id="ac357-115">Local no disco do recurso de arquivo.</span><span class="sxs-lookup"><span data-stu-id="ac357-115">Location on disk of the file resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ac357-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac357-116">JSON representation</span></span>

<span data-ttu-id="ac357-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ac357-117">The following is a JSON representation of the resource.</span></span>

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
