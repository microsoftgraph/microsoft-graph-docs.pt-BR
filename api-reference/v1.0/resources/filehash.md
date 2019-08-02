---
title: tipo de recurso FileHash
description: Contém informações com monitoração de hash de arquivo (criptografia e confidencialidade de local).
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: aabe56237ea44285c93f802268bd68688f16aa05
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030377"
---
# <a name="filehash-resource-type"></a><span data-ttu-id="e5614-103">tipo de recurso FileHash</span><span class="sxs-lookup"><span data-stu-id="e5614-103">fileHash resource type</span></span>

<span data-ttu-id="e5614-104">Contém informações com monitoração de hash de arquivo (criptografia e confidencialidade de local).</span><span class="sxs-lookup"><span data-stu-id="e5614-104">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="e5614-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5614-105">Properties</span></span>

| <span data-ttu-id="e5614-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5614-106">Property</span></span>     | <span data-ttu-id="e5614-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5614-107">Type</span></span>        | <span data-ttu-id="e5614-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5614-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e5614-109">hashtype</span><span class="sxs-lookup"><span data-stu-id="e5614-109">hashType</span></span>|<span data-ttu-id="e5614-110">fileHashType</span><span class="sxs-lookup"><span data-stu-id="e5614-110">fileHashType</span></span>|<span data-ttu-id="e5614-111">Tipo de hash de arquivo.</span><span class="sxs-lookup"><span data-stu-id="e5614-111">File hash type.</span></span> <span data-ttu-id="e5614-112">Os valores possíveis são: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span><span class="sxs-lookup"><span data-stu-id="e5614-112">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="e5614-113">hashValue</span><span class="sxs-lookup"><span data-stu-id="e5614-113">hashValue</span></span>|<span data-ttu-id="e5614-114">String</span><span class="sxs-lookup"><span data-stu-id="e5614-114">String</span></span>|<span data-ttu-id="e5614-115">Valor do hash do arquivo.</span><span class="sxs-lookup"><span data-stu-id="e5614-115">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e5614-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5614-116">JSON representation</span></span>

<span data-ttu-id="e5614-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e5614-117">The following is a JSON representation of the resource.</span></span>

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
