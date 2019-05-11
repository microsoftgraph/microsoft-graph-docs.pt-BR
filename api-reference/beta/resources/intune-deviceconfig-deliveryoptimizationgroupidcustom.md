---
title: tipo de recurso deliveryOptimizationGroupIdCustom
description: Tipo de ID de grupo personalizado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e439b9d4777a0b0c513d750d0b5e35783dbd9a1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947250"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a><span data-ttu-id="32cdb-103">tipo de recurso deliveryOptimizationGroupIdCustom</span><span class="sxs-lookup"><span data-stu-id="32cdb-103">deliveryOptimizationGroupIdCustom resource type</span></span>

> <span data-ttu-id="32cdb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="32cdb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32cdb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="32cdb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32cdb-106">Tipo de ID de grupo personalizado</span><span class="sxs-lookup"><span data-stu-id="32cdb-106">Custom group id type</span></span>


<span data-ttu-id="32cdb-107">Herda de [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="32cdb-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="32cdb-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="32cdb-108">Properties</span></span>
|<span data-ttu-id="32cdb-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32cdb-109">Property</span></span>|<span data-ttu-id="32cdb-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="32cdb-110">Type</span></span>|<span data-ttu-id="32cdb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="32cdb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32cdb-112">groupIdCustom</span><span class="sxs-lookup"><span data-stu-id="32cdb-112">groupIdCustom</span></span>|<span data-ttu-id="32cdb-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32cdb-113">String</span></span>|<span data-ttu-id="32cdb-114">Especifica uma ID de grupo arbitrária à qual o dispositivo pertence</span><span class="sxs-lookup"><span data-stu-id="32cdb-114">Specifies an arbitrary group ID that the device belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="32cdb-115">Relações</span><span class="sxs-lookup"><span data-stu-id="32cdb-115">Relationships</span></span>
<span data-ttu-id="32cdb-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="32cdb-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32cdb-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="32cdb-117">JSON Representation</span></span>
<span data-ttu-id="32cdb-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="32cdb-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationGroupIdCustom",
  "groupIdCustom": "String"
}
```




