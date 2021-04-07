---
title: Tipo de recurso deviceActionResult
description: Resultado de ação de dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dbf24152e5e804c713a7aa761b05e5b2a3b13997
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611885"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="14496-103">Tipo de recurso deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="14496-103">deviceActionResult resource type</span></span>

<span data-ttu-id="14496-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14496-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14496-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="14496-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14496-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="14496-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14496-107">Resultado de ação de dispositivo</span><span class="sxs-lookup"><span data-stu-id="14496-107">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="14496-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="14496-108">Properties</span></span>
|<span data-ttu-id="14496-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14496-109">Property</span></span>|<span data-ttu-id="14496-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="14496-110">Type</span></span>|<span data-ttu-id="14496-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="14496-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14496-112">actionName</span><span class="sxs-lookup"><span data-stu-id="14496-112">actionName</span></span>|<span data-ttu-id="14496-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14496-113">String</span></span>|<span data-ttu-id="14496-114">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="14496-114">Action name</span></span>|
|<span data-ttu-id="14496-115">actionState</span><span class="sxs-lookup"><span data-stu-id="14496-115">actionState</span></span>|[<span data-ttu-id="14496-116">actionState</span><span class="sxs-lookup"><span data-stu-id="14496-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="14496-117">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="14496-117">State of the action.</span></span> <span data-ttu-id="14496-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="14496-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="14496-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="14496-119">startDateTime</span></span>|<span data-ttu-id="14496-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14496-120">DateTimeOffset</span></span>|<span data-ttu-id="14496-121">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="14496-121">Time the action was initiated</span></span>|
|<span data-ttu-id="14496-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="14496-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="14496-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14496-123">DateTimeOffset</span></span>|<span data-ttu-id="14496-124">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="14496-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="14496-125">Relações</span><span class="sxs-lookup"><span data-stu-id="14496-125">Relationships</span></span>
<span data-ttu-id="14496-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="14496-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14496-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="14496-127">JSON Representation</span></span>
<span data-ttu-id="14496-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="14496-128">Here is a JSON representation of the resource.</span></span>
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




