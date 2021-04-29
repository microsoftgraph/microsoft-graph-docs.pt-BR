---
title: Tipo de recurso ocrSettings
description: Configurações de OCR para um caso de Descoberta e
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 648e0ad63f558f211591d1c8aa976c2689dd271d
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080716"
---
# <a name="ocrsettings-resource-type"></a><span data-ttu-id="497c9-103">Tipo de recurso ocrSettings</span><span class="sxs-lookup"><span data-stu-id="497c9-103">ocrSettings resource type</span></span>

<span data-ttu-id="497c9-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="497c9-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="497c9-105">As configurações OCR (Reconhecimento Óptico de Caracteres) para o caso de Descoberta e.</span><span class="sxs-lookup"><span data-stu-id="497c9-105">The OCR (Optical Character Recognition) settings for the eDiscovery case.</span></span>

## <a name="properties"></a><span data-ttu-id="497c9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="497c9-106">Properties</span></span>

|<span data-ttu-id="497c9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="497c9-107">Property</span></span>|<span data-ttu-id="497c9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="497c9-108">Type</span></span>|<span data-ttu-id="497c9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="497c9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="497c9-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="497c9-110">isEnabled</span></span>|<span data-ttu-id="497c9-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="497c9-111">Boolean</span></span>|<span data-ttu-id="497c9-112">Indica se o OCR está habilitado ou não para o caso.</span><span class="sxs-lookup"><span data-stu-id="497c9-112">Indicates whether or not OCR is enabled for the case.</span></span>|
|<span data-ttu-id="497c9-113">maxImageSize</span><span class="sxs-lookup"><span data-stu-id="497c9-113">maxImageSize</span></span>|<span data-ttu-id="497c9-114">Int32</span><span class="sxs-lookup"><span data-stu-id="497c9-114">Int32</span></span>|<span data-ttu-id="497c9-115">Tamanho máximo da imagem que será processado em KB).</span><span class="sxs-lookup"><span data-stu-id="497c9-115">Maximum image size that will be processed in KB).</span></span>|
|<span data-ttu-id="497c9-116">timeout</span><span class="sxs-lookup"><span data-stu-id="497c9-116">timeout</span></span>|<span data-ttu-id="497c9-117">Duration</span><span class="sxs-lookup"><span data-stu-id="497c9-117">Duration</span></span>|<span data-ttu-id="497c9-118">A duração do tempo de duração do mecanismo OCR.</span><span class="sxs-lookup"><span data-stu-id="497c9-118">The timeout duration for the OCR engine.</span></span> <span data-ttu-id="497c9-119">Um tempo de tempo maior pode aumentar o sucesso do OCR, mas pode adicionar ao tempo total de processamento.</span><span class="sxs-lookup"><span data-stu-id="497c9-119">A longer timeout may increase success of OCR, but may add to the total processing time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="497c9-120">Relações</span><span class="sxs-lookup"><span data-stu-id="497c9-120">Relationships</span></span>

<span data-ttu-id="497c9-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="497c9-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="497c9-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="497c9-122">JSON representation</span></span>

<span data-ttu-id="497c9-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="497c9-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ediscovery.ocrSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.ocrSettings",
  "isEnabled": "Boolean",
  "maxImageSize": "Integer",
  "timeout": "String (duration)"
}
```
