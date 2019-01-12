---
title: tipo de recurso de windowsAutopilotSettings
description: O recurso de windowsAutopilotSettings representa uma conta do Windows piloto automático aos dados de sincronização com o serviço de sincronização de dados de dispositivo do Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4bf9a39d6a5078362c966edde38ec98deec037b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939550"
---
# <a name="windowsautopilotsettings-resource-type"></a><span data-ttu-id="83792-103">tipo de recurso de windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="83792-103">windowsAutopilotSettings resource type</span></span>

> <span data-ttu-id="83792-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="83792-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="83792-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="83792-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="83792-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="83792-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83792-107">O recurso de windowsAutopilotSettings representa uma conta do Windows piloto automático aos dados de sincronização com o serviço de sincronização de dados de dispositivo do Windows.</span><span class="sxs-lookup"><span data-stu-id="83792-107">The windowsAutopilotSettings resource represents a Windows Autopilot Account to sync data with Windows device data sync service.</span></span>
## <a name="methods"></a><span data-ttu-id="83792-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="83792-108">Methods</span></span>
|<span data-ttu-id="83792-109">Método</span><span class="sxs-lookup"><span data-stu-id="83792-109">Method</span></span>|<span data-ttu-id="83792-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="83792-110">Return Type</span></span>|<span data-ttu-id="83792-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="83792-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="83792-112">Obter windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="83792-112">Get windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-get.md)|[<span data-ttu-id="83792-113">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="83792-113">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="83792-114">Leia as propriedades e os relacionamentos do objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="83792-114">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="83792-115">Atualizar windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="83792-115">Update windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-update.md)|[<span data-ttu-id="83792-116">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="83792-116">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="83792-117">Atualize as propriedades de um objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="83792-117">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="83792-118">ação de sincronização</span><span class="sxs-lookup"><span data-stu-id="83792-118">sync action</span></span>](../api/intune-enrollment-windowsautopilotsettings-sync.md)|<span data-ttu-id="83792-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="83792-119">None</span></span>|<span data-ttu-id="83792-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="83792-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="83792-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83792-121">Properties</span></span>
|<span data-ttu-id="83792-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83792-122">Property</span></span>|<span data-ttu-id="83792-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="83792-123">Type</span></span>|<span data-ttu-id="83792-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="83792-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83792-125">id</span><span class="sxs-lookup"><span data-stu-id="83792-125">id</span></span>|<span data-ttu-id="83792-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83792-126">String</span></span>|<span data-ttu-id="83792-127">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="83792-127">The GUID for the object</span></span>|
|<span data-ttu-id="83792-128">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="83792-128">lastSyncDateTime</span></span>|<span data-ttu-id="83792-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83792-129">DateTimeOffset</span></span>|<span data-ttu-id="83792-130">Última dados sincronizar data hora com o serviço DDS.</span><span class="sxs-lookup"><span data-stu-id="83792-130">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="83792-131">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="83792-131">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="83792-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83792-132">DateTimeOffset</span></span>|<span data-ttu-id="83792-133">Última dados sincronizar data hora com o serviço DDS.</span><span class="sxs-lookup"><span data-stu-id="83792-133">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="83792-134">syncStatus</span><span class="sxs-lookup"><span data-stu-id="83792-134">syncStatus</span></span>|[<span data-ttu-id="83792-135">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="83792-135">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="83792-136">Indica o status da sincronização com o serviço de sincronização (DDS) de dados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="83792-136">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="83792-137">Os valores possíveis são: `unknown`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="83792-137">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83792-138">Relações</span><span class="sxs-lookup"><span data-stu-id="83792-138">Relationships</span></span>
<span data-ttu-id="83792-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="83792-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="83792-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83792-140">JSON Representation</span></span>
<span data-ttu-id="83792-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="83792-141">Here is a JSON representation of the resource.</span></span>
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





