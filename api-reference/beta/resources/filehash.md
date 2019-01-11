---
title: tipo de recurso de fileHash
description: Contém informações com informações de estado sobre hashes de arquivo (criptográficos e confidenciais local).
localization_priority: Normal
ms.openlocfilehash: f5d865a7ded230ca611b8628c3648ec1e331c67d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815642"
---
# <a name="filehash-resource-type"></a><span data-ttu-id="d7838-103">tipo de recurso de fileHash</span><span class="sxs-lookup"><span data-stu-id="d7838-103">fileHash resource type</span></span>

<span data-ttu-id="d7838-104">Contém informações com informações de estado sobre hashes de arquivo (criptográficos e confidenciais local).</span><span class="sxs-lookup"><span data-stu-id="d7838-104">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="d7838-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d7838-105">Properties</span></span>

| <span data-ttu-id="d7838-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7838-106">Property</span></span>     | <span data-ttu-id="d7838-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7838-107">Type</span></span>        | <span data-ttu-id="d7838-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7838-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d7838-109">hashType</span><span class="sxs-lookup"><span data-stu-id="d7838-109">hashType</span></span>|<span data-ttu-id="d7838-110">enumeração [fileHashType](filehashtypeenumtype.md)</span><span class="sxs-lookup"><span data-stu-id="d7838-110">[fileHashType](filehashtypeenumtype.md) enum</span></span>|<span data-ttu-id="d7838-111">Tipo de hash do arquivo.</span><span class="sxs-lookup"><span data-stu-id="d7838-111">File hash type.</span></span> <span data-ttu-id="d7838-112">Os valores possíveis são: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span><span class="sxs-lookup"><span data-stu-id="d7838-112">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="d7838-113">hashValue</span><span class="sxs-lookup"><span data-stu-id="d7838-113">hashValue</span></span>|<span data-ttu-id="d7838-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7838-114">String</span></span>|<span data-ttu-id="d7838-115">Valor de hash do arquivo.</span><span class="sxs-lookup"><span data-stu-id="d7838-115">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d7838-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d7838-116">JSON representation</span></span>

<span data-ttu-id="d7838-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d7838-117">The following is a JSON representation of the resource.</span></span>

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
