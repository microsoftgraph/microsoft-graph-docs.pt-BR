---
title: tipo de recurso de configurationManagerClientHealthState
description: Estado de integridade de cliente do Configuration manager
ms.openlocfilehash: f2724f5d230ee539720e105daf1758bf727bee26
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034516"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="bcdea-103">tipo de recurso de configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="bcdea-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="bcdea-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bcdea-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bcdea-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bcdea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bcdea-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bcdea-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bcdea-107">Estado de integridade de cliente do Configuration manager</span><span class="sxs-lookup"><span data-stu-id="bcdea-107">Configuration manager client health state</span></span>
## <a name="properties"></a><span data-ttu-id="bcdea-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bcdea-108">Properties</span></span>
|<span data-ttu-id="bcdea-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bcdea-109">Property</span></span>|<span data-ttu-id="bcdea-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bcdea-110">Type</span></span>|<span data-ttu-id="bcdea-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bcdea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcdea-112">state</span><span class="sxs-lookup"><span data-stu-id="bcdea-112">state</span></span>|[<span data-ttu-id="bcdea-113">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="bcdea-113">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="bcdea-114">Estado da cliente do Gerenciador de configuração atual.</span><span class="sxs-lookup"><span data-stu-id="bcdea-114">Current configuration manager client state.</span></span> <span data-ttu-id="bcdea-115">Os valores possíveis são: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span><span class="sxs-lookup"><span data-stu-id="bcdea-115">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="bcdea-116">errorCode</span><span class="sxs-lookup"><span data-stu-id="bcdea-116">errorCode</span></span>|<span data-ttu-id="bcdea-117">Int32</span><span class="sxs-lookup"><span data-stu-id="bcdea-117">Int32</span></span>|<span data-ttu-id="bcdea-118">Código de erro para o estado de falha.</span><span class="sxs-lookup"><span data-stu-id="bcdea-118">Error code for failed state.</span></span>|
|<span data-ttu-id="bcdea-119">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="bcdea-119">lastSyncDateTime</span></span>|<span data-ttu-id="bcdea-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcdea-120">DateTimeOffset</span></span>|<span data-ttu-id="bcdea-121">Ponto de DateTime fo última sincronização com o gerenciamento do Gerenciador de configuração.</span><span class="sxs-lookup"><span data-stu-id="bcdea-121">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bcdea-122">Relações</span><span class="sxs-lookup"><span data-stu-id="bcdea-122">Relationships</span></span>
<span data-ttu-id="bcdea-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bcdea-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bcdea-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bcdea-124">JSON Representation</span></span>
<span data-ttu-id="bcdea-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bcdea-125">Here is a JSON representation of the resource.</span></span>
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





