---
title: tipo de recurso windowsAutopilotSettings
description: O recurso windowsAutopilotSettings representa uma conta do Windows AutoPilot para sincronizar dados com o serviço de sincronização de dados do dispositivo Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4f6e65e2c898cbaaaf9d77b00cbf056d4cf369af
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49288625"
---
# <a name="windowsautopilotsettings-resource-type"></a><span data-ttu-id="2e507-103">tipo de recurso windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="2e507-103">windowsAutopilotSettings resource type</span></span>

<span data-ttu-id="2e507-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e507-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e507-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2e507-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e507-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2e507-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e507-107">O recurso windowsAutopilotSettings representa uma conta do Windows AutoPilot para sincronizar dados com o serviço de sincronização de dados do dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="2e507-107">The windowsAutopilotSettings resource represents a Windows Autopilot Account to sync data with Windows device data sync service.</span></span>

## <a name="methods"></a><span data-ttu-id="2e507-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="2e507-108">Methods</span></span>
|<span data-ttu-id="2e507-109">Método</span><span class="sxs-lookup"><span data-stu-id="2e507-109">Method</span></span>|<span data-ttu-id="2e507-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2e507-110">Return Type</span></span>|<span data-ttu-id="2e507-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e507-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2e507-112">Obter windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="2e507-112">Get windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-get.md)|[<span data-ttu-id="2e507-113">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="2e507-113">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="2e507-114">Leia as propriedades e as relações do objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="2e507-114">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="2e507-115">Atualizar windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="2e507-115">Update windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-update.md)|[<span data-ttu-id="2e507-116">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="2e507-116">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="2e507-117">Atualiza as propriedades de um objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="2e507-117">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="2e507-118">ação de sincronização</span><span class="sxs-lookup"><span data-stu-id="2e507-118">sync action</span></span>](../api/intune-enrollment-windowsautopilotsettings-sync.md)|<span data-ttu-id="2e507-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2e507-119">None</span></span>|<span data-ttu-id="2e507-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2e507-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2e507-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2e507-121">Properties</span></span>
|<span data-ttu-id="2e507-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2e507-122">Property</span></span>|<span data-ttu-id="2e507-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e507-123">Type</span></span>|<span data-ttu-id="2e507-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e507-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e507-125">id</span><span class="sxs-lookup"><span data-stu-id="2e507-125">id</span></span>|<span data-ttu-id="2e507-126">String</span><span class="sxs-lookup"><span data-stu-id="2e507-126">String</span></span>|<span data-ttu-id="2e507-127">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="2e507-127">The GUID for the object</span></span>|
|<span data-ttu-id="2e507-128">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2e507-128">lastSyncDateTime</span></span>|<span data-ttu-id="2e507-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e507-129">DateTimeOffset</span></span>|<span data-ttu-id="2e507-130">Data e hora da última sincronização de dados com o DDS Service.</span><span class="sxs-lookup"><span data-stu-id="2e507-130">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="2e507-131">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="2e507-131">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="2e507-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e507-132">DateTimeOffset</span></span>|<span data-ttu-id="2e507-133">Data e hora da última sincronização de dados com o DDS Service.</span><span class="sxs-lookup"><span data-stu-id="2e507-133">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="2e507-134">syncStatus</span><span class="sxs-lookup"><span data-stu-id="2e507-134">syncStatus</span></span>|[<span data-ttu-id="2e507-135">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="2e507-135">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="2e507-136">Indica o status da sincronização com o serviço de DDS (sincronização de dados do dispositivo).</span><span class="sxs-lookup"><span data-stu-id="2e507-136">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="2e507-137">Os valores possíveis são: `unknown`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="2e507-137">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e507-138">Relações</span><span class="sxs-lookup"><span data-stu-id="2e507-138">Relationships</span></span>
<span data-ttu-id="2e507-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2e507-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e507-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2e507-140">JSON Representation</span></span>
<span data-ttu-id="2e507-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2e507-141">Here is a JSON representation of the resource.</span></span>
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




