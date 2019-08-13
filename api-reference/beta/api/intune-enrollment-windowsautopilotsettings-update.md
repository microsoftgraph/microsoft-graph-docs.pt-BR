---
title: Atualizar windowsAutopilotSettings
description: Atualiza as propriedades de um objeto windowsAutopilotSettings.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a44dc502f1732f15c36de1bef83601fc4268f453
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36355910"
---
# <a name="update-windowsautopilotsettings"></a><span data-ttu-id="0fc2c-103">Atualizar windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="0fc2c-103">Update windowsAutopilotSettings</span></span>

> <span data-ttu-id="0fc2c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0fc2c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fc2c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0fc2c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fc2c-106">Atualiza as propriedades de um objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="0fc2c-106">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0fc2c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0fc2c-107">Prerequisites</span></span>
<span data-ttu-id="0fc2c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fc2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fc2c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0fc2c-110">Permission type</span></span>|<span data-ttu-id="0fc2c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0fc2c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fc2c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0fc2c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0fc2c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fc2c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0fc2c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0fc2c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fc2c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fc2c-115">Not supported.</span></span>|
|<span data-ttu-id="0fc2c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0fc2c-116">Application</span></span>|<span data-ttu-id="0fc2c-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fc2c-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fc2c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0fc2c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotSettings
```

## <a name="request-headers"></a><span data-ttu-id="0fc2c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0fc2c-119">Request headers</span></span>
|<span data-ttu-id="0fc2c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0fc2c-120">Header</span></span>|<span data-ttu-id="0fc2c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0fc2c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0fc2c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0fc2c-122">Authorization</span></span>|<span data-ttu-id="0fc2c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0fc2c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0fc2c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0fc2c-124">Accept</span></span>|<span data-ttu-id="0fc2c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0fc2c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fc2c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0fc2c-126">Request body</span></span>
<span data-ttu-id="0fc2c-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="0fc2c-127">In the request body, supply a JSON representation for the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

<span data-ttu-id="0fc2c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span><span class="sxs-lookup"><span data-stu-id="0fc2c-128">The following table shows the properties that are required when you create the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span></span>

|<span data-ttu-id="0fc2c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0fc2c-129">Property</span></span>|<span data-ttu-id="0fc2c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0fc2c-130">Type</span></span>|<span data-ttu-id="0fc2c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0fc2c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fc2c-132">id</span><span class="sxs-lookup"><span data-stu-id="0fc2c-132">id</span></span>|<span data-ttu-id="0fc2c-133">String</span><span class="sxs-lookup"><span data-stu-id="0fc2c-133">String</span></span>|<span data-ttu-id="0fc2c-134">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="0fc2c-134">The GUID for the object</span></span>|
|<span data-ttu-id="0fc2c-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0fc2c-135">lastSyncDateTime</span></span>|<span data-ttu-id="0fc2c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fc2c-136">DateTimeOffset</span></span>|<span data-ttu-id="0fc2c-137">Data e hora da última sincronização de dados com o DDS Service.</span><span class="sxs-lookup"><span data-stu-id="0fc2c-137">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="0fc2c-138">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="0fc2c-138">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="0fc2c-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fc2c-139">DateTimeOffset</span></span>|<span data-ttu-id="0fc2c-140">Data e hora da última sincronização de dados com o DDS Service.</span><span class="sxs-lookup"><span data-stu-id="0fc2c-140">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="0fc2c-141">syncStatus</span><span class="sxs-lookup"><span data-stu-id="0fc2c-141">syncStatus</span></span>|[<span data-ttu-id="0fc2c-142">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="0fc2c-142">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="0fc2c-143">Indica o status da sincronização com o serviço de DDS (sincronização de dados do dispositivo).</span><span class="sxs-lookup"><span data-stu-id="0fc2c-143">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="0fc2c-144">Os valores possíveis são: `unknown`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="0fc2c-144">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|



## <a name="response"></a><span data-ttu-id="0fc2c-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fc2c-145">Response</span></span>
<span data-ttu-id="0fc2c-146">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fc2c-146">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fc2c-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0fc2c-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="0fc2c-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fc2c-148">Request</span></span>
<span data-ttu-id="0fc2c-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fc2c-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0fc2c-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fc2c-150">Response</span></span>
<span data-ttu-id="0fc2c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0fc2c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






