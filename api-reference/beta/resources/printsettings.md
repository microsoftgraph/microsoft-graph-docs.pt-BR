---
title: tipo de recurso printSettings
description: Representa configurações de todo o locatário para o serviço de impressão universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c9af888d85256b88d4212cc84ba74d8dcdd5b590
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973817"
---
# <a name="printsettings-resource-type"></a><span data-ttu-id="14b51-103">tipo de recurso printSettings</span><span class="sxs-lookup"><span data-stu-id="14b51-103">printSettings resource type</span></span>

<span data-ttu-id="14b51-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14b51-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14b51-105">Representa configurações de todo o locatário para o serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="14b51-105">Represents tenant-wide settings for the Universal Print service.</span></span>

## <a name="properties"></a><span data-ttu-id="14b51-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="14b51-106">Properties</span></span>
| <span data-ttu-id="14b51-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14b51-107">Property</span></span>     | <span data-ttu-id="14b51-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="14b51-108">Type</span></span>        | <span data-ttu-id="14b51-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="14b51-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="14b51-110">documentConversionEnabled</span><span class="sxs-lookup"><span data-stu-id="14b51-110">documentConversionEnabled</span></span>|<span data-ttu-id="14b51-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="14b51-111">Boolean</span></span>|<span data-ttu-id="14b51-112">Especifica se a conversão de documentos está habilitada para o locatário.</span><span class="sxs-lookup"><span data-stu-id="14b51-112">Specifies whether document conversion is enabled for the tenant.</span></span> <span data-ttu-id="14b51-113">Se a conversão de documentos estiver habilitada, o serviço de impressão universal converterá automaticamente os documentos em um formato compatível com a impressora (XPS para PDF), quando necessário.</span><span class="sxs-lookup"><span data-stu-id="14b51-113">If document conversion is enabled, Universal Print service will automatically convert documents into a format compatible with the printer (xps to pdf) when needed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="14b51-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="14b51-114">JSON representation</span></span>

<span data-ttu-id="14b51-115">Veja a seguir uma representação JSON de printSettings.</span><span class="sxs-lookup"><span data-stu-id="14b51-115">The following is a JSON representation of printSettings.</span></span>
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


