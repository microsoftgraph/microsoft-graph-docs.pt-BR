---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Arquivo
localization_priority: Normal
ms.openlocfilehash: 7478ba064b5193ce7ddcd8685fc571a72d4b0057
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564782"
---
# <a name="file-resource-type"></a><span data-ttu-id="fa844-102">Tipo de recurso File</span><span class="sxs-lookup"><span data-stu-id="fa844-102">File resource type</span></span>

<span data-ttu-id="fa844-103">O recurso **File** agrupa itens de dados relacionados a arquivos em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="fa844-103">The **File** resource groups file-related data items into a single structure.</span></span>

<span data-ttu-id="fa844-p101">Se um [**DriveItem**](driveitem.md) tiver uma faceta **file** não nula, o item representa um arquivo. Além de outras propriedades, os arquivos têm um relacionamento **content**, que contém o fluxo de bytes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="fa844-p101">If a [**DriveItem**](driveitem.md) has a non-null **file** facet, the item represents an file. In addition to other properties, files have a **content** relationship which contains the byte stream of the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa844-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fa844-106">JSON representation</span></span>

<span data-ttu-id="fa844-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fa844-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="fa844-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fa844-108">Properties</span></span>

| <span data-ttu-id="fa844-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa844-109">Property</span></span> | <span data-ttu-id="fa844-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa844-110">Type</span></span>                    | <span data-ttu-id="fa844-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa844-111">Description</span></span>                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="fa844-112">hashes</span><span class="sxs-lookup"><span data-stu-id="fa844-112">hashes</span></span>   | [<span data-ttu-id="fa844-113">Hashes</span><span class="sxs-lookup"><span data-stu-id="fa844-113">Hashes</span></span>](hashes.md) | <span data-ttu-id="fa844-p102">Hash do conteúdo binário do arquivo, se houver. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fa844-p102">Hashes of the file's binary content, if available. Read-only.</span></span>                                                                                    |
| <span data-ttu-id="fa844-116">mimeType</span><span class="sxs-lookup"><span data-stu-id="fa844-116">mimeType</span></span> | <span data-ttu-id="fa844-117">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fa844-117">string</span></span>                  | <span data-ttu-id="fa844-p103">O tipo MIME para o arquivo. Determinado pela lógica no servidor e pode não ser o valor fornecido quando o arquivo foi carregado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fa844-p103">The MIME type for the file. This is determined by logic on the server and might not be the value provided when the file was uploaded. Read-only.</span></span> |

## <a name="remarks"></a><span data-ttu-id="fa844-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="fa844-121">Remarks</span></span> 

<span data-ttu-id="fa844-122">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="fa844-122">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File"
} -->
