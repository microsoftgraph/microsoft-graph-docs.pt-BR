---
title: tipo de recurso configurationManagerClientHealthState
description: Estado de integridade do cliente de gerenciador de configurações
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1c1c707d118b666f52e8a898cd0ad258c5cc8308
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465034"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="df969-103">tipo de recurso configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="df969-103">configurationManagerClientHealthState resource type</span></span>

<span data-ttu-id="df969-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df969-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df969-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="df969-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df969-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="df969-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df969-107">Estado de integridade do cliente de gerenciador de configurações</span><span class="sxs-lookup"><span data-stu-id="df969-107">Configuration manager client health state</span></span>

## <a name="properties"></a><span data-ttu-id="df969-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df969-108">Properties</span></span>
|<span data-ttu-id="df969-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df969-109">Property</span></span>|<span data-ttu-id="df969-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="df969-110">Type</span></span>|<span data-ttu-id="df969-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="df969-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df969-112">state</span><span class="sxs-lookup"><span data-stu-id="df969-112">state</span></span>|[<span data-ttu-id="df969-113">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="df969-113">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="df969-114">Estado atual do cliente do Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="df969-114">Current configuration manager client state.</span></span> <span data-ttu-id="df969-115">Os valores possíveis são: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span><span class="sxs-lookup"><span data-stu-id="df969-115">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="df969-116">errorCode</span><span class="sxs-lookup"><span data-stu-id="df969-116">errorCode</span></span>|<span data-ttu-id="df969-117">Int32</span><span class="sxs-lookup"><span data-stu-id="df969-117">Int32</span></span>|<span data-ttu-id="df969-118">Código de erro para estado de falha.</span><span class="sxs-lookup"><span data-stu-id="df969-118">Error code for failed state.</span></span>|
|<span data-ttu-id="df969-119">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="df969-119">lastSyncDateTime</span></span>|<span data-ttu-id="df969-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df969-120">DateTimeOffset</span></span>|<span data-ttu-id="df969-121">DateTime da última sincronização com o ponto de gerenciamento do Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="df969-121">Datetime for last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df969-122">Relações</span><span class="sxs-lookup"><span data-stu-id="df969-122">Relationships</span></span>
<span data-ttu-id="df969-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="df969-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="df969-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df969-124">JSON Representation</span></span>
<span data-ttu-id="df969-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="df969-125">Here is a JSON representation of the resource.</span></span>
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



