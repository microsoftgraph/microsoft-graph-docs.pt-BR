---
title: Tipo de recurso educationFileResource
description: Uma subclasse de educationResource que representa um objeto de arquivo associado à atribuição ou envio.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 814ea6119210184356c561ac4f6a3dee5d3eac10
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912107"
---
# <a name="educationfileresource-resource-type"></a><span data-ttu-id="2d537-103">Tipo de recurso educationFileResource</span><span class="sxs-lookup"><span data-stu-id="2d537-103">educationFileResource resource type</span></span>

<span data-ttu-id="2d537-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d537-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2d537-105">Uma subclasse [de educationResource](educationresource.md) que representa um objeto de arquivo associado à atribuição ou envio.</span><span class="sxs-lookup"><span data-stu-id="2d537-105">A subclass of [educationResource](educationresource.md) that represents a file object that is associated with the assignment or submission.</span></span>

<span data-ttu-id="2d537-106">Nesse caso, o arquivo não é um dos arquivos especiais (Word, Excel e assim por diante), mas é um arquivo que não tem tratamento especial dentro do sistema.</span><span class="sxs-lookup"><span data-stu-id="2d537-106">In this case, the file isn't one of the special files (Word, Excel, and so on) but is a file that does not have special handling within the system.</span></span> <span data-ttu-id="2d537-107">O recurso de arquivo deve ser armazenado no **resourceFolder** que está associado à atribuição ou ao envio ao que esse recurso está anexado.</span><span class="sxs-lookup"><span data-stu-id="2d537-107">The file resource must be stored in the **resourceFolder** that is associated with the assignment or submission this resource is attached to.</span></span>

## <a name="properties"></a><span data-ttu-id="2d537-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2d537-108">Properties</span></span>
| <span data-ttu-id="2d537-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d537-109">Property</span></span>     | <span data-ttu-id="2d537-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d537-110">Type</span></span>   |<span data-ttu-id="2d537-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d537-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d537-112">fileUrl</span><span class="sxs-lookup"><span data-stu-id="2d537-112">fileUrl</span></span>|<span data-ttu-id="2d537-113">String</span><span class="sxs-lookup"><span data-stu-id="2d537-113">String</span></span>|<span data-ttu-id="2d537-114">Local no disco do recurso de arquivo.</span><span class="sxs-lookup"><span data-stu-id="2d537-114">Location on disk of the file resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2d537-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2d537-115">JSON representation</span></span>

<span data-ttu-id="2d537-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2d537-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->


