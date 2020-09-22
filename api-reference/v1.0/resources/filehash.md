---
title: tipo de recurso FileHash
description: Contém informações com monitoração de hash de arquivo (criptografia e confidencialidade de local).
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 412308fc20c3baee63640451bb1a2c8059e71be0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018372"
---
# <a name="filehash-resource-type"></a><span data-ttu-id="91ab6-103">tipo de recurso FileHash</span><span class="sxs-lookup"><span data-stu-id="91ab6-103">fileHash resource type</span></span>

<span data-ttu-id="91ab6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91ab6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="91ab6-105">Contém informações com monitoração de hash de arquivo (criptografia e confidencialidade de local).</span><span class="sxs-lookup"><span data-stu-id="91ab6-105">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="91ab6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="91ab6-106">Properties</span></span>

| <span data-ttu-id="91ab6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91ab6-107">Property</span></span>     | <span data-ttu-id="91ab6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="91ab6-108">Type</span></span>        | <span data-ttu-id="91ab6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="91ab6-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="91ab6-110">hashtype</span><span class="sxs-lookup"><span data-stu-id="91ab6-110">hashType</span></span>|<span data-ttu-id="91ab6-111">fileHashType</span><span class="sxs-lookup"><span data-stu-id="91ab6-111">fileHashType</span></span>|<span data-ttu-id="91ab6-112">Tipo de hash de arquivo.</span><span class="sxs-lookup"><span data-stu-id="91ab6-112">File hash type.</span></span> <span data-ttu-id="91ab6-113">Os valores possíveis são: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span><span class="sxs-lookup"><span data-stu-id="91ab6-113">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="91ab6-114">hashValue</span><span class="sxs-lookup"><span data-stu-id="91ab6-114">hashValue</span></span>|<span data-ttu-id="91ab6-115">String</span><span class="sxs-lookup"><span data-stu-id="91ab6-115">String</span></span>|<span data-ttu-id="91ab6-116">Valor do hash do arquivo.</span><span class="sxs-lookup"><span data-stu-id="91ab6-116">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="91ab6-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="91ab6-117">JSON representation</span></span>

<span data-ttu-id="91ab6-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="91ab6-118">The following is a JSON representation of the resource.</span></span>

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

