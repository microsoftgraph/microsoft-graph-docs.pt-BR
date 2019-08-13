---
title: tipo de recurso configurationManagerClientHealthState
description: Estado de integridade do cliente de gerenciador de configurações
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ab1b47ac9371c0a0806ff03e18bf9cc7eed577f0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369462"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="ad2d7-103">tipo de recurso configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="ad2d7-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="ad2d7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ad2d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad2d7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ad2d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad2d7-106">Estado de integridade do cliente de gerenciador de configurações</span><span class="sxs-lookup"><span data-stu-id="ad2d7-106">Configuration manager client health state</span></span>

## <a name="properties"></a><span data-ttu-id="ad2d7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ad2d7-107">Properties</span></span>
|<span data-ttu-id="ad2d7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad2d7-108">Property</span></span>|<span data-ttu-id="ad2d7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad2d7-109">Type</span></span>|<span data-ttu-id="ad2d7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad2d7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad2d7-111">state</span><span class="sxs-lookup"><span data-stu-id="ad2d7-111">state</span></span>|[<span data-ttu-id="ad2d7-112">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="ad2d7-112">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="ad2d7-113">Estado atual do cliente do Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="ad2d7-113">Current configuration manager client state.</span></span> <span data-ttu-id="ad2d7-114">Os valores possíveis são: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span><span class="sxs-lookup"><span data-stu-id="ad2d7-114">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="ad2d7-115">errorCode</span><span class="sxs-lookup"><span data-stu-id="ad2d7-115">errorCode</span></span>|<span data-ttu-id="ad2d7-116">Int32</span><span class="sxs-lookup"><span data-stu-id="ad2d7-116">Int32</span></span>|<span data-ttu-id="ad2d7-117">Código de erro para estado de falha.</span><span class="sxs-lookup"><span data-stu-id="ad2d7-117">Error code for failed state.</span></span>|
|<span data-ttu-id="ad2d7-118">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ad2d7-118">lastSyncDateTime</span></span>|<span data-ttu-id="ad2d7-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad2d7-119">DateTimeOffset</span></span>|<span data-ttu-id="ad2d7-120">DateTime fo última sincronização com o ponto de gerenciamento do Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="ad2d7-120">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad2d7-121">Relações</span><span class="sxs-lookup"><span data-stu-id="ad2d7-121">Relationships</span></span>
<span data-ttu-id="ad2d7-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ad2d7-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad2d7-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ad2d7-123">JSON Representation</span></span>
<span data-ttu-id="ad2d7-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ad2d7-124">Here is a JSON representation of the resource.</span></span>
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



