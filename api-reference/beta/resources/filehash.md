---
title: tipo de recurso fileHash
description: Contém informações com monitoração de hash de arquivo (criptografia e confidencialidade de local).
localization_priority: Normal
ms.openlocfilehash: f5d865a7ded230ca611b8628c3648ec1e331c67d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547603"
---
# <a name="filehash-resource-type"></a><span data-ttu-id="04f10-103">tipo de recurso fileHash</span><span class="sxs-lookup"><span data-stu-id="04f10-103">fileHash resource type</span></span>

<span data-ttu-id="04f10-104">Contém informações com monitoração de hash de arquivo (criptografia e confidencialidade de local).</span><span class="sxs-lookup"><span data-stu-id="04f10-104">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="04f10-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04f10-105">Properties</span></span>

| <span data-ttu-id="04f10-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04f10-106">Property</span></span>     | <span data-ttu-id="04f10-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="04f10-107">Type</span></span>        | <span data-ttu-id="04f10-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="04f10-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="04f10-109">hashtype</span><span class="sxs-lookup"><span data-stu-id="04f10-109">hashType</span></span>|<span data-ttu-id="04f10-110">[](filehashtypeenumtype.md) Enumeração filehashtype</span><span class="sxs-lookup"><span data-stu-id="04f10-110">[fileHashType](filehashtypeenumtype.md) enum</span></span>|<span data-ttu-id="04f10-111">Tipo de hash de arquivo.</span><span class="sxs-lookup"><span data-stu-id="04f10-111">File hash type.</span></span> <span data-ttu-id="04f10-112">Os valores possíveis são: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span><span class="sxs-lookup"><span data-stu-id="04f10-112">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="04f10-113">hashValue</span><span class="sxs-lookup"><span data-stu-id="04f10-113">hashValue</span></span>|<span data-ttu-id="04f10-114">String</span><span class="sxs-lookup"><span data-stu-id="04f10-114">String</span></span>|<span data-ttu-id="04f10-115">Valor do hash do arquivo.</span><span class="sxs-lookup"><span data-stu-id="04f10-115">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="04f10-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04f10-116">JSON representation</span></span>

<span data-ttu-id="04f10-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04f10-117">The following is a JSON representation of the resource.</span></span>

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
