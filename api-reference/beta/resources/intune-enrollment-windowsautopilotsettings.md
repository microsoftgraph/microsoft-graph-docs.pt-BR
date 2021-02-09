---
title: Tipo de recurso windowsAutopilotSettings
description: O recurso windowsAutopilotSettings representa uma conta do Windows Autopilot para sincronizar dados com o serviço de sincronização de dados do dispositivo Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2e49191d204a040327c510606c6ca8186644beb7
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159525"
---
# <a name="windowsautopilotsettings-resource-type"></a><span data-ttu-id="a2e3b-103">Tipo de recurso windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="a2e3b-103">windowsAutopilotSettings resource type</span></span>

<span data-ttu-id="a2e3b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2e3b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2e3b-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a2e3b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2e3b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a2e3b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2e3b-107">O recurso windowsAutopilotSettings representa uma conta do Windows Autopilot para sincronizar dados com o serviço de sincronização de dados do dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="a2e3b-107">The windowsAutopilotSettings resource represents a Windows Autopilot Account to sync data with Windows device data sync service.</span></span>

## <a name="methods"></a><span data-ttu-id="a2e3b-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="a2e3b-108">Methods</span></span>
|<span data-ttu-id="a2e3b-109">Método</span><span class="sxs-lookup"><span data-stu-id="a2e3b-109">Method</span></span>|<span data-ttu-id="a2e3b-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a2e3b-110">Return Type</span></span>|<span data-ttu-id="a2e3b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2e3b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a2e3b-112">Obter windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="a2e3b-112">Get windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-get.md)|[<span data-ttu-id="a2e3b-113">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="a2e3b-113">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="a2e3b-114">Leia as propriedades e as relações do [objeto windowsAutopilotSettings.](../resources/intune-enrollment-windowsautopilotsettings.md)</span><span class="sxs-lookup"><span data-stu-id="a2e3b-114">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="a2e3b-115">Atualizar windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="a2e3b-115">Update windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-update.md)|[<span data-ttu-id="a2e3b-116">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="a2e3b-116">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="a2e3b-117">Atualizar as propriedades de um [objeto windowsAutopilotSettings.](../resources/intune-enrollment-windowsautopilotsettings.md)</span><span class="sxs-lookup"><span data-stu-id="a2e3b-117">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="a2e3b-118">ação de sincronização</span><span class="sxs-lookup"><span data-stu-id="a2e3b-118">sync action</span></span>](../api/intune-enrollment-windowsautopilotsettings-sync.md)|<span data-ttu-id="a2e3b-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a2e3b-119">None</span></span>|<span data-ttu-id="a2e3b-120">Inicia uma sincronização de todos os dispositivos registrados do AutoPilot na Loja para Empresas e em outros portais.</span><span class="sxs-lookup"><span data-stu-id="a2e3b-120">Initiates a sync of all AutoPilot registered devices from Store for Business and other portals.</span></span> <span data-ttu-id="a2e3b-121">Se a sincronização for bem-sucedida, essa ação retornará um código de resposta 204 No Content.</span><span class="sxs-lookup"><span data-stu-id="a2e3b-121">If the sync successful, this action returns a 204 No Content response code.</span></span> <span data-ttu-id="a2e3b-122">Se uma sincronização já estiver em andamento, a ação retornará um código de resposta de conflito 409.</span><span class="sxs-lookup"><span data-stu-id="a2e3b-122">If a sync is already in progress, the action returns a 409 Conflict response code.</span></span>  <span data-ttu-id="a2e3b-123">Se essa ação de sincronização for chamada dentro de 10 minutos após a sincronização anterior, a ação retornará um código de resposta 429 Solicitações Demais.</span><span class="sxs-lookup"><span data-stu-id="a2e3b-123">If this sync action is called within 10 minutes of the previous sync, the action returns a 429 Too Many Requests response code.</span></span>|

## <a name="properties"></a><span data-ttu-id="a2e3b-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2e3b-124">Properties</span></span>
|<span data-ttu-id="a2e3b-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2e3b-125">Property</span></span>|<span data-ttu-id="a2e3b-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2e3b-126">Type</span></span>|<span data-ttu-id="a2e3b-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2e3b-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2e3b-128">id</span><span class="sxs-lookup"><span data-stu-id="a2e3b-128">id</span></span>|<span data-ttu-id="a2e3b-129">String</span><span class="sxs-lookup"><span data-stu-id="a2e3b-129">String</span></span>|<span data-ttu-id="a2e3b-130">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="a2e3b-130">The GUID for the object</span></span>|
|<span data-ttu-id="a2e3b-131">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a2e3b-131">lastSyncDateTime</span></span>|<span data-ttu-id="a2e3b-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2e3b-132">DateTimeOffset</span></span>|<span data-ttu-id="a2e3b-133">Hora da última sincronização de dados com o serviço DDS.</span><span class="sxs-lookup"><span data-stu-id="a2e3b-133">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="a2e3b-134">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="a2e3b-134">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="a2e3b-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2e3b-135">DateTimeOffset</span></span>|<span data-ttu-id="a2e3b-136">Hora da última sincronização de dados com o serviço DDS.</span><span class="sxs-lookup"><span data-stu-id="a2e3b-136">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="a2e3b-137">syncStatus</span><span class="sxs-lookup"><span data-stu-id="a2e3b-137">syncStatus</span></span>|[<span data-ttu-id="a2e3b-138">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="a2e3b-138">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="a2e3b-139">Indica o status de sincronização com o serviço de sincronização de dados do dispositivo (DDS).</span><span class="sxs-lookup"><span data-stu-id="a2e3b-139">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="a2e3b-140">Os valores possíveis são: `unknown`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="a2e3b-140">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2e3b-141">Relações</span><span class="sxs-lookup"><span data-stu-id="a2e3b-141">Relationships</span></span>
<span data-ttu-id="a2e3b-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a2e3b-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2e3b-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2e3b-143">JSON Representation</span></span>
<span data-ttu-id="a2e3b-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a2e3b-144">Here is a JSON representation of the resource.</span></span>
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




