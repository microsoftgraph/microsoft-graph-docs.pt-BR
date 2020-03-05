---
title: Tipo de recurso deviceActionResult
description: Resultado de ação de dispositivo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f25b98f98f8a8350aa94c69029b7ae74de6513aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528651"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="fb3d5-103">Tipo de recurso deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="fb3d5-103">deviceActionResult resource type</span></span>

<span data-ttu-id="fb3d5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fb3d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb3d5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fb3d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb3d5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fb3d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb3d5-107">Resultado de ação de dispositivo</span><span class="sxs-lookup"><span data-stu-id="fb3d5-107">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="fb3d5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fb3d5-108">Properties</span></span>
|<span data-ttu-id="fb3d5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb3d5-109">Property</span></span>|<span data-ttu-id="fb3d5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb3d5-110">Type</span></span>|<span data-ttu-id="fb3d5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb3d5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb3d5-112">actionName</span><span class="sxs-lookup"><span data-stu-id="fb3d5-112">actionName</span></span>|<span data-ttu-id="fb3d5-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb3d5-113">String</span></span>|<span data-ttu-id="fb3d5-114">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="fb3d5-114">Action name</span></span>|
|<span data-ttu-id="fb3d5-115">actionState</span><span class="sxs-lookup"><span data-stu-id="fb3d5-115">actionState</span></span>|[<span data-ttu-id="fb3d5-116">actionState</span><span class="sxs-lookup"><span data-stu-id="fb3d5-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="fb3d5-117">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="fb3d5-117">State of the action.</span></span> <span data-ttu-id="fb3d5-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="fb3d5-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="fb3d5-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fb3d5-119">startDateTime</span></span>|<span data-ttu-id="fb3d5-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb3d5-120">DateTimeOffset</span></span>|<span data-ttu-id="fb3d5-121">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="fb3d5-121">Time the action was initiated</span></span>|
|<span data-ttu-id="fb3d5-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb3d5-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="fb3d5-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb3d5-123">DateTimeOffset</span></span>|<span data-ttu-id="fb3d5-124">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="fb3d5-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb3d5-125">Relações</span><span class="sxs-lookup"><span data-stu-id="fb3d5-125">Relationships</span></span>
<span data-ttu-id="fb3d5-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fb3d5-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb3d5-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fb3d5-127">JSON Representation</span></span>
<span data-ttu-id="fb3d5-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fb3d5-128">Here is a JSON representation of the resource.</span></span>
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



