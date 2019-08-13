---
title: tipo de recurso windowsAutopilotSettings
description: O recurso windowsAutopilotSettings representa uma conta do Windows AutoPilot para sincronizar dados com o serviço de sincronização de dados do dispositivo Windows.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f242bd184737daea34446d345eb39c4c2a9027f7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327679"
---
# <a name="windowsautopilotsettings-resource-type"></a><span data-ttu-id="b59de-103">tipo de recurso windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="b59de-103">windowsAutopilotSettings resource type</span></span>

> <span data-ttu-id="b59de-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b59de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b59de-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b59de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b59de-106">O recurso windowsAutopilotSettings representa uma conta do Windows AutoPilot para sincronizar dados com o serviço de sincronização de dados do dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="b59de-106">The windowsAutopilotSettings resource represents a Windows Autopilot Account to sync data with Windows device data sync service.</span></span>

## <a name="methods"></a><span data-ttu-id="b59de-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="b59de-107">Methods</span></span>
|<span data-ttu-id="b59de-108">Método</span><span class="sxs-lookup"><span data-stu-id="b59de-108">Method</span></span>|<span data-ttu-id="b59de-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b59de-109">Return Type</span></span>|<span data-ttu-id="b59de-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b59de-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b59de-111">Obter windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="b59de-111">Get windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-get.md)|[<span data-ttu-id="b59de-112">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="b59de-112">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="b59de-113">Leia as propriedades e as relações do objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="b59de-113">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="b59de-114">Atualizar windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="b59de-114">Update windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-update.md)|[<span data-ttu-id="b59de-115">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="b59de-115">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="b59de-116">Atualiza as propriedades de um objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="b59de-116">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="b59de-117">ação de sincronização</span><span class="sxs-lookup"><span data-stu-id="b59de-117">sync action</span></span>](../api/intune-enrollment-windowsautopilotsettings-sync.md)|<span data-ttu-id="b59de-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b59de-118">None</span></span>|<span data-ttu-id="b59de-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b59de-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="b59de-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b59de-120">Properties</span></span>
|<span data-ttu-id="b59de-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b59de-121">Property</span></span>|<span data-ttu-id="b59de-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="b59de-122">Type</span></span>|<span data-ttu-id="b59de-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b59de-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b59de-124">id</span><span class="sxs-lookup"><span data-stu-id="b59de-124">id</span></span>|<span data-ttu-id="b59de-125">String</span><span class="sxs-lookup"><span data-stu-id="b59de-125">String</span></span>|<span data-ttu-id="b59de-126">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="b59de-126">The GUID for the object</span></span>|
|<span data-ttu-id="b59de-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b59de-127">lastSyncDateTime</span></span>|<span data-ttu-id="b59de-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b59de-128">DateTimeOffset</span></span>|<span data-ttu-id="b59de-129">Data e hora da última sincronização de dados com o DDS Service.</span><span class="sxs-lookup"><span data-stu-id="b59de-129">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="b59de-130">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="b59de-130">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="b59de-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b59de-131">DateTimeOffset</span></span>|<span data-ttu-id="b59de-132">Data e hora da última sincronização de dados com o DDS Service.</span><span class="sxs-lookup"><span data-stu-id="b59de-132">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="b59de-133">syncStatus</span><span class="sxs-lookup"><span data-stu-id="b59de-133">syncStatus</span></span>|[<span data-ttu-id="b59de-134">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="b59de-134">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="b59de-135">Indica o status da sincronização com o serviço de DDS (sincronização de dados do dispositivo).</span><span class="sxs-lookup"><span data-stu-id="b59de-135">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="b59de-136">Os valores possíveis são: `unknown`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="b59de-136">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b59de-137">Relações</span><span class="sxs-lookup"><span data-stu-id="b59de-137">Relationships</span></span>
<span data-ttu-id="b59de-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b59de-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b59de-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b59de-139">JSON Representation</span></span>
<span data-ttu-id="b59de-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b59de-140">Here is a JSON representation of the resource.</span></span>
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



