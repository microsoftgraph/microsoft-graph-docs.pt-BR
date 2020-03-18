---
title: Atualizar windowsAutopilotSettings
description: Atualiza as propriedades de um objeto windowsAutopilotSettings.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e81e2b83e6969f9752bb2f6170df9210ea869039
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804958"
---
# <a name="update-windowsautopilotsettings"></a><span data-ttu-id="6a711-103">Atualizar windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="6a711-103">Update windowsAutopilotSettings</span></span>

> <span data-ttu-id="6a711-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6a711-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a711-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a711-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a711-106">Atualiza as propriedades de um objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="6a711-106">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a711-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6a711-107">Prerequisites</span></span>
<span data-ttu-id="6a711-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a711-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a711-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a711-110">Permission type</span></span>|<span data-ttu-id="6a711-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6a711-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a711-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a711-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a711-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a711-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6a711-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a711-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a711-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a711-115">Not supported.</span></span>|
|<span data-ttu-id="6a711-116">Application</span><span class="sxs-lookup"><span data-stu-id="6a711-116">Application</span></span>|<span data-ttu-id="6a711-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a711-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a711-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a711-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotSettings
```

## <a name="request-headers"></a><span data-ttu-id="6a711-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a711-119">Request headers</span></span>
|<span data-ttu-id="6a711-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a711-120">Header</span></span>|<span data-ttu-id="6a711-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6a711-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a711-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a711-122">Authorization</span></span>|<span data-ttu-id="6a711-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a711-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a711-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6a711-124">Accept</span></span>|<span data-ttu-id="6a711-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a711-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a711-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a711-126">Request body</span></span>
<span data-ttu-id="6a711-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="6a711-127">In the request body, supply a JSON representation for the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

<span data-ttu-id="6a711-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span><span class="sxs-lookup"><span data-stu-id="6a711-128">The following table shows the properties that are required when you create the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span></span>

|<span data-ttu-id="6a711-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a711-129">Property</span></span>|<span data-ttu-id="6a711-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a711-130">Type</span></span>|<span data-ttu-id="6a711-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a711-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a711-132">id</span><span class="sxs-lookup"><span data-stu-id="6a711-132">id</span></span>|<span data-ttu-id="6a711-133">String</span><span class="sxs-lookup"><span data-stu-id="6a711-133">String</span></span>|<span data-ttu-id="6a711-134">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="6a711-134">The GUID for the object</span></span>|
|<span data-ttu-id="6a711-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6a711-135">lastSyncDateTime</span></span>|<span data-ttu-id="6a711-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a711-136">DateTimeOffset</span></span>|<span data-ttu-id="6a711-137">Data e hora da última sincronização de dados com o DDS Service.</span><span class="sxs-lookup"><span data-stu-id="6a711-137">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="6a711-138">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="6a711-138">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="6a711-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a711-139">DateTimeOffset</span></span>|<span data-ttu-id="6a711-140">Data e hora da última sincronização de dados com o DDS Service.</span><span class="sxs-lookup"><span data-stu-id="6a711-140">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="6a711-141">syncStatus</span><span class="sxs-lookup"><span data-stu-id="6a711-141">syncStatus</span></span>|[<span data-ttu-id="6a711-142">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="6a711-142">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="6a711-143">Indica o status da sincronização com o serviço de DDS (sincronização de dados do dispositivo).</span><span class="sxs-lookup"><span data-stu-id="6a711-143">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="6a711-144">Os valores possíveis são: `unknown`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="6a711-144">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|



## <a name="response"></a><span data-ttu-id="6a711-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a711-145">Response</span></span>
<span data-ttu-id="6a711-146">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a711-146">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a711-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a711-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a711-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a711-148">Request</span></span>
<span data-ttu-id="6a711-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a711-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6a711-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a711-150">Response</span></span>
<span data-ttu-id="6a711-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a711-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




