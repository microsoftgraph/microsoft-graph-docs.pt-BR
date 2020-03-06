---
title: tipo de recurso filesecuritystate
description: Contém informações sobre o arquivo (não processo) relacionado ao alerta.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fc9d05e875104469a25ee742635ea8e86682d9e9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531424"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="ef761-103">tipo de recurso filesecuritystate</span><span class="sxs-lookup"><span data-stu-id="ef761-103">fileSecurityState resource type</span></span>

<span data-ttu-id="ef761-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef761-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ef761-105">Contém informações sobre o arquivo (não processo) relacionado ao alerta.</span><span class="sxs-lookup"><span data-stu-id="ef761-105">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="ef761-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ef761-106">Properties</span></span>

| <span data-ttu-id="ef761-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef761-107">Property</span></span>   | <span data-ttu-id="ef761-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef761-108">Type</span></span>|<span data-ttu-id="ef761-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef761-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef761-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="ef761-110">fileHash</span></span>|[<span data-ttu-id="ef761-111">fileHash</span><span class="sxs-lookup"><span data-stu-id="ef761-111">fileHash</span></span>](filehash.md)|<span data-ttu-id="ef761-112">Tipo complexo contendo hashes de arquivo (criptográfico e diferencia local).</span><span class="sxs-lookup"><span data-stu-id="ef761-112">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="ef761-113">nome</span><span class="sxs-lookup"><span data-stu-id="ef761-113">name</span></span>|<span data-ttu-id="ef761-114">String</span><span class="sxs-lookup"><span data-stu-id="ef761-114">String</span></span>|<span data-ttu-id="ef761-115">Nome do arquivo (sem o caminho).</span><span class="sxs-lookup"><span data-stu-id="ef761-115">File name (without path).</span></span>|
|<span data-ttu-id="ef761-116">caminho</span><span class="sxs-lookup"><span data-stu-id="ef761-116">path</span></span>|<span data-ttu-id="ef761-117">String</span><span class="sxs-lookup"><span data-stu-id="ef761-117">String</span></span>|<span data-ttu-id="ef761-118">Caminho completo do arquivo/ImageFile.</span><span class="sxs-lookup"><span data-stu-id="ef761-118">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="ef761-119">riskScore</span><span class="sxs-lookup"><span data-stu-id="ef761-119">riskScore</span></span>|<span data-ttu-id="ef761-120">String</span><span class="sxs-lookup"><span data-stu-id="ef761-120">String</span></span>|<span data-ttu-id="ef761-121">Geração de um provedor/Pontuação de risco calculado do arquivo de alerta.</span><span class="sxs-lookup"><span data-stu-id="ef761-121">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="ef761-122">O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="ef761-122">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ef761-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ef761-123">JSON representation</span></span>

<span data-ttu-id="ef761-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ef761-124">The following is a JSON representation of the resource.</span></span>

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
