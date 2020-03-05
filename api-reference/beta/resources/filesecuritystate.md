---
title: tipo de recurso filesecuritystate
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3827562407b0c253c1d5a16ff26071e8500010bd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498165"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="bcaf0-104">tipo de recurso filesecuritystate</span><span class="sxs-lookup"><span data-stu-id="bcaf0-104">fileSecurityState resource type</span></span>

<span data-ttu-id="bcaf0-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bcaf0-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcaf0-106">Contém informações sobre o arquivo (não processo) relacionado ao alerta.</span><span class="sxs-lookup"><span data-stu-id="bcaf0-106">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="bcaf0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bcaf0-107">Properties</span></span>

| <span data-ttu-id="bcaf0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bcaf0-108">Property</span></span>   | <span data-ttu-id="bcaf0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="bcaf0-109">Type</span></span>|<span data-ttu-id="bcaf0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bcaf0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bcaf0-111">fileHash</span><span class="sxs-lookup"><span data-stu-id="bcaf0-111">fileHash</span></span>|[<span data-ttu-id="bcaf0-112">fileHash</span><span class="sxs-lookup"><span data-stu-id="bcaf0-112">fileHash</span></span>](filehash.md)|<span data-ttu-id="bcaf0-113">Tipo complexo contendo hashes de arquivo (criptográfico e diferencia local).</span><span class="sxs-lookup"><span data-stu-id="bcaf0-113">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="bcaf0-114">nome</span><span class="sxs-lookup"><span data-stu-id="bcaf0-114">name</span></span>|<span data-ttu-id="bcaf0-115">String</span><span class="sxs-lookup"><span data-stu-id="bcaf0-115">String</span></span>|<span data-ttu-id="bcaf0-116">Nome do arquivo (sem o caminho).</span><span class="sxs-lookup"><span data-stu-id="bcaf0-116">File name (without path).</span></span>|
|<span data-ttu-id="bcaf0-117">caminho</span><span class="sxs-lookup"><span data-stu-id="bcaf0-117">path</span></span>|<span data-ttu-id="bcaf0-118">String</span><span class="sxs-lookup"><span data-stu-id="bcaf0-118">String</span></span>|<span data-ttu-id="bcaf0-119">Caminho completo do arquivo/ImageFile.</span><span class="sxs-lookup"><span data-stu-id="bcaf0-119">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="bcaf0-120">riskScore</span><span class="sxs-lookup"><span data-stu-id="bcaf0-120">riskScore</span></span>|<span data-ttu-id="bcaf0-121">String</span><span class="sxs-lookup"><span data-stu-id="bcaf0-121">String</span></span>|<span data-ttu-id="bcaf0-122">Geração de um provedor/Pontuação de risco calculado do arquivo de alerta.</span><span class="sxs-lookup"><span data-stu-id="bcaf0-122">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="bcaf0-123">O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="bcaf0-123">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bcaf0-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bcaf0-124">JSON representation</span></span>

<span data-ttu-id="bcaf0-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bcaf0-125">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
