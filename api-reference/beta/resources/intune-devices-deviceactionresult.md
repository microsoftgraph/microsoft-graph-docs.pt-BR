---
title: Tipo de recurso deviceActionResult
description: Resultado de ação de dispositivo
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0f0e6612eccf309cc03dea51c50dfcf06d1b6567
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456875"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="75f16-103">Tipo de recurso deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="75f16-103">deviceActionResult resource type</span></span>

<span data-ttu-id="75f16-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75f16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75f16-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="75f16-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75f16-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75f16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75f16-107">Resultado de ação de dispositivo</span><span class="sxs-lookup"><span data-stu-id="75f16-107">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="75f16-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75f16-108">Properties</span></span>
|<span data-ttu-id="75f16-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75f16-109">Property</span></span>|<span data-ttu-id="75f16-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="75f16-110">Type</span></span>|<span data-ttu-id="75f16-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="75f16-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75f16-112">actionName</span><span class="sxs-lookup"><span data-stu-id="75f16-112">actionName</span></span>|<span data-ttu-id="75f16-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75f16-113">String</span></span>|<span data-ttu-id="75f16-114">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="75f16-114">Action name</span></span>|
|<span data-ttu-id="75f16-115">actionState</span><span class="sxs-lookup"><span data-stu-id="75f16-115">actionState</span></span>|[<span data-ttu-id="75f16-116">actionState</span><span class="sxs-lookup"><span data-stu-id="75f16-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="75f16-117">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="75f16-117">State of the action.</span></span> <span data-ttu-id="75f16-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="75f16-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="75f16-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="75f16-119">startDateTime</span></span>|<span data-ttu-id="75f16-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75f16-120">DateTimeOffset</span></span>|<span data-ttu-id="75f16-121">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="75f16-121">Time the action was initiated</span></span>|
|<span data-ttu-id="75f16-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="75f16-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="75f16-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75f16-123">DateTimeOffset</span></span>|<span data-ttu-id="75f16-124">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="75f16-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="75f16-125">Relações</span><span class="sxs-lookup"><span data-stu-id="75f16-125">Relationships</span></span>
<span data-ttu-id="75f16-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="75f16-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="75f16-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75f16-127">JSON Representation</span></span>
<span data-ttu-id="75f16-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="75f16-128">Here is a JSON representation of the resource.</span></span>
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



