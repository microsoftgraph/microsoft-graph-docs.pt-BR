---
title: tipo de recurso windowsAutopilotSettings
description: O recurso windowsAutopilotSettings representa uma conta do Windows AutoPilot para sincronizar dados com o serviço de sincronização de dados do dispositivo Windows.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d5f7893b7a9dd01a3ea7c41875f235870a5ce27f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941433"
---
# <a name="windowsautopilotsettings-resource-type"></a><span data-ttu-id="5584e-103">tipo de recurso windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="5584e-103">windowsAutopilotSettings resource type</span></span>

> <span data-ttu-id="5584e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5584e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5584e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5584e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5584e-106">O recurso windowsAutopilotSettings representa uma conta do Windows AutoPilot para sincronizar dados com o serviço de sincronização de dados do dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="5584e-106">The windowsAutopilotSettings resource represents a Windows Autopilot Account to sync data with Windows device data sync service.</span></span>

## <a name="methods"></a><span data-ttu-id="5584e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="5584e-107">Methods</span></span>
|<span data-ttu-id="5584e-108">Método</span><span class="sxs-lookup"><span data-stu-id="5584e-108">Method</span></span>|<span data-ttu-id="5584e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5584e-109">Return Type</span></span>|<span data-ttu-id="5584e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5584e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5584e-111">Obter windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="5584e-111">Get windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-get.md)|[<span data-ttu-id="5584e-112">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="5584e-112">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="5584e-113">Leia as propriedades e as relações do objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="5584e-113">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="5584e-114">Atualizar windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="5584e-114">Update windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-update.md)|[<span data-ttu-id="5584e-115">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="5584e-115">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="5584e-116">Atualiza as propriedades de um objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="5584e-116">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="5584e-117">ação de sincronização</span><span class="sxs-lookup"><span data-stu-id="5584e-117">sync action</span></span>](../api/intune-enrollment-windowsautopilotsettings-sync.md)|<span data-ttu-id="5584e-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5584e-118">None</span></span>|<span data-ttu-id="5584e-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5584e-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5584e-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5584e-120">Properties</span></span>
|<span data-ttu-id="5584e-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5584e-121">Property</span></span>|<span data-ttu-id="5584e-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="5584e-122">Type</span></span>|<span data-ttu-id="5584e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5584e-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5584e-124">id</span><span class="sxs-lookup"><span data-stu-id="5584e-124">id</span></span>|<span data-ttu-id="5584e-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5584e-125">String</span></span>|<span data-ttu-id="5584e-126">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="5584e-126">The GUID for the object</span></span>|
|<span data-ttu-id="5584e-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="5584e-127">lastSyncDateTime</span></span>|<span data-ttu-id="5584e-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5584e-128">DateTimeOffset</span></span>|<span data-ttu-id="5584e-129">Data e hora da última sincronização de dados com o DDS Service.</span><span class="sxs-lookup"><span data-stu-id="5584e-129">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="5584e-130">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="5584e-130">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="5584e-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5584e-131">DateTimeOffset</span></span>|<span data-ttu-id="5584e-132">Data e hora da última sincronização de dados com o DDS Service.</span><span class="sxs-lookup"><span data-stu-id="5584e-132">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="5584e-133">syncStatus</span><span class="sxs-lookup"><span data-stu-id="5584e-133">syncStatus</span></span>|[<span data-ttu-id="5584e-134">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="5584e-134">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="5584e-135">Indica o status da sincronização com o serviço de DDS (sincronização de dados do dispositivo).</span><span class="sxs-lookup"><span data-stu-id="5584e-135">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="5584e-136">Os valores possíveis são: `unknown`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="5584e-136">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5584e-137">Relações</span><span class="sxs-lookup"><span data-stu-id="5584e-137">Relationships</span></span>
<span data-ttu-id="5584e-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5584e-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5584e-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5584e-139">JSON Representation</span></span>
<span data-ttu-id="5584e-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5584e-140">Here is a JSON representation of the resource.</span></span>
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




