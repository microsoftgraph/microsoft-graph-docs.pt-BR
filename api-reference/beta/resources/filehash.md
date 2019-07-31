---
title: tipo de recurso FileHash
description: Contém informações com monitoração de hash de arquivo (criptografia e confidencialidade de local).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 532389671cacb907c7e85862a621b936ec1691a0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973531"
---
# <a name="filehash-resource-type"></a><span data-ttu-id="9c9d2-103">tipo de recurso FileHash</span><span class="sxs-lookup"><span data-stu-id="9c9d2-103">fileHash resource type</span></span>

<span data-ttu-id="9c9d2-104">Contém informações com monitoração de hash de arquivo (criptografia e confidencialidade de local).</span><span class="sxs-lookup"><span data-stu-id="9c9d2-104">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="9c9d2-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c9d2-105">Properties</span></span>

| <span data-ttu-id="9c9d2-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c9d2-106">Property</span></span>     | <span data-ttu-id="9c9d2-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c9d2-107">Type</span></span>        | <span data-ttu-id="9c9d2-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c9d2-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9c9d2-109">hashtype</span><span class="sxs-lookup"><span data-stu-id="9c9d2-109">hashType</span></span>|<span data-ttu-id="9c9d2-110">[](filehashtypeenumtype.md) Enumeração filehashtype</span><span class="sxs-lookup"><span data-stu-id="9c9d2-110">[fileHashType](filehashtypeenumtype.md) enum</span></span>|<span data-ttu-id="9c9d2-111">Tipo de hash de arquivo.</span><span class="sxs-lookup"><span data-stu-id="9c9d2-111">File hash type.</span></span> <span data-ttu-id="9c9d2-112">Os valores possíveis são: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span><span class="sxs-lookup"><span data-stu-id="9c9d2-112">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="9c9d2-113">hashValue</span><span class="sxs-lookup"><span data-stu-id="9c9d2-113">hashValue</span></span>|<span data-ttu-id="9c9d2-114">String</span><span class="sxs-lookup"><span data-stu-id="9c9d2-114">String</span></span>|<span data-ttu-id="9c9d2-115">Valor do hash do arquivo.</span><span class="sxs-lookup"><span data-stu-id="9c9d2-115">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9c9d2-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c9d2-116">JSON representation</span></span>

<span data-ttu-id="9c9d2-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c9d2-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileHash"
}-->

```json
{
  "hashType": "@odata.type: microsoft.graph.fileHashType",
  "hashValue": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileHash resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
