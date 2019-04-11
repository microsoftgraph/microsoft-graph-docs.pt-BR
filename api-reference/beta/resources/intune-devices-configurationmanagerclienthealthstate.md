---
title: tipo de recurso configurationManagerClientHealthState
description: Estado de integridade do cliente de gerenciador de configurações
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e2a04b8cf7520425527e118fcc9db00461c4edda
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797736"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="d3278-103">tipo de recurso configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="d3278-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="d3278-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d3278-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3278-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d3278-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3278-106">Estado de integridade do cliente de gerenciador de configurações</span><span class="sxs-lookup"><span data-stu-id="d3278-106">Configuration manager client health state</span></span>

## <a name="properties"></a><span data-ttu-id="d3278-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d3278-107">Properties</span></span>
|<span data-ttu-id="d3278-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3278-108">Property</span></span>|<span data-ttu-id="d3278-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3278-109">Type</span></span>|<span data-ttu-id="d3278-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3278-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3278-111">state</span><span class="sxs-lookup"><span data-stu-id="d3278-111">state</span></span>|[<span data-ttu-id="d3278-112">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="d3278-112">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="d3278-113">Estado atual do cliente do Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="d3278-113">Current configuration manager client state.</span></span> <span data-ttu-id="d3278-114">Os valores possíveis são: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span><span class="sxs-lookup"><span data-stu-id="d3278-114">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="d3278-115">errorCode</span><span class="sxs-lookup"><span data-stu-id="d3278-115">errorCode</span></span>|<span data-ttu-id="d3278-116">Int32</span><span class="sxs-lookup"><span data-stu-id="d3278-116">Int32</span></span>|<span data-ttu-id="d3278-117">Código de erro para estado de falha.</span><span class="sxs-lookup"><span data-stu-id="d3278-117">Error code for failed state.</span></span>|
|<span data-ttu-id="d3278-118">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d3278-118">lastSyncDateTime</span></span>|<span data-ttu-id="d3278-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3278-119">DateTimeOffset</span></span>|<span data-ttu-id="d3278-120">DateTime fo última sincronização com o ponto de gerenciamento do Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="d3278-120">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3278-121">Relações</span><span class="sxs-lookup"><span data-stu-id="d3278-121">Relationships</span></span>
<span data-ttu-id="d3278-122">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d3278-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3278-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3278-123">JSON Representation</span></span>
<span data-ttu-id="d3278-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d3278-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientHealthState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientHealthState",
  "state": "String",
  "errorCode": 1024,
  "lastSyncDateTime": "String (timestamp)"
}
```





