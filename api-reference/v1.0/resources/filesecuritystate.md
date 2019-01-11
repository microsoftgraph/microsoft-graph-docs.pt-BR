---
title: tipo de recurso de fileSecurityState
description: Contém informações sobre o arquivo (não process) relacionada ao alerta.
localization_priority: Normal
ms.openlocfilehash: 14ffa41b395bde04972f0af0436297aa4d038524
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894093"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="df993-103">tipo de recurso de fileSecurityState</span><span class="sxs-lookup"><span data-stu-id="df993-103">fileSecurityState resource type</span></span>

<span data-ttu-id="df993-104">Contém informações sobre o arquivo (não process) relacionada ao alerta.</span><span class="sxs-lookup"><span data-stu-id="df993-104">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="df993-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df993-105">Properties</span></span>

| <span data-ttu-id="df993-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df993-106">Property</span></span>   | <span data-ttu-id="df993-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="df993-107">Type</span></span>|<span data-ttu-id="df993-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="df993-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df993-109">fileHash</span><span class="sxs-lookup"><span data-stu-id="df993-109">fileHash</span></span>|[<span data-ttu-id="df993-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="df993-110">fileHash</span></span>](filehash.md)|<span data-ttu-id="df993-111">Tipo complexo contendo hashes de arquivo (criptográficos e confidenciais local).</span><span class="sxs-lookup"><span data-stu-id="df993-111">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="df993-112">name</span><span class="sxs-lookup"><span data-stu-id="df993-112">name</span></span>|<span data-ttu-id="df993-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df993-113">String</span></span>|<span data-ttu-id="df993-114">Nome de arquivo (sem o caminho).</span><span class="sxs-lookup"><span data-stu-id="df993-114">File name (without path).</span></span>|
|<span data-ttu-id="df993-115">caminho</span><span class="sxs-lookup"><span data-stu-id="df993-115">path</span></span>|<span data-ttu-id="df993-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df993-116">String</span></span>|<span data-ttu-id="df993-117">Caminho do arquivo completo do arquivo/imageFile.</span><span class="sxs-lookup"><span data-stu-id="df993-117">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="df993-118">riskScore</span><span class="sxs-lookup"><span data-stu-id="df993-118">riskScore</span></span>|<span data-ttu-id="df993-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df993-119">String</span></span>|<span data-ttu-id="df993-120">Provedor gerado/calculado o risco de pontuação do arquivo de alerta.</span><span class="sxs-lookup"><span data-stu-id="df993-120">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="df993-121">Valor recomendado o intervalo de 0-1, que é igual a um percentual.</span><span class="sxs-lookup"><span data-stu-id="df993-121">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="df993-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df993-122">JSON representation</span></span>

<span data-ttu-id="df993-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="df993-123">The following is a JSON representation of the resource.</span></span>

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
