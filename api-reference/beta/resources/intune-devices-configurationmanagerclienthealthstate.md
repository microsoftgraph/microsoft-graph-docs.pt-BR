---
title: tipo de recurso de configurationManagerClientHealthState
description: Estado de integridade de cliente do Configuration manager
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9eedca9f3ab7ddf10ab73c62d986fed393dcfa48
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806066"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="23202-103">tipo de recurso de configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="23202-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="23202-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="23202-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23202-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="23202-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23202-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="23202-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23202-107">Estado de integridade de cliente do Configuration manager</span><span class="sxs-lookup"><span data-stu-id="23202-107">Configuration manager client health state</span></span>
## <a name="properties"></a><span data-ttu-id="23202-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23202-108">Properties</span></span>
|<span data-ttu-id="23202-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23202-109">Property</span></span>|<span data-ttu-id="23202-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="23202-110">Type</span></span>|<span data-ttu-id="23202-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="23202-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23202-112">state</span><span class="sxs-lookup"><span data-stu-id="23202-112">state</span></span>|[<span data-ttu-id="23202-113">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="23202-113">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="23202-114">Estado da cliente do Gerenciador de configuração atual.</span><span class="sxs-lookup"><span data-stu-id="23202-114">Current configuration manager client state.</span></span> <span data-ttu-id="23202-115">Os valores possíveis são: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span><span class="sxs-lookup"><span data-stu-id="23202-115">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="23202-116">errorCode</span><span class="sxs-lookup"><span data-stu-id="23202-116">errorCode</span></span>|<span data-ttu-id="23202-117">Int32</span><span class="sxs-lookup"><span data-stu-id="23202-117">Int32</span></span>|<span data-ttu-id="23202-118">Código de erro para o estado de falha.</span><span class="sxs-lookup"><span data-stu-id="23202-118">Error code for failed state.</span></span>|
|<span data-ttu-id="23202-119">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="23202-119">lastSyncDateTime</span></span>|<span data-ttu-id="23202-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23202-120">DateTimeOffset</span></span>|<span data-ttu-id="23202-121">Ponto de DateTime fo última sincronização com o gerenciamento do Gerenciador de configuração.</span><span class="sxs-lookup"><span data-stu-id="23202-121">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23202-122">Relações</span><span class="sxs-lookup"><span data-stu-id="23202-122">Relationships</span></span>
<span data-ttu-id="23202-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23202-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="23202-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23202-124">JSON Representation</span></span>
<span data-ttu-id="23202-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23202-125">Here is a JSON representation of the resource.</span></span>
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





