---
title: tipo de recurso filesecuritystate
description: Contém informações sobre o arquivo (não processo) relacionado ao alerta.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6e6f30625412022006d88179e3192b1463c797c0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032491"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="84234-103">tipo de recurso filesecuritystate</span><span class="sxs-lookup"><span data-stu-id="84234-103">fileSecurityState resource type</span></span>

<span data-ttu-id="84234-104">Contém informações sobre o arquivo (não processo) relacionado ao alerta.</span><span class="sxs-lookup"><span data-stu-id="84234-104">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="84234-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="84234-105">Properties</span></span>

| <span data-ttu-id="84234-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84234-106">Property</span></span>   | <span data-ttu-id="84234-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="84234-107">Type</span></span>|<span data-ttu-id="84234-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="84234-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84234-109">fileHash</span><span class="sxs-lookup"><span data-stu-id="84234-109">fileHash</span></span>|[<span data-ttu-id="84234-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="84234-110">fileHash</span></span>](filehash.md)|<span data-ttu-id="84234-111">Tipo complexo contendo hashes de arquivo (criptográfico e diferencia local).</span><span class="sxs-lookup"><span data-stu-id="84234-111">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="84234-112">name</span><span class="sxs-lookup"><span data-stu-id="84234-112">name</span></span>|<span data-ttu-id="84234-113">String</span><span class="sxs-lookup"><span data-stu-id="84234-113">String</span></span>|<span data-ttu-id="84234-114">Nome do arquivo (sem o caminho).</span><span class="sxs-lookup"><span data-stu-id="84234-114">File name (without path).</span></span>|
|<span data-ttu-id="84234-115">caminho</span><span class="sxs-lookup"><span data-stu-id="84234-115">path</span></span>|<span data-ttu-id="84234-116">String</span><span class="sxs-lookup"><span data-stu-id="84234-116">String</span></span>|<span data-ttu-id="84234-117">Caminho completo do arquivo/ImageFile.</span><span class="sxs-lookup"><span data-stu-id="84234-117">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="84234-118">riskScore</span><span class="sxs-lookup"><span data-stu-id="84234-118">riskScore</span></span>|<span data-ttu-id="84234-119">String</span><span class="sxs-lookup"><span data-stu-id="84234-119">String</span></span>|<span data-ttu-id="84234-120">Geração de um provedor/Pontuação de risco calculado do arquivo de alerta.</span><span class="sxs-lookup"><span data-stu-id="84234-120">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="84234-121">O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="84234-121">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="84234-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="84234-122">JSON representation</span></span>

<span data-ttu-id="84234-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="84234-123">The following is a JSON representation of the resource.</span></span>

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
