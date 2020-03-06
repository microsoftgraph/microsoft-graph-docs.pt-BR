---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Arquivo
localization_priority: Normal
description: O recurso File agrupa itens de dados relacionados a arquivos em uma única estrutura.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c316e3b09f00ffebd7ebfab5e47b49c7df3980d3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532956"
---
# <a name="file-resource-type"></a><span data-ttu-id="ee75a-103">Tipo de recurso File</span><span class="sxs-lookup"><span data-stu-id="ee75a-103">File resource type</span></span>

<span data-ttu-id="ee75a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee75a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ee75a-105">O recurso **File** agrupa itens de dados relacionados a arquivos em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="ee75a-105">The **File** resource groups file-related data items into a single structure.</span></span>

<span data-ttu-id="ee75a-p101">Se um [**DriveItem**](driveitem.md) tiver uma faceta **file** não nula, o item representa um arquivo. Além de outras propriedades, os arquivos têm um relacionamento **content**, que contém o fluxo de bytes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="ee75a-p101">If a [**DriveItem**](driveitem.md) has a non-null **file** facet, the item represents an file. In addition to other properties, files have a **content** relationship which contains the byte stream of the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee75a-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee75a-108">JSON representation</span></span>

<span data-ttu-id="ee75a-109">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee75a-109">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.file"
}-->

```json
{
  "hashes": {"@odata.type": "microsoft.graph.hashes"},
  "mimeType": "string"
}
```

## <a name="properties"></a><span data-ttu-id="ee75a-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee75a-110">Properties</span></span>

| <span data-ttu-id="ee75a-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee75a-111">Property</span></span> | <span data-ttu-id="ee75a-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee75a-112">Type</span></span>                    | <span data-ttu-id="ee75a-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee75a-113">Description</span></span>                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ee75a-114">hashes</span><span class="sxs-lookup"><span data-stu-id="ee75a-114">hashes</span></span>   | [<span data-ttu-id="ee75a-115">Hashes</span><span class="sxs-lookup"><span data-stu-id="ee75a-115">Hashes</span></span>](hashes.md) | <span data-ttu-id="ee75a-p102">Hash do conteúdo binário do arquivo, se houver. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee75a-p102">Hashes of the file's binary content, if available. Read-only.</span></span>                                                                                    |
| <span data-ttu-id="ee75a-118">mimeType</span><span class="sxs-lookup"><span data-stu-id="ee75a-118">mimeType</span></span> | <span data-ttu-id="ee75a-119">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee75a-119">string</span></span>                  | <span data-ttu-id="ee75a-p103">O tipo MIME para o arquivo. Determinado pela lógica no servidor e pode não ser o valor fornecido quando o arquivo foi carregado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee75a-p103">The MIME type for the file. This is determined by logic on the server and might not be the value provided when the file was uploaded. Read-only.</span></span> |

## <a name="remarks"></a><span data-ttu-id="ee75a-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="ee75a-123">Remarks</span></span> 

<span data-ttu-id="ee75a-124">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ee75a-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File"
} -->
