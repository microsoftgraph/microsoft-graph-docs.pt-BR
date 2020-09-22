---
title: tipo de recurso numberRange
description: Definição do intervalo de números.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c9f2cf7d1a79b59f289a607820ff82412591c784
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019527"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="7f358-103">tipo de recurso numberRange</span><span class="sxs-lookup"><span data-stu-id="7f358-103">numberRange resource type</span></span>

<span data-ttu-id="7f358-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f358-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f358-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7f358-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f358-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7f358-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f358-107">Definição do intervalo de números.</span><span class="sxs-lookup"><span data-stu-id="7f358-107">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="7f358-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f358-108">Properties</span></span>
|<span data-ttu-id="7f358-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f358-109">Property</span></span>|<span data-ttu-id="7f358-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f358-110">Type</span></span>|<span data-ttu-id="7f358-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f358-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f358-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="7f358-112">lowerNumber</span></span>|<span data-ttu-id="7f358-113">Int32</span><span class="sxs-lookup"><span data-stu-id="7f358-113">Int32</span></span>|<span data-ttu-id="7f358-114">Número menor.</span><span class="sxs-lookup"><span data-stu-id="7f358-114">Lower number.</span></span>|
|<span data-ttu-id="7f358-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="7f358-115">upperNumber</span></span>|<span data-ttu-id="7f358-116">Int32</span><span class="sxs-lookup"><span data-stu-id="7f358-116">Int32</span></span>|<span data-ttu-id="7f358-117">Número superior.</span><span class="sxs-lookup"><span data-stu-id="7f358-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f358-118">Relações</span><span class="sxs-lookup"><span data-stu-id="7f358-118">Relationships</span></span>
<span data-ttu-id="7f358-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7f358-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f358-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f358-120">JSON Representation</span></span>
<span data-ttu-id="7f358-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7f358-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.numberRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.numberRange",
  "lowerNumber": 1024,
  "upperNumber": 1024
}
```






