---
title: tipo de recurso configurationManagerClientHealthState
description: Estado de integridade do cliente de gerenciador de configurações
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f860dd86f596983975a44762fcb5168b29bf84bf
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690263"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="20080-103">tipo de recurso configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="20080-103">configurationManagerClientHealthState resource type</span></span>

<span data-ttu-id="20080-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20080-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="20080-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="20080-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20080-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="20080-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20080-107">Estado de integridade do cliente de gerenciador de configurações</span><span class="sxs-lookup"><span data-stu-id="20080-107">Configuration manager client health state</span></span>

## <a name="properties"></a><span data-ttu-id="20080-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20080-108">Properties</span></span>
|<span data-ttu-id="20080-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20080-109">Property</span></span>|<span data-ttu-id="20080-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="20080-110">Type</span></span>|<span data-ttu-id="20080-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="20080-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20080-112">state</span><span class="sxs-lookup"><span data-stu-id="20080-112">state</span></span>|[<span data-ttu-id="20080-113">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="20080-113">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="20080-114">Estado atual do cliente do Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="20080-114">Current configuration manager client state.</span></span> <span data-ttu-id="20080-115">Os valores possíveis são: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span><span class="sxs-lookup"><span data-stu-id="20080-115">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="20080-116">errorCode</span><span class="sxs-lookup"><span data-stu-id="20080-116">errorCode</span></span>|<span data-ttu-id="20080-117">Int32</span><span class="sxs-lookup"><span data-stu-id="20080-117">Int32</span></span>|<span data-ttu-id="20080-118">Código de erro para estado de falha.</span><span class="sxs-lookup"><span data-stu-id="20080-118">Error code for failed state.</span></span>|
|<span data-ttu-id="20080-119">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="20080-119">lastSyncDateTime</span></span>|<span data-ttu-id="20080-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20080-120">DateTimeOffset</span></span>|<span data-ttu-id="20080-121">DateTime da última sincronização com o ponto de gerenciamento do Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="20080-121">Datetime for last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20080-122">Relações</span><span class="sxs-lookup"><span data-stu-id="20080-122">Relationships</span></span>
<span data-ttu-id="20080-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="20080-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="20080-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20080-124">JSON Representation</span></span>
<span data-ttu-id="20080-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="20080-125">Here is a JSON representation of the resource.</span></span>
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





