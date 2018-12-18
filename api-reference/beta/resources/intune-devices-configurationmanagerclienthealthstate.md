---
title: tipo de recurso de configurationManagerClientHealthState
description: Estado de integridade de cliente do Configuration manager
author: tfitzmac
ms.openlocfilehash: 8361d74f675cf1eaf70b78e2350aae2fc6e83554
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302783"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="4b97e-103">tipo de recurso de configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="4b97e-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="4b97e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4b97e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b97e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4b97e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b97e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4b97e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b97e-107">Estado de integridade de cliente do Configuration manager</span><span class="sxs-lookup"><span data-stu-id="4b97e-107">Configuration manager client health state</span></span>
## <a name="properties"></a><span data-ttu-id="4b97e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4b97e-108">Properties</span></span>
|<span data-ttu-id="4b97e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b97e-109">Property</span></span>|<span data-ttu-id="4b97e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b97e-110">Type</span></span>|<span data-ttu-id="4b97e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b97e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b97e-112">state</span><span class="sxs-lookup"><span data-stu-id="4b97e-112">state</span></span>|[<span data-ttu-id="4b97e-113">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="4b97e-113">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="4b97e-114">Estado da cliente do Gerenciador de configuração atual.</span><span class="sxs-lookup"><span data-stu-id="4b97e-114">Current configuration manager client state.</span></span> <span data-ttu-id="4b97e-115">Os valores possíveis são: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span><span class="sxs-lookup"><span data-stu-id="4b97e-115">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="4b97e-116">errorCode</span><span class="sxs-lookup"><span data-stu-id="4b97e-116">errorCode</span></span>|<span data-ttu-id="4b97e-117">Int32</span><span class="sxs-lookup"><span data-stu-id="4b97e-117">Int32</span></span>|<span data-ttu-id="4b97e-118">Código de erro para o estado de falha.</span><span class="sxs-lookup"><span data-stu-id="4b97e-118">Error code for failed state.</span></span>|
|<span data-ttu-id="4b97e-119">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4b97e-119">lastSyncDateTime</span></span>|<span data-ttu-id="4b97e-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b97e-120">DateTimeOffset</span></span>|<span data-ttu-id="4b97e-121">Ponto de DateTime fo última sincronização com o gerenciamento do Gerenciador de configuração.</span><span class="sxs-lookup"><span data-stu-id="4b97e-121">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b97e-122">Relações</span><span class="sxs-lookup"><span data-stu-id="4b97e-122">Relationships</span></span>
<span data-ttu-id="4b97e-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4b97e-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4b97e-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4b97e-124">JSON Representation</span></span>
<span data-ttu-id="4b97e-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4b97e-125">Here is a JSON representation of the resource.</span></span>
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





