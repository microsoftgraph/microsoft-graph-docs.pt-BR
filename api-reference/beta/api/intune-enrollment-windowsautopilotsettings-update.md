---
title: Atualizar windowsAutopilotSettings
description: Atualiza as propriedades de um objeto windowsAutopilotSettings.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 53560e607bd3cdfe9cc56268d68fa09d9f95ac44
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49212346"
---
# <a name="update-windowsautopilotsettings"></a><span data-ttu-id="d94d3-103">Atualizar windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="d94d3-103">Update windowsAutopilotSettings</span></span>

<span data-ttu-id="d94d3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d94d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d94d3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d94d3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d94d3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d94d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d94d3-107">Atualiza as propriedades de um objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="d94d3-107">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d94d3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d94d3-108">Prerequisites</span></span>
<span data-ttu-id="d94d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d94d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d94d3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d94d3-111">Permission type</span></span>|<span data-ttu-id="d94d3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d94d3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d94d3-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d94d3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d94d3-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d94d3-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d94d3-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d94d3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d94d3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d94d3-116">Not supported.</span></span>|
|<span data-ttu-id="d94d3-117">Application</span><span class="sxs-lookup"><span data-stu-id="d94d3-117">Application</span></span>|<span data-ttu-id="d94d3-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d94d3-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d94d3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d94d3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotSettings
```

## <a name="request-headers"></a><span data-ttu-id="d94d3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d94d3-120">Request headers</span></span>
|<span data-ttu-id="d94d3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d94d3-121">Header</span></span>|<span data-ttu-id="d94d3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d94d3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d94d3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d94d3-123">Authorization</span></span>|<span data-ttu-id="d94d3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d94d3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d94d3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d94d3-125">Accept</span></span>|<span data-ttu-id="d94d3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d94d3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d94d3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d94d3-127">Request body</span></span>
<span data-ttu-id="d94d3-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="d94d3-128">In the request body, supply a JSON representation for the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

<span data-ttu-id="d94d3-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span><span class="sxs-lookup"><span data-stu-id="d94d3-129">The following table shows the properties that are required when you create the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span></span>

|<span data-ttu-id="d94d3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d94d3-130">Property</span></span>|<span data-ttu-id="d94d3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d94d3-131">Type</span></span>|<span data-ttu-id="d94d3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d94d3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d94d3-133">id</span><span class="sxs-lookup"><span data-stu-id="d94d3-133">id</span></span>|<span data-ttu-id="d94d3-134">String</span><span class="sxs-lookup"><span data-stu-id="d94d3-134">String</span></span>|<span data-ttu-id="d94d3-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="d94d3-135">The GUID for the object</span></span>|
|<span data-ttu-id="d94d3-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d94d3-136">lastSyncDateTime</span></span>|<span data-ttu-id="d94d3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d94d3-137">DateTimeOffset</span></span>|<span data-ttu-id="d94d3-138">Data e hora da última sincronização de dados com o DDS Service.</span><span class="sxs-lookup"><span data-stu-id="d94d3-138">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="d94d3-139">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="d94d3-139">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="d94d3-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d94d3-140">DateTimeOffset</span></span>|<span data-ttu-id="d94d3-141">Data e hora da última sincronização de dados com o DDS Service.</span><span class="sxs-lookup"><span data-stu-id="d94d3-141">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="d94d3-142">syncStatus</span><span class="sxs-lookup"><span data-stu-id="d94d3-142">syncStatus</span></span>|[<span data-ttu-id="d94d3-143">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="d94d3-143">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="d94d3-144">Indica o status da sincronização com o serviço de DDS (sincronização de dados do dispositivo).</span><span class="sxs-lookup"><span data-stu-id="d94d3-144">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="d94d3-145">Os valores possíveis são: `unknown`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="d94d3-145">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|



## <a name="response"></a><span data-ttu-id="d94d3-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="d94d3-146">Response</span></span>
<span data-ttu-id="d94d3-147">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d94d3-147">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d94d3-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d94d3-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="d94d3-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d94d3-149">Request</span></span>
<span data-ttu-id="d94d3-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d94d3-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d94d3-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="d94d3-151">Response</span></span>
<span data-ttu-id="d94d3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d94d3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




