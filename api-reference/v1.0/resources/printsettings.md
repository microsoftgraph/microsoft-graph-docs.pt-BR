---
title: Tipo de recurso printSettings
description: Representa as configurações de todo o locatário para o serviço de Impressão Universal.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 53e0db2a1923cad0af1f35baf5bed6fecd896fb3
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516861"
---
# <a name="printsettings-resource-type"></a><span data-ttu-id="2dfcf-103">Tipo de recurso printSettings</span><span class="sxs-lookup"><span data-stu-id="2dfcf-103">printSettings resource type</span></span>

<span data-ttu-id="2dfcf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2dfcf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="2dfcf-105">Representa as configurações de todo o locatário para o serviço de Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="2dfcf-105">Represents tenant-wide settings for the Universal Print service.</span></span>

## <a name="properties"></a><span data-ttu-id="2dfcf-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2dfcf-106">Properties</span></span>
|<span data-ttu-id="2dfcf-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2dfcf-107">Property</span></span>|<span data-ttu-id="2dfcf-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2dfcf-108">Type</span></span>|<span data-ttu-id="2dfcf-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2dfcf-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dfcf-110">documentConversionEnabled</span><span class="sxs-lookup"><span data-stu-id="2dfcf-110">documentConversionEnabled</span></span>|<span data-ttu-id="2dfcf-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="2dfcf-111">Boolean</span></span>|<span data-ttu-id="2dfcf-112">Especifica se a conversão de documento está habilitada para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2dfcf-112">Specifies whether document conversion is enabled for the tenant.</span></span> <span data-ttu-id="2dfcf-113">Se a conversão de documentos estiver habilitada, o serviço de Impressão Universal converterá automaticamente documentos em um formato compatível com a impressora (xps para pdf) quando necessário.</span><span class="sxs-lookup"><span data-stu-id="2dfcf-113">If document conversion is enabled, Universal Print service will automatically convert documents into a format compatible with the printer (xps to pdf) when needed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2dfcf-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2dfcf-114">JSON representation</span></span>
<span data-ttu-id="2dfcf-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2dfcf-115">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printSettings",
  "documentConversionEnabled": "Boolean"
}
```

