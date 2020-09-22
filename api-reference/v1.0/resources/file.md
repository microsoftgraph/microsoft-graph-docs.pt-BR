---
author: JeremyKelley
ms.date: 09/10/2017
title: Thype de recurso de arquivo
localization_priority: Normal
description: O recurso File agrupa itens de dados relacionados a arquivos em uma única estrutura.
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 0b8fc90a54dcb4a052994b4848aeb297b914d9ec
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018407"
---
# <a name="file-resource-type"></a><span data-ttu-id="99599-103">Tipo de recurso File</span><span class="sxs-lookup"><span data-stu-id="99599-103">File resource type</span></span>

<span data-ttu-id="99599-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99599-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="99599-105">O recurso **File** agrupa itens de dados relacionados a arquivos em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="99599-105">The **File** resource groups file-related data items into a single structure.</span></span>

<span data-ttu-id="99599-106">Se um [**DriveItem**](driveitem.md) tiver uma faceta **File** não nula, o item representa um arquivo.</span><span class="sxs-lookup"><span data-stu-id="99599-106">If a [**DriveItem**](driveitem.md) has a non-null **file** facet, the item represents a file.</span></span>
<span data-ttu-id="99599-107">Além de outras propriedades, os arquivos têm um relacionamento **content**, que contém o fluxo de bytes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="99599-107">In addition to other properties, files have a **content** relationship which contains the byte stream of the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="99599-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99599-108">JSON representation</span></span>

<span data-ttu-id="99599-109">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="99599-109">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="99599-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99599-110">Properties</span></span>

| <span data-ttu-id="99599-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99599-111">Property</span></span> | <span data-ttu-id="99599-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="99599-112">Type</span></span>                    | <span data-ttu-id="99599-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="99599-113">Description</span></span>                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="99599-114">hashes</span><span class="sxs-lookup"><span data-stu-id="99599-114">hashes</span></span>   | [<span data-ttu-id="99599-115">Hashes</span><span class="sxs-lookup"><span data-stu-id="99599-115">Hashes</span></span>](hashes.md) | <span data-ttu-id="99599-p102">Hash do conteúdo binário do arquivo, se houver. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="99599-p102">Hashes of the file's binary content, if available. Read-only.</span></span>                                                                                    |
| <span data-ttu-id="99599-118">mimeType</span><span class="sxs-lookup"><span data-stu-id="99599-118">mimeType</span></span> | <span data-ttu-id="99599-119">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99599-119">string</span></span>                  | <span data-ttu-id="99599-p103">O tipo MIME para o arquivo. Determinado pela lógica no servidor e pode não ser o valor fornecido quando o arquivo foi carregado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="99599-p103">The MIME type for the file. This is determined by logic on the server and might not be the value provided when the file was uploaded. Read-only.</span></span> |

## <a name="remarks"></a><span data-ttu-id="99599-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="99599-123">Remarks</span></span> 

<span data-ttu-id="99599-124">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="99599-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File"
} -->

