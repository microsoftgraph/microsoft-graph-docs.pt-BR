---
title: Tipo de recurso deviceActionResult
description: Resultado de ação de dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 808d9e559494338a7831626fd6d4d77f20092dcb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755774"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="e088a-103">Tipo de recurso deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="e088a-103">deviceActionResult resource type</span></span>

<span data-ttu-id="e088a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e088a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e088a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e088a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e088a-106">Resultado de ação de dispositivo</span><span class="sxs-lookup"><span data-stu-id="e088a-106">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="e088a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e088a-107">Properties</span></span>
|<span data-ttu-id="e088a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e088a-108">Property</span></span>|<span data-ttu-id="e088a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e088a-109">Type</span></span>|<span data-ttu-id="e088a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e088a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e088a-111">actionName</span><span class="sxs-lookup"><span data-stu-id="e088a-111">actionName</span></span>|<span data-ttu-id="e088a-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e088a-112">String</span></span>|<span data-ttu-id="e088a-113">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="e088a-113">Action name</span></span>|
|<span data-ttu-id="e088a-114">actionState</span><span class="sxs-lookup"><span data-stu-id="e088a-114">actionState</span></span>|[<span data-ttu-id="e088a-115">actionState</span><span class="sxs-lookup"><span data-stu-id="e088a-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="e088a-116">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="e088a-116">State of the action.</span></span> <span data-ttu-id="e088a-117">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="e088a-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="e088a-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e088a-118">startDateTime</span></span>|<span data-ttu-id="e088a-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e088a-119">DateTimeOffset</span></span>|<span data-ttu-id="e088a-120">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="e088a-120">Time the action was initiated</span></span>|
|<span data-ttu-id="e088a-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e088a-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="e088a-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e088a-122">DateTimeOffset</span></span>|<span data-ttu-id="e088a-123">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="e088a-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="e088a-124">Relações</span><span class="sxs-lookup"><span data-stu-id="e088a-124">Relationships</span></span>
<span data-ttu-id="e088a-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e088a-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e088a-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e088a-126">JSON Representation</span></span>
<span data-ttu-id="e088a-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e088a-127">Here is a JSON representation of the resource.</span></span>
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




