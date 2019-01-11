---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: File
localization_priority: Normal
ms.openlocfilehash: bd2b0fba75ef54586dcfe8b69043669b0681f6b2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816321"
---
# <a name="file-resource-type"></a><span data-ttu-id="0ff3e-102">Tipo de recurso File</span><span class="sxs-lookup"><span data-stu-id="0ff3e-102">File resource type</span></span>

> <span data-ttu-id="0ff3e-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0ff3e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ff3e-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0ff3e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0ff3e-105">O recurso **File** agrupa itens de dados relacionados a arquivos em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="0ff3e-105">The **File** resource groups file-related data items into a single structure.</span></span>

<span data-ttu-id="0ff3e-p102">Se um [**DriveItem**](driveitem.md) tiver uma faceta **file** não nula, o item representa um arquivo. Além de outras propriedades, os arquivos têm um relacionamento **content**, que contém o fluxo de bytes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="0ff3e-p102">If a [**DriveItem**](driveitem.md) has a non-null **file** facet, the item represents an file. In addition to other properties, files have a **content** relationship which contains the byte stream of the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ff3e-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ff3e-108">JSON representation</span></span>

<span data-ttu-id="0ff3e-109">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ff3e-109">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="0ff3e-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ff3e-110">Properties</span></span>

| <span data-ttu-id="0ff3e-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ff3e-111">Property</span></span> | <span data-ttu-id="0ff3e-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ff3e-112">Type</span></span>                    | <span data-ttu-id="0ff3e-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ff3e-113">Description</span></span>                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0ff3e-114">hashes</span><span class="sxs-lookup"><span data-stu-id="0ff3e-114">hashes</span></span>   | [<span data-ttu-id="0ff3e-115">HashesType</span><span class="sxs-lookup"><span data-stu-id="0ff3e-115">HashesType</span></span>](hashes.md) | <span data-ttu-id="0ff3e-p103">Hash do conteúdo binário do arquivo, se houver. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ff3e-p103">Hashes of the file's binary content, if available. Read-only.</span></span>                                                                                    |
| <span data-ttu-id="0ff3e-118">mimeType</span><span class="sxs-lookup"><span data-stu-id="0ff3e-118">mimeType</span></span> | <span data-ttu-id="0ff3e-119">string</span><span class="sxs-lookup"><span data-stu-id="0ff3e-119">string</span></span>                  | <span data-ttu-id="0ff3e-p104">O tipo MIME para o arquivo. Determinado pela lógica no servidor e pode não ser o valor fornecido quando o arquivo foi carregado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ff3e-p104">The MIME type for the file. This is determined by logic on the server and might not be the value provided when the file was uploaded. Read-only.</span></span> |

## <a name="remarks"></a><span data-ttu-id="0ff3e-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="0ff3e-123">Remarks</span></span> 

<span data-ttu-id="0ff3e-124">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="0ff3e-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File"
} -->
