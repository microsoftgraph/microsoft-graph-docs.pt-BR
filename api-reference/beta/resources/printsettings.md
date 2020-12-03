---
title: tipo de recurso printSettings
description: Representa configurações de todo o locatário para o serviço de impressão universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 01c98eb68031018e6f7a32837e49a2095c7880d2
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521233"
---
# <a name="printsettings-resource-type"></a><span data-ttu-id="b4d3b-103">tipo de recurso printSettings</span><span class="sxs-lookup"><span data-stu-id="b4d3b-103">printSettings resource type</span></span>

<span data-ttu-id="b4d3b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4d3b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4d3b-105">Representa configurações de todo o locatário para o serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="b4d3b-105">Represents tenant-wide settings for the Universal Print service.</span></span>

## <a name="properties"></a><span data-ttu-id="b4d3b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4d3b-106">Properties</span></span>
| <span data-ttu-id="b4d3b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4d3b-107">Property</span></span>     | <span data-ttu-id="b4d3b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4d3b-108">Type</span></span>        | <span data-ttu-id="b4d3b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4d3b-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b4d3b-110">documentConversionEnabled</span><span class="sxs-lookup"><span data-stu-id="b4d3b-110">documentConversionEnabled</span></span>|<span data-ttu-id="b4d3b-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4d3b-111">Boolean</span></span>|<span data-ttu-id="b4d3b-112">Especifica se a conversão de documentos está habilitada para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b4d3b-112">Specifies whether document conversion is enabled for the tenant.</span></span> <span data-ttu-id="b4d3b-113">Se a conversão de documentos estiver habilitada, o serviço de impressão universal converterá automaticamente os documentos em um formato compatível com a impressora (XPS para PDF), quando necessário.</span><span class="sxs-lookup"><span data-stu-id="b4d3b-113">If document conversion is enabled, Universal Print service will automatically convert documents into a format compatible with the printer (xps to pdf) when needed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b4d3b-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4d3b-114">JSON representation</span></span>

<span data-ttu-id="b4d3b-115">Veja a seguir uma representação JSON de printSettings.</span><span class="sxs-lookup"><span data-stu-id="b4d3b-115">The following is a JSON representation of printSettings.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printSettings"
}-->

```json
{
  "documentConversionEnabled": true
}
```


