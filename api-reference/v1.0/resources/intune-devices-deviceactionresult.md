---
title: Tipo de recurso deviceActionResult
description: Resultado de ação de dispositivo
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1b802d1b09fbe65e9e1e72e4c34a387462e12113
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861121"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="31497-103">Tipo de recurso deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="31497-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="31497-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="31497-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31497-105">Resultado de ação de dispositivo</span><span class="sxs-lookup"><span data-stu-id="31497-105">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="31497-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="31497-106">Properties</span></span>
|<span data-ttu-id="31497-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31497-107">Property</span></span>|<span data-ttu-id="31497-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="31497-108">Type</span></span>|<span data-ttu-id="31497-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="31497-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31497-110">actionName</span><span class="sxs-lookup"><span data-stu-id="31497-110">actionName</span></span>|<span data-ttu-id="31497-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31497-111">String</span></span>|<span data-ttu-id="31497-112">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="31497-112">Action name</span></span>|
|<span data-ttu-id="31497-113">actionState</span><span class="sxs-lookup"><span data-stu-id="31497-113">actionState</span></span>|[<span data-ttu-id="31497-114">actionState</span><span class="sxs-lookup"><span data-stu-id="31497-114">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="31497-115">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="31497-115">State of the action.</span></span> <span data-ttu-id="31497-116">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="31497-116">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="31497-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="31497-117">startDateTime</span></span>|<span data-ttu-id="31497-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31497-118">DateTimeOffset</span></span>|<span data-ttu-id="31497-119">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="31497-119">Time the action was initiated</span></span>|
|<span data-ttu-id="31497-120">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="31497-120">lastUpdatedDateTime</span></span>|<span data-ttu-id="31497-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31497-121">DateTimeOffset</span></span>|<span data-ttu-id="31497-122">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="31497-122">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="31497-123">Relações</span><span class="sxs-lookup"><span data-stu-id="31497-123">Relationships</span></span>
<span data-ttu-id="31497-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="31497-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="31497-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="31497-125">JSON Representation</span></span>
<span data-ttu-id="31497-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="31497-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```



