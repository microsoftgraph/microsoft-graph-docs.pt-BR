---
title: Tipo de recurso rgbColor
description: Cor em RGB.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 505383227d1014f779cb558d43c18da29d3989aa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395514"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="846fd-103">Tipo de recurso rgbColor</span><span class="sxs-lookup"><span data-stu-id="846fd-103">rgbColor resource type</span></span>

> <span data-ttu-id="846fd-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="846fd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="846fd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="846fd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="846fd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="846fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="846fd-107">Cor em RGB.</span><span class="sxs-lookup"><span data-stu-id="846fd-107">Color in RGB.</span></span>

## <a name="properties"></a><span data-ttu-id="846fd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="846fd-108">Properties</span></span>
|<span data-ttu-id="846fd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="846fd-109">Property</span></span>|<span data-ttu-id="846fd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="846fd-110">Type</span></span>|<span data-ttu-id="846fd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="846fd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="846fd-112">r</span><span class="sxs-lookup"><span data-stu-id="846fd-112">r</span></span>|<span data-ttu-id="846fd-113">Byte</span><span class="sxs-lookup"><span data-stu-id="846fd-113">Byte</span></span>|<span data-ttu-id="846fd-114">Valor de vermelho</span><span class="sxs-lookup"><span data-stu-id="846fd-114">Red value</span></span>|
|<span data-ttu-id="846fd-115">g</span><span class="sxs-lookup"><span data-stu-id="846fd-115">g</span></span>|<span data-ttu-id="846fd-116">Byte</span><span class="sxs-lookup"><span data-stu-id="846fd-116">Byte</span></span>|<span data-ttu-id="846fd-117">Valor de verde</span><span class="sxs-lookup"><span data-stu-id="846fd-117">Green value</span></span>|
|<span data-ttu-id="846fd-118">b</span><span class="sxs-lookup"><span data-stu-id="846fd-118">b</span></span>|<span data-ttu-id="846fd-119">Byte</span><span class="sxs-lookup"><span data-stu-id="846fd-119">Byte</span></span>|<span data-ttu-id="846fd-120">Valor de azul</span><span class="sxs-lookup"><span data-stu-id="846fd-120">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="846fd-121">Relações</span><span class="sxs-lookup"><span data-stu-id="846fd-121">Relationships</span></span>
<span data-ttu-id="846fd-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="846fd-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="846fd-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="846fd-123">JSON Representation</span></span>
<span data-ttu-id="846fd-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="846fd-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rgbColor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rgbColor",
  "r": 1024,
  "g": 1024,
  "b": 1024
}
```




