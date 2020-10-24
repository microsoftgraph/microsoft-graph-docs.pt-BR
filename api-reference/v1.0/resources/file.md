---
author: JeremyKelley
ms.date: 09/10/2017
title: Tipo de recurso File
localization_priority: Normal
description: O recurso File agrupa itens de dados relacionados a arquivos em uma única estrutura.
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: c19f2afce6128c7fb29a81c6e8d8f2d1c08c7913
ms.sourcegitcommit: ab578b062c534db57844490f35e802df8a8f4dfa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/24/2020
ms.locfileid: "48753392"
---
# <a name="file-resource-type"></a><span data-ttu-id="0589c-103">Tipo de recurso File</span><span class="sxs-lookup"><span data-stu-id="0589c-103">File resource type</span></span>

<span data-ttu-id="0589c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0589c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0589c-105">O recurso **File** agrupa itens de dados relacionados a arquivos em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="0589c-105">The **File** resource groups file-related data items into a single structure.</span></span>

<span data-ttu-id="0589c-106">Se um [**DriveItem**](driveitem.md) tiver uma faceta **File** não nula, o item representa um arquivo.</span><span class="sxs-lookup"><span data-stu-id="0589c-106">If a [**DriveItem**](driveitem.md) has a non-null **file** facet, the item represents a file.</span></span>
<span data-ttu-id="0589c-107">Além de outras propriedades, os arquivos têm um relacionamento **content**, que contém o fluxo de bytes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="0589c-107">In addition to other properties, files have a **content** relationship which contains the byte stream of the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0589c-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0589c-108">JSON representation</span></span>

<span data-ttu-id="0589c-109">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0589c-109">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="0589c-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0589c-110">Properties</span></span>

| <span data-ttu-id="0589c-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0589c-111">Property</span></span> | <span data-ttu-id="0589c-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="0589c-112">Type</span></span>                    | <span data-ttu-id="0589c-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="0589c-113">Description</span></span>                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0589c-114">hashes</span><span class="sxs-lookup"><span data-stu-id="0589c-114">hashes</span></span>   | [<span data-ttu-id="0589c-115">Hashes</span><span class="sxs-lookup"><span data-stu-id="0589c-115">Hashes</span></span>](hashes.md) | <span data-ttu-id="0589c-p102">Hash do conteúdo binário do arquivo, se houver. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0589c-p102">Hashes of the file's binary content, if available. Read-only.</span></span>                                                                                    |
| <span data-ttu-id="0589c-118">mimeType</span><span class="sxs-lookup"><span data-stu-id="0589c-118">mimeType</span></span> | <span data-ttu-id="0589c-119">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0589c-119">string</span></span>                  | <span data-ttu-id="0589c-p103">O tipo MIME para o arquivo. Determinado pela lógica no servidor e pode não ser o valor fornecido quando o arquivo foi carregado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0589c-p103">The MIME type for the file. This is determined by logic on the server and might not be the value provided when the file was uploaded. Read-only.</span></span> |

## <a name="remarks"></a><span data-ttu-id="0589c-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="0589c-123">Remarks</span></span> 

<span data-ttu-id="0589c-124">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="0589c-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File"
} -->

