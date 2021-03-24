---
title: Atualizar windowsAutopilotSettings
description: Atualize as propriedades de um objeto windowsAutopilotSettings.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bff766b56e9c625e2d22247db0612e5e8aeb95fc
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145849"
---
# <a name="update-windowsautopilotsettings"></a><span data-ttu-id="dccf8-103">Atualizar windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="dccf8-103">Update windowsAutopilotSettings</span></span>

<span data-ttu-id="dccf8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dccf8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dccf8-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dccf8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dccf8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dccf8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dccf8-107">Atualize as propriedades de um [objeto windowsAutopilotSettings.](../resources/intune-enrollment-windowsautopilotsettings.md)</span><span class="sxs-lookup"><span data-stu-id="dccf8-107">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dccf8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dccf8-108">Prerequisites</span></span>
<span data-ttu-id="dccf8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dccf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dccf8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dccf8-111">Permission type</span></span>|<span data-ttu-id="dccf8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dccf8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dccf8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dccf8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dccf8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dccf8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dccf8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dccf8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dccf8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dccf8-116">Not supported.</span></span>|
|<span data-ttu-id="dccf8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dccf8-117">Application</span></span>|<span data-ttu-id="dccf8-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dccf8-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dccf8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dccf8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotSettings
```

## <a name="request-headers"></a><span data-ttu-id="dccf8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dccf8-120">Request headers</span></span>
|<span data-ttu-id="dccf8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dccf8-121">Header</span></span>|<span data-ttu-id="dccf8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dccf8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dccf8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dccf8-123">Authorization</span></span>|<span data-ttu-id="dccf8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dccf8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dccf8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dccf8-125">Accept</span></span>|<span data-ttu-id="dccf8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dccf8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dccf8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dccf8-127">Request body</span></span>
<span data-ttu-id="dccf8-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsAutopilotSettings.](../resources/intune-enrollment-windowsautopilotsettings.md)</span><span class="sxs-lookup"><span data-stu-id="dccf8-128">In the request body, supply a JSON representation for the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

<span data-ttu-id="dccf8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span><span class="sxs-lookup"><span data-stu-id="dccf8-129">The following table shows the properties that are required when you create the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span></span>

|<span data-ttu-id="dccf8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dccf8-130">Property</span></span>|<span data-ttu-id="dccf8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="dccf8-131">Type</span></span>|<span data-ttu-id="dccf8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dccf8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dccf8-133">id</span><span class="sxs-lookup"><span data-stu-id="dccf8-133">id</span></span>|<span data-ttu-id="dccf8-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dccf8-134">String</span></span>|<span data-ttu-id="dccf8-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="dccf8-135">The GUID for the object</span></span>|
|<span data-ttu-id="dccf8-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="dccf8-136">lastSyncDateTime</span></span>|<span data-ttu-id="dccf8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dccf8-137">DateTimeOffset</span></span>|<span data-ttu-id="dccf8-138">Última data de sincronização de dados com o serviço DDS.</span><span class="sxs-lookup"><span data-stu-id="dccf8-138">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="dccf8-139">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="dccf8-139">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="dccf8-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dccf8-140">DateTimeOffset</span></span>|<span data-ttu-id="dccf8-141">Última data de sincronização de dados com o serviço DDS.</span><span class="sxs-lookup"><span data-stu-id="dccf8-141">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="dccf8-142">syncStatus</span><span class="sxs-lookup"><span data-stu-id="dccf8-142">syncStatus</span></span>|[<span data-ttu-id="dccf8-143">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="dccf8-143">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="dccf8-144">Indica o status da sincronização com o serviço de sincronização de dados de dispositivo (DDS).</span><span class="sxs-lookup"><span data-stu-id="dccf8-144">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="dccf8-145">Os valores possíveis são: `unknown`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="dccf8-145">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|



## <a name="response"></a><span data-ttu-id="dccf8-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="dccf8-146">Response</span></span>
<span data-ttu-id="dccf8-147">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dccf8-147">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dccf8-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dccf8-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="dccf8-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dccf8-149">Request</span></span>
<span data-ttu-id="dccf8-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dccf8-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dccf8-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="dccf8-151">Response</span></span>
<span data-ttu-id="dccf8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dccf8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




