---
author: JeremyKelley
description: Grupos de itens de dados especiais relacionados a pastas em uma única estrutura.
title: Tipo de recurso specialFolder
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: d9552c79588f8533980879c2ed49ed32fdfe7927
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236268"
---
# <a name="specialfolder-resource-type"></a><span data-ttu-id="d57f5-103">Tipo de recurso specialFolder</span><span class="sxs-lookup"><span data-stu-id="d57f5-103">specialFolder resource type</span></span>

<span data-ttu-id="d57f5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d57f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d57f5-105">Grupos de itens de dados especiais relacionados a pastas em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="d57f5-105">Groups special folder-related data items into a single structure.</span></span>

<span data-ttu-id="d57f5-106">Se um **driveItem** tiver uma faceta **especialFolder** não nula, o item representará uma pasta especial (nomeada).</span><span class="sxs-lookup"><span data-stu-id="d57f5-106">If a **driveItem** has a non-null **specialFolder** facet, the item represents a special (named) folder.</span></span>
<span data-ttu-id="d57f5-107">Pastas especiais que podem ser acessadas diretamente por meio da [coleção de pastas especiais](../api/drive-get-specialfolder.md).</span><span class="sxs-lookup"><span data-stu-id="d57f5-107">Special folders can be accessed directly via the [special folders collection](../api/drive-get-specialfolder.md).</span></span>

<span data-ttu-id="d57f5-p102">Pastas especiais fornecem aliases simples para acessar pastas conhecidas sem a necessidade de pesquisar a pasta pelo caminho (o que exigiria a localização) ou fazer referência à pasta com uma ID. Se uma pasta especial for renomeada ou movida para outro local na unidade de disco, esta sintaxe continuará a retornar a pasta.</span><span class="sxs-lookup"><span data-stu-id="d57f5-p102">Special folders provide simple aliases to access well-known folders without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to return that folder.</span></span>

<span data-ttu-id="d57f5-p103">As pastas especiais são criadas automaticamente na primeira vez que um aplicativo tenta gravar em uma, caso ainda não existam. Se um usuário excluir uma, ela será recriada quando algo for gravado nela novamente.</span><span class="sxs-lookup"><span data-stu-id="d57f5-p103">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

[!INCLUDE [files-special-folder-list](../includes/files-special-folder-list.md)]

><span data-ttu-id="d57f5-112">**Observação:** Se seu aplicativo solicitou apenas o escopo **Files.Read** e solicitar uma pasta especial que não exista, a resposta será um erro `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="d57f5-112">**Note:** If your app has only requested **Files.Read** scope and requests a special folder that doesn't exist, the response will be a `403 Forbidden` error.</span></span>

## <a name="properties"></a><span data-ttu-id="d57f5-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d57f5-113">Properties</span></span>

| <span data-ttu-id="d57f5-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d57f5-114">Property</span></span>  | <span data-ttu-id="d57f5-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="d57f5-115">Type</span></span>   | <span data-ttu-id="d57f5-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="d57f5-116">Description</span></span>                                                            |
|:----------|:-------|:-----------------------------------------------------------------------|
| <span data-ttu-id="d57f5-117">nome</span><span class="sxs-lookup"><span data-stu-id="d57f5-117">name</span></span>      | <span data-ttu-id="d57f5-118">string</span><span class="sxs-lookup"><span data-stu-id="d57f5-118">string</span></span> | <span data-ttu-id="d57f5-119">O identificador exclusivo deste item na coleção `/drive/special`</span><span class="sxs-lookup"><span data-stu-id="d57f5-119">The unique identifier for this item in the `/drive/special` collection</span></span> |


## <a name="json-representation"></a><span data-ttu-id="d57f5-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d57f5-120">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.specialFolder"
}-->
```json
{
  "name": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="d57f5-121">Confira também</span><span class="sxs-lookup"><span data-stu-id="d57f5-121">See also</span></span> 

<span data-ttu-id="d57f5-122">Para obter mais informações sobre as facetas em um driveItem, [consulte driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="d57f5-122">For more information about the facets on a driveItem, see [driveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The SpecialFolder facet provides information about folders accessible as special folders.",
  "keywords": "special folder,item,facet",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


