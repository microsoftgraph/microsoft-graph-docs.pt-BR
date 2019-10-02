---
title: Tipo de recurso deviceActionResult
description: Resultado de ação de dispositivo
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 593df6737c83b46f560d983f031bfadc12fb18c9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356986"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="6a55b-103">Tipo de recurso deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="6a55b-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="6a55b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a55b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a55b-105">Resultado de ação de dispositivo</span><span class="sxs-lookup"><span data-stu-id="6a55b-105">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="6a55b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a55b-106">Properties</span></span>
|<span data-ttu-id="6a55b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a55b-107">Property</span></span>|<span data-ttu-id="6a55b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a55b-108">Type</span></span>|<span data-ttu-id="6a55b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a55b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a55b-110">actionName</span><span class="sxs-lookup"><span data-stu-id="6a55b-110">actionName</span></span>|<span data-ttu-id="6a55b-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a55b-111">String</span></span>|<span data-ttu-id="6a55b-112">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="6a55b-112">Action name</span></span>|
|<span data-ttu-id="6a55b-113">actionState</span><span class="sxs-lookup"><span data-stu-id="6a55b-113">actionState</span></span>|[<span data-ttu-id="6a55b-114">actionState</span><span class="sxs-lookup"><span data-stu-id="6a55b-114">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="6a55b-115">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="6a55b-115">State of the action.</span></span> <span data-ttu-id="6a55b-116">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="6a55b-116">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="6a55b-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6a55b-117">startDateTime</span></span>|<span data-ttu-id="6a55b-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a55b-118">DateTimeOffset</span></span>|<span data-ttu-id="6a55b-119">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="6a55b-119">Time the action was initiated</span></span>|
|<span data-ttu-id="6a55b-120">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a55b-120">lastUpdatedDateTime</span></span>|<span data-ttu-id="6a55b-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a55b-121">DateTimeOffset</span></span>|<span data-ttu-id="6a55b-122">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="6a55b-122">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a55b-123">Relações</span><span class="sxs-lookup"><span data-stu-id="6a55b-123">Relationships</span></span>
<span data-ttu-id="6a55b-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a55b-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a55b-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a55b-125">JSON Representation</span></span>
<span data-ttu-id="6a55b-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6a55b-126">Here is a JSON representation of the resource.</span></span>
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




