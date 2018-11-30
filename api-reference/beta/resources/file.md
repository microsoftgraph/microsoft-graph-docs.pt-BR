---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: File
ms.openlocfilehash: bd0cd6ea5f5ee2225392aa61c2dda9b30e2ffbca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039194"
---
# <a name="file-resource-type"></a><span data-ttu-id="dbadf-102">Tipo de recurso File</span><span class="sxs-lookup"><span data-stu-id="dbadf-102">File resource type</span></span>

> <span data-ttu-id="dbadf-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dbadf-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbadf-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dbadf-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dbadf-105">O recurso **File** agrupa itens de dados relacionados a arquivos em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="dbadf-105">The **File** resource groups file-related data items into a single structure.</span></span>

<span data-ttu-id="dbadf-p102">Se um [**DriveItem**](driveitem.md) tiver uma faceta **file** não nula, o item representa um arquivo. Além de outras propriedades, os arquivos têm um relacionamento **content**, que contém o fluxo de bytes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="dbadf-p102">If a [**DriveItem**](driveitem.md) has a non-null **file** facet, the item represents an file. In addition to other properties, files have a **content** relationship which contains the byte stream of the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dbadf-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dbadf-108">JSON representation</span></span>

<span data-ttu-id="dbadf-109">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dbadf-109">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="dbadf-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dbadf-110">Properties</span></span>

| <span data-ttu-id="dbadf-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dbadf-111">Property</span></span> | <span data-ttu-id="dbadf-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbadf-112">Type</span></span>                    | <span data-ttu-id="dbadf-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbadf-113">Description</span></span>                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="dbadf-114">hashes</span><span class="sxs-lookup"><span data-stu-id="dbadf-114">hashes</span></span>   | [<span data-ttu-id="dbadf-115">HashesType</span><span class="sxs-lookup"><span data-stu-id="dbadf-115">HashesType</span></span>](hashes.md) | <span data-ttu-id="dbadf-p103">Hash do conteúdo binário do arquivo, se houver. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dbadf-p103">Hashes of the file's binary content, if available. Read-only.</span></span>                                                                                    |
| <span data-ttu-id="dbadf-118">mimeType</span><span class="sxs-lookup"><span data-stu-id="dbadf-118">mimeType</span></span> | <span data-ttu-id="dbadf-119">string</span><span class="sxs-lookup"><span data-stu-id="dbadf-119">string</span></span>                  | <span data-ttu-id="dbadf-p104">O tipo MIME para o arquivo. Determinado pela lógica no servidor e pode não ser o valor fornecido quando o arquivo foi carregado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dbadf-p104">The MIME type for the file. This is determined by logic on the server and might not be the value provided when the file was uploaded. Read-only.</span></span> |

## <a name="remarks"></a><span data-ttu-id="dbadf-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="dbadf-123">Remarks</span></span> 

<span data-ttu-id="dbadf-124">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="dbadf-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File"
} -->
