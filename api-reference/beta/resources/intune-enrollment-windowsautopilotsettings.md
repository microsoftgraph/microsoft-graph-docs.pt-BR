---
title: tipo de recurso windowsAutopilotSettings
description: O recurso windowsAutopilotSettings representa uma conta do Windows AutoPilot para sincronizar dados com o serviço de sincronização de dados do dispositivo Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b34d6edbed5bc98989ea70186b081d5c88a1c1b6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140513"
---
# <a name="windowsautopilotsettings-resource-type"></a><span data-ttu-id="ac7d2-103">tipo de recurso windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="ac7d2-103">windowsAutopilotSettings resource type</span></span>

> <span data-ttu-id="ac7d2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ac7d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac7d2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ac7d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac7d2-106">O recurso windowsAutopilotSettings representa uma conta do Windows AutoPilot para sincronizar dados com o serviço de sincronização de dados do dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="ac7d2-106">The windowsAutopilotSettings resource represents a Windows Autopilot Account to sync data with Windows device data sync service.</span></span>

## <a name="methods"></a><span data-ttu-id="ac7d2-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="ac7d2-107">Methods</span></span>
|<span data-ttu-id="ac7d2-108">Método</span><span class="sxs-lookup"><span data-stu-id="ac7d2-108">Method</span></span>|<span data-ttu-id="ac7d2-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ac7d2-109">Return Type</span></span>|<span data-ttu-id="ac7d2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac7d2-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ac7d2-111">Obter windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="ac7d2-111">Get windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-get.md)|[<span data-ttu-id="ac7d2-112">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="ac7d2-112">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="ac7d2-113">Leia as propriedades e as relações do objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="ac7d2-113">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="ac7d2-114">Atualizar windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="ac7d2-114">Update windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-update.md)|[<span data-ttu-id="ac7d2-115">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="ac7d2-115">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="ac7d2-116">Atualiza as propriedades de um objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="ac7d2-116">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="ac7d2-117">ação de sincronização</span><span class="sxs-lookup"><span data-stu-id="ac7d2-117">sync action</span></span>](../api/intune-enrollment-windowsautopilotsettings-sync.md)|<span data-ttu-id="ac7d2-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ac7d2-118">None</span></span>|<span data-ttu-id="ac7d2-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ac7d2-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ac7d2-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac7d2-120">Properties</span></span>
|<span data-ttu-id="ac7d2-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac7d2-121">Property</span></span>|<span data-ttu-id="ac7d2-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac7d2-122">Type</span></span>|<span data-ttu-id="ac7d2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac7d2-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac7d2-124">id</span><span class="sxs-lookup"><span data-stu-id="ac7d2-124">id</span></span>|<span data-ttu-id="ac7d2-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac7d2-125">String</span></span>|<span data-ttu-id="ac7d2-126">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="ac7d2-126">The GUID for the object</span></span>|
|<span data-ttu-id="ac7d2-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ac7d2-127">lastSyncDateTime</span></span>|<span data-ttu-id="ac7d2-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac7d2-128">DateTimeOffset</span></span>|<span data-ttu-id="ac7d2-129">Data e hora da última sincronização de dados com o DDS Service.</span><span class="sxs-lookup"><span data-stu-id="ac7d2-129">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="ac7d2-130">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="ac7d2-130">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="ac7d2-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac7d2-131">DateTimeOffset</span></span>|<span data-ttu-id="ac7d2-132">Data e hora da última sincronização de dados com o DDS Service.</span><span class="sxs-lookup"><span data-stu-id="ac7d2-132">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="ac7d2-133">syncStatus</span><span class="sxs-lookup"><span data-stu-id="ac7d2-133">syncStatus</span></span>|[<span data-ttu-id="ac7d2-134">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="ac7d2-134">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="ac7d2-135">Indica o status da sincronização com o serviço de DDS (sincronização de dados do dispositivo).</span><span class="sxs-lookup"><span data-stu-id="ac7d2-135">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="ac7d2-136">Os valores possíveis são: `unknown`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="ac7d2-136">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac7d2-137">Relações</span><span class="sxs-lookup"><span data-stu-id="ac7d2-137">Relationships</span></span>
<span data-ttu-id="ac7d2-138">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="ac7d2-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac7d2-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac7d2-139">JSON Representation</span></span>
<span data-ttu-id="ac7d2-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ac7d2-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "id": "String (identifier)",
  "lastSyncDateTime": "String (timestamp)",
  "lastManualSyncTriggerDateTime": "String (timestamp)",
  "syncStatus": "String"
}
```




