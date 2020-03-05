---
title: tipo de recurso FileHash
description: Contém informações com monitoração de hash de arquivo (criptografia e confidencialidade de local).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: a163a89e1e7ca7cb2a6bdf4c65945a601323d8fd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498235"
---
# <a name="filehash-resource-type"></a><span data-ttu-id="ac5ab-103">tipo de recurso FileHash</span><span class="sxs-lookup"><span data-stu-id="ac5ab-103">fileHash resource type</span></span>

<span data-ttu-id="ac5ab-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ac5ab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ac5ab-105">Contém informações com monitoração de hash de arquivo (criptografia e confidencialidade de local).</span><span class="sxs-lookup"><span data-stu-id="ac5ab-105">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="ac5ab-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac5ab-106">Properties</span></span>

| <span data-ttu-id="ac5ab-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac5ab-107">Property</span></span>     | <span data-ttu-id="ac5ab-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac5ab-108">Type</span></span>        | <span data-ttu-id="ac5ab-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac5ab-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ac5ab-110">hashtype</span><span class="sxs-lookup"><span data-stu-id="ac5ab-110">hashType</span></span>|<span data-ttu-id="ac5ab-111">Enumeração [Filehashtype](filehashtypeenumtype.md)</span><span class="sxs-lookup"><span data-stu-id="ac5ab-111">[fileHashType](filehashtypeenumtype.md) enum</span></span>|<span data-ttu-id="ac5ab-112">Tipo de hash de arquivo.</span><span class="sxs-lookup"><span data-stu-id="ac5ab-112">File hash type.</span></span> <span data-ttu-id="ac5ab-113">Os valores possíveis são: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span><span class="sxs-lookup"><span data-stu-id="ac5ab-113">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="ac5ab-114">hashValue</span><span class="sxs-lookup"><span data-stu-id="ac5ab-114">hashValue</span></span>|<span data-ttu-id="ac5ab-115">String</span><span class="sxs-lookup"><span data-stu-id="ac5ab-115">String</span></span>|<span data-ttu-id="ac5ab-116">Valor do hash do arquivo.</span><span class="sxs-lookup"><span data-stu-id="ac5ab-116">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ac5ab-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac5ab-117">JSON representation</span></span>

<span data-ttu-id="ac5ab-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ac5ab-118">The following is a JSON representation of the resource.</span></span>

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
