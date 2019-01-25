---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Pacote
localization_priority: Normal
ms.openlocfilehash: 67e82faa3f51eeae71c2dcb22ecb7a973e2070bb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516599"
---
# <a name="package-resource-type"></a><span data-ttu-id="54076-102">Tipo de recurso Package</span><span class="sxs-lookup"><span data-stu-id="54076-102">Package resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54076-103">O recurso **Package** indica que um DriveItem é o item de nível superior em um "pacote" ou uma coleção de itens que devem ser tratados como uma coleção, em vez de itens individuais.</span><span class="sxs-lookup"><span data-stu-id="54076-103">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="54076-p101">Um exemplo de um pacote é um bloco de anotações do OneNote. Embora o bloco de anotações seja composto de arquivos e pastas que representam o conteúdo do bloco de anotações, o item de nível superior que representa o bloco de anotações tem uma faceta **Pacote** para indicar aos clientes que se trata de uma coleção de dados que deve ser tratada de forma especial.</span><span class="sxs-lookup"><span data-stu-id="54076-p101">An example of a package is a OneNote notebook. While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="54076-106">DriveItems com a faceta **package** não incluem uma faceta **folder** ou **file**, mas são conceitualmente semelhantes a um item com uma faceta **folder**.</span><span class="sxs-lookup"><span data-stu-id="54076-106">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="54076-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="54076-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

| <span data-ttu-id="54076-108">Nome da Propriedade</span><span class="sxs-lookup"><span data-stu-id="54076-108">Property Name</span></span> | <span data-ttu-id="54076-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="54076-109">Type</span></span>   | <span data-ttu-id="54076-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="54076-110">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="54076-111">**type**</span><span class="sxs-lookup"><span data-stu-id="54076-111">**type**</span></span>      | <span data-ttu-id="54076-112">string</span><span class="sxs-lookup"><span data-stu-id="54076-112">string</span></span> | <span data-ttu-id="54076-p102">Uma cadeia de caracteres indicando o tipo de pacote. Embora `oneNote` seja o único valor definido atualmente, você deve esperar que outros tipos de pacote sejam retornados e lidar com eles da forma apropriada.</span><span class="sxs-lookup"><span data-stu-id="54076-p102">An string indicating the type of package. While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="54076-115">Comentários</span><span class="sxs-lookup"><span data-stu-id="54076-115">Remarks</span></span> 

<span data-ttu-id="54076-116">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="54076-116">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/beta/resources/package.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
