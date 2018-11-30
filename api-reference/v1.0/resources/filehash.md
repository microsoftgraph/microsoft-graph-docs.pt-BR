---
title: tipo de recurso de fileHash
description: Contém informações com informações de estado sobre hashes de arquivo (criptográficos e confidenciais local).
ms.openlocfilehash: f7e1f5ceba700a30f1e68e0670ebcec40c3d6fd5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004606"
---
# <a name="filehash-resource-type"></a><span data-ttu-id="6fdae-103">tipo de recurso de fileHash</span><span class="sxs-lookup"><span data-stu-id="6fdae-103">fileHash resource type</span></span>

<span data-ttu-id="6fdae-104">Contém informações com informações de estado sobre hashes de arquivo (criptográficos e confidenciais local).</span><span class="sxs-lookup"><span data-stu-id="6fdae-104">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="6fdae-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6fdae-105">Properties</span></span>

| <span data-ttu-id="6fdae-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6fdae-106">Property</span></span>     | <span data-ttu-id="6fdae-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fdae-107">Type</span></span>        | <span data-ttu-id="6fdae-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fdae-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6fdae-109">hashType</span><span class="sxs-lookup"><span data-stu-id="6fdae-109">hashType</span></span>|<span data-ttu-id="6fdae-110">fileHashType</span><span class="sxs-lookup"><span data-stu-id="6fdae-110">fileHashType</span></span>|<span data-ttu-id="6fdae-111">Tipo de hash do arquivo.</span><span class="sxs-lookup"><span data-stu-id="6fdae-111">File hash type.</span></span> <span data-ttu-id="6fdae-112">Os valores possíveis são: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span><span class="sxs-lookup"><span data-stu-id="6fdae-112">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="6fdae-113">hashValue</span><span class="sxs-lookup"><span data-stu-id="6fdae-113">hashValue</span></span>|<span data-ttu-id="6fdae-114">String</span><span class="sxs-lookup"><span data-stu-id="6fdae-114">String</span></span>|<span data-ttu-id="6fdae-115">Valor de hash do arquivo.</span><span class="sxs-lookup"><span data-stu-id="6fdae-115">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6fdae-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6fdae-116">JSON representation</span></span>

<span data-ttu-id="6fdae-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6fdae-117">The following is a JSON representation of the resource.</span></span>

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