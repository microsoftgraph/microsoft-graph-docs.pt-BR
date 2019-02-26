---
title: Tipo de recurso deviceActionResult
description: Resultado de ação de dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d08b4285f81c7b6f7e4962c4738279f84ba37b7d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261044"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="58573-103">Tipo de recurso deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="58573-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="58573-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="58573-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58573-105">Resultado de ação de dispositivo</span><span class="sxs-lookup"><span data-stu-id="58573-105">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="58573-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="58573-106">Properties</span></span>
|<span data-ttu-id="58573-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58573-107">Property</span></span>|<span data-ttu-id="58573-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="58573-108">Type</span></span>|<span data-ttu-id="58573-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="58573-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58573-110">actionName</span><span class="sxs-lookup"><span data-stu-id="58573-110">actionName</span></span>|<span data-ttu-id="58573-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58573-111">String</span></span>|<span data-ttu-id="58573-112">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="58573-112">Action name</span></span>|
|<span data-ttu-id="58573-113">actionState</span><span class="sxs-lookup"><span data-stu-id="58573-113">actionState</span></span>|[<span data-ttu-id="58573-114">actionState</span><span class="sxs-lookup"><span data-stu-id="58573-114">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="58573-115">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="58573-115">State of the action.</span></span> <span data-ttu-id="58573-116">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="58573-116">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="58573-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="58573-117">startDateTime</span></span>|<span data-ttu-id="58573-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58573-118">DateTimeOffset</span></span>|<span data-ttu-id="58573-119">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="58573-119">Time the action was initiated</span></span>|
|<span data-ttu-id="58573-120">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="58573-120">lastUpdatedDateTime</span></span>|<span data-ttu-id="58573-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58573-121">DateTimeOffset</span></span>|<span data-ttu-id="58573-122">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="58573-122">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="58573-123">Relações</span><span class="sxs-lookup"><span data-stu-id="58573-123">Relationships</span></span>
<span data-ttu-id="58573-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="58573-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58573-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="58573-125">JSON Representation</span></span>
<span data-ttu-id="58573-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="58573-126">Here is a JSON representation of the resource.</span></span>
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



