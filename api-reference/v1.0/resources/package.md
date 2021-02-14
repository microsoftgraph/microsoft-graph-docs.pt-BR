---
author: JeremyKelley
ms.date: 09/10/2017
title: Pacote
localization_priority: Normal
description: " ou uma coleção de itens que devem ser tratados como uma coleção em vez de itens individuais."
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e248c74add209690dbd7c3cc11d8056c5ca30dcc
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239811"
---
# <a name="package-resource-type"></a><span data-ttu-id="f6a55-103">Tipo de recurso Package</span><span class="sxs-lookup"><span data-stu-id="f6a55-103">Package resource type</span></span>

<span data-ttu-id="f6a55-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6a55-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f6a55-105">O recurso **Package** indica que um DriveItem é o item de nível superior em um "pacote" ou uma coleção de itens que devem ser tratados como uma coleção, em vez de itens individuais.</span><span class="sxs-lookup"><span data-stu-id="f6a55-105">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="f6a55-p101">Um exemplo de um pacote é um bloco de anotações do OneNote. Embora o bloco de anotações seja composto de arquivos e pastas que representam o conteúdo do bloco de anotações, o item de nível superior que representa o bloco de anotações tem uma faceta **package** para indicar aos clientes que se trata de uma coleção de dados que deve ser tratada de forma especial.</span><span class="sxs-lookup"><span data-stu-id="f6a55-p101">An example of a package is a OneNote notebook. While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="f6a55-108">DriveItems com a faceta **package** não incluem uma faceta **folder** ou **file**, mas são conceitualmente semelhantes a um item com uma faceta **folder**.</span><span class="sxs-lookup"><span data-stu-id="f6a55-108">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6a55-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f6a55-109">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

## <a name="properties"></a><span data-ttu-id="f6a55-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f6a55-110">Properties</span></span>

| <span data-ttu-id="f6a55-111">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="f6a55-111">Property Name</span></span> | <span data-ttu-id="f6a55-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6a55-112">Type</span></span>   | <span data-ttu-id="f6a55-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6a55-113">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f6a55-114">type</span><span class="sxs-lookup"><span data-stu-id="f6a55-114">type</span></span>          | <span data-ttu-id="f6a55-115">string</span><span class="sxs-lookup"><span data-stu-id="f6a55-115">string</span></span> | <span data-ttu-id="f6a55-116">Uma cadeia de caracteres indicando o tipo de pacote.</span><span class="sxs-lookup"><span data-stu-id="f6a55-116">A string indicating the type of package.</span></span> <span data-ttu-id="f6a55-117">Embora `oneNote` seja o único valor definido atualmente, você deve esperar que outros tipos de pacote sejam retornados e lidar com eles da forma apropriada.</span><span class="sxs-lookup"><span data-stu-id="f6a55-117">While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="f6a55-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="f6a55-118">Remarks</span></span> 

<span data-ttu-id="f6a55-119">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="f6a55-119">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "tocPath": "Facets/Package"
} -->

