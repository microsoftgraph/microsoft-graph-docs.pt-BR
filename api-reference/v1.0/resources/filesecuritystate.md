---
title: tipo de recurso fileSecuritystate
description: Contém informações sobre o arquivo (não processo) relacionado ao alerta.
localization_priority: Normal
ms.openlocfilehash: 14ffa41b395bde04972f0af0436297aa4d038524
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564789"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="33d12-103">tipo de recurso fileSecuritystate</span><span class="sxs-lookup"><span data-stu-id="33d12-103">fileSecurityState resource type</span></span>

<span data-ttu-id="33d12-104">Contém informações sobre o arquivo (não processo) relacionado ao alerta.</span><span class="sxs-lookup"><span data-stu-id="33d12-104">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="33d12-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="33d12-105">Properties</span></span>

| <span data-ttu-id="33d12-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33d12-106">Property</span></span>   | <span data-ttu-id="33d12-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="33d12-107">Type</span></span>|<span data-ttu-id="33d12-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="33d12-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33d12-109">fileHash</span><span class="sxs-lookup"><span data-stu-id="33d12-109">fileHash</span></span>|[<span data-ttu-id="33d12-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="33d12-110">fileHash</span></span>](filehash.md)|<span data-ttu-id="33d12-111">Tipo complexo contendo hashes de arquivo (criptográfico e diferencia local).</span><span class="sxs-lookup"><span data-stu-id="33d12-111">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="33d12-112">name</span><span class="sxs-lookup"><span data-stu-id="33d12-112">name</span></span>|<span data-ttu-id="33d12-113">String</span><span class="sxs-lookup"><span data-stu-id="33d12-113">String</span></span>|<span data-ttu-id="33d12-114">Nome do arquivo (sem o caminho).</span><span class="sxs-lookup"><span data-stu-id="33d12-114">File name (without path).</span></span>|
|<span data-ttu-id="33d12-115">caminho</span><span class="sxs-lookup"><span data-stu-id="33d12-115">path</span></span>|<span data-ttu-id="33d12-116">String</span><span class="sxs-lookup"><span data-stu-id="33d12-116">String</span></span>|<span data-ttu-id="33d12-117">Caminho completo do arquivo/ImageFile.</span><span class="sxs-lookup"><span data-stu-id="33d12-117">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="33d12-118">riskScore</span><span class="sxs-lookup"><span data-stu-id="33d12-118">riskScore</span></span>|<span data-ttu-id="33d12-119">String</span><span class="sxs-lookup"><span data-stu-id="33d12-119">String</span></span>|<span data-ttu-id="33d12-120">Geração de um provedor/Pontuação de risco calculado do arquivo de alerta.</span><span class="sxs-lookup"><span data-stu-id="33d12-120">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="33d12-121">O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="33d12-121">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="33d12-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="33d12-122">JSON representation</span></span>

<span data-ttu-id="33d12-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="33d12-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileSecurityState"
}-->

```json
{
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "name": "String",
  "path": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
