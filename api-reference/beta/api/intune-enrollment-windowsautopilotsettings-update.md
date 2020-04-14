---
title: Atualizar windowsAutopilotSettings
description: Atualiza as propriedades de um objeto windowsAutopilotSettings.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 29ec5af7b5b900bcd6ec8f976c665782d371c165
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452279"
---
# <a name="update-windowsautopilotsettings"></a><span data-ttu-id="32b40-103">Atualizar windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="32b40-103">Update windowsAutopilotSettings</span></span>

<span data-ttu-id="32b40-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32b40-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32b40-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="32b40-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32b40-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="32b40-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32b40-107">Atualiza as propriedades de um objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="32b40-107">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32b40-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="32b40-108">Prerequisites</span></span>
<span data-ttu-id="32b40-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32b40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32b40-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32b40-111">Permission type</span></span>|<span data-ttu-id="32b40-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="32b40-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32b40-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32b40-113">Delegated (work or school account)</span></span>|<span data-ttu-id="32b40-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32b40-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="32b40-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32b40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32b40-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32b40-116">Not supported.</span></span>|
|<span data-ttu-id="32b40-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32b40-117">Application</span></span>|<span data-ttu-id="32b40-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32b40-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32b40-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32b40-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotSettings
```

## <a name="request-headers"></a><span data-ttu-id="32b40-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32b40-120">Request headers</span></span>
|<span data-ttu-id="32b40-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="32b40-121">Header</span></span>|<span data-ttu-id="32b40-122">Valor</span><span class="sxs-lookup"><span data-stu-id="32b40-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32b40-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="32b40-123">Authorization</span></span>|<span data-ttu-id="32b40-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32b40-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32b40-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="32b40-125">Accept</span></span>|<span data-ttu-id="32b40-126">application/json</span><span class="sxs-lookup"><span data-stu-id="32b40-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32b40-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32b40-127">Request body</span></span>
<span data-ttu-id="32b40-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="32b40-128">In the request body, supply a JSON representation for the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

<span data-ttu-id="32b40-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span><span class="sxs-lookup"><span data-stu-id="32b40-129">The following table shows the properties that are required when you create the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span></span>

|<span data-ttu-id="32b40-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32b40-130">Property</span></span>|<span data-ttu-id="32b40-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="32b40-131">Type</span></span>|<span data-ttu-id="32b40-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="32b40-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32b40-133">id</span><span class="sxs-lookup"><span data-stu-id="32b40-133">id</span></span>|<span data-ttu-id="32b40-134">String</span><span class="sxs-lookup"><span data-stu-id="32b40-134">String</span></span>|<span data-ttu-id="32b40-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="32b40-135">The GUID for the object</span></span>|
|<span data-ttu-id="32b40-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="32b40-136">lastSyncDateTime</span></span>|<span data-ttu-id="32b40-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32b40-137">DateTimeOffset</span></span>|<span data-ttu-id="32b40-138">Data e hora da última sincronização de dados com o DDS Service.</span><span class="sxs-lookup"><span data-stu-id="32b40-138">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="32b40-139">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="32b40-139">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="32b40-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32b40-140">DateTimeOffset</span></span>|<span data-ttu-id="32b40-141">Data e hora da última sincronização de dados com o DDS Service.</span><span class="sxs-lookup"><span data-stu-id="32b40-141">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="32b40-142">syncStatus</span><span class="sxs-lookup"><span data-stu-id="32b40-142">syncStatus</span></span>|[<span data-ttu-id="32b40-143">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="32b40-143">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="32b40-144">Indica o status da sincronização com o serviço de DDS (sincronização de dados do dispositivo).</span><span class="sxs-lookup"><span data-stu-id="32b40-144">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="32b40-145">Os valores possíveis são: `unknown`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="32b40-145">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|



## <a name="response"></a><span data-ttu-id="32b40-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="32b40-146">Response</span></span>
<span data-ttu-id="32b40-147">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32b40-147">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32b40-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32b40-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="32b40-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32b40-149">Request</span></span>
<span data-ttu-id="32b40-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="32b40-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings
Content-type: application/json
Content-length: 230

{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "lastManualSyncTriggerDateTime": "2016-12-31T23:57:54.7364636-08:00",
  "syncStatus": "inProgress"
}
```

### <a name="response"></a><span data-ttu-id="32b40-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="32b40-151">Response</span></span>
<span data-ttu-id="32b40-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32b40-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "id": "08c16770-6770-08c1-7067-c1087067c108",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "lastManualSyncTriggerDateTime": "2016-12-31T23:57:54.7364636-08:00",
  "syncStatus": "inProgress"
}
```



