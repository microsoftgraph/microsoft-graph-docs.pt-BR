---
title: tipo de recurso de fileSecurityState
description: Contém informações sobre o arquivo (não process) relacionada ao alerta.
ms.openlocfilehash: d1358d7fe0d5565845201781e32b3da14a89f412
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007213"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="8f1cb-103">tipo de recurso de fileSecurityState</span><span class="sxs-lookup"><span data-stu-id="8f1cb-103">fileSecurityState resource type</span></span>

<span data-ttu-id="8f1cb-104">Contém informações sobre o arquivo (não process) relacionada ao alerta.</span><span class="sxs-lookup"><span data-stu-id="8f1cb-104">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="8f1cb-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8f1cb-105">Properties</span></span>

| <span data-ttu-id="8f1cb-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8f1cb-106">Property</span></span>   | <span data-ttu-id="8f1cb-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f1cb-107">Type</span></span>|<span data-ttu-id="8f1cb-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f1cb-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f1cb-109">fileHash</span><span class="sxs-lookup"><span data-stu-id="8f1cb-109">fileHash</span></span>|[<span data-ttu-id="8f1cb-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="8f1cb-110">fileHash</span></span>](filehash.md)|<span data-ttu-id="8f1cb-111">Tipo complexo contendo hashes de arquivo (criptográficos e confidenciais local).</span><span class="sxs-lookup"><span data-stu-id="8f1cb-111">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="8f1cb-112">name</span><span class="sxs-lookup"><span data-stu-id="8f1cb-112">name</span></span>|<span data-ttu-id="8f1cb-113">String</span><span class="sxs-lookup"><span data-stu-id="8f1cb-113">String</span></span>|<span data-ttu-id="8f1cb-114">Nome de arquivo (sem o caminho).</span><span class="sxs-lookup"><span data-stu-id="8f1cb-114">File name (without path).</span></span>|
|<span data-ttu-id="8f1cb-115">caminho</span><span class="sxs-lookup"><span data-stu-id="8f1cb-115">path</span></span>|<span data-ttu-id="8f1cb-116">String</span><span class="sxs-lookup"><span data-stu-id="8f1cb-116">String</span></span>|<span data-ttu-id="8f1cb-117">Caminho do arquivo completo do arquivo/imageFile.</span><span class="sxs-lookup"><span data-stu-id="8f1cb-117">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="8f1cb-118">riskScore</span><span class="sxs-lookup"><span data-stu-id="8f1cb-118">riskScore</span></span>|<span data-ttu-id="8f1cb-119">String</span><span class="sxs-lookup"><span data-stu-id="8f1cb-119">String</span></span>|<span data-ttu-id="8f1cb-120">Provedor gerado/calculado o risco de pontuação do arquivo de alerta.</span><span class="sxs-lookup"><span data-stu-id="8f1cb-120">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="8f1cb-121">Valor recomendado o intervalo de 0-1, que é igual a um percentual.</span><span class="sxs-lookup"><span data-stu-id="8f1cb-121">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8f1cb-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8f1cb-122">JSON representation</span></span>

<span data-ttu-id="8f1cb-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8f1cb-123">The following is a JSON representation of the resource.</span></span>

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