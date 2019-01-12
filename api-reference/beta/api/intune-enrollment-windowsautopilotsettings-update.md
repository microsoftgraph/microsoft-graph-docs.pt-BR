---
title: Atualizar windowsAutopilotSettings
description: Atualize as propriedades de um objeto windowsAutopilotSettings.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3d07ce1b4416b671e8d18ebaa416d2b6e7ffe96e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945101"
---
# <a name="update-windowsautopilotsettings"></a><span data-ttu-id="04e4d-103">Atualizar windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="04e4d-103">Update windowsAutopilotSettings</span></span>

> <span data-ttu-id="04e4d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="04e4d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04e4d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="04e4d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04e4d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="04e4d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04e4d-107">Atualize as propriedades de um objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="04e4d-107">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="04e4d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="04e4d-108">Prerequisites</span></span>
<span data-ttu-id="04e4d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04e4d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04e4d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04e4d-111">Permission type</span></span>|<span data-ttu-id="04e4d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="04e4d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04e4d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04e4d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04e4d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04e4d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="04e4d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04e4d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04e4d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04e4d-116">Not supported.</span></span>|
|<span data-ttu-id="04e4d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04e4d-117">Application</span></span>|<span data-ttu-id="04e4d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04e4d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04e4d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04e4d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotSettings
```

## <a name="request-headers"></a><span data-ttu-id="04e4d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04e4d-120">Request headers</span></span>
|<span data-ttu-id="04e4d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="04e4d-121">Header</span></span>|<span data-ttu-id="04e4d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="04e4d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04e4d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="04e4d-123">Authorization</span></span>|<span data-ttu-id="04e4d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04e4d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04e4d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="04e4d-125">Accept</span></span>|<span data-ttu-id="04e4d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04e4d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04e4d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04e4d-127">Request body</span></span>
<span data-ttu-id="04e4d-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="04e4d-128">In the request body, supply a JSON representation for the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

<span data-ttu-id="04e4d-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span><span class="sxs-lookup"><span data-stu-id="04e4d-129">The following table shows the properties that are required when you create the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span></span>

|<span data-ttu-id="04e4d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04e4d-130">Property</span></span>|<span data-ttu-id="04e4d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="04e4d-131">Type</span></span>|<span data-ttu-id="04e4d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="04e4d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04e4d-133">id</span><span class="sxs-lookup"><span data-stu-id="04e4d-133">id</span></span>|<span data-ttu-id="04e4d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="04e4d-134">String</span></span>|<span data-ttu-id="04e4d-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="04e4d-135">The GUID for the object</span></span>|
|<span data-ttu-id="04e4d-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="04e4d-136">lastSyncDateTime</span></span>|<span data-ttu-id="04e4d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04e4d-137">DateTimeOffset</span></span>|<span data-ttu-id="04e4d-138">Última dados sincronizar data hora com o serviço DDS.</span><span class="sxs-lookup"><span data-stu-id="04e4d-138">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="04e4d-139">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="04e4d-139">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="04e4d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04e4d-140">DateTimeOffset</span></span>|<span data-ttu-id="04e4d-141">Última dados sincronizar data hora com o serviço DDS.</span><span class="sxs-lookup"><span data-stu-id="04e4d-141">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="04e4d-142">syncStatus</span><span class="sxs-lookup"><span data-stu-id="04e4d-142">syncStatus</span></span>|[<span data-ttu-id="04e4d-143">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="04e4d-143">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="04e4d-144">Indica o status da sincronização com o serviço de sincronização (DDS) de dados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="04e4d-144">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="04e4d-145">Os valores possíveis são: `unknown`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="04e4d-145">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|



## <a name="response"></a><span data-ttu-id="04e4d-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="04e4d-146">Response</span></span>
<span data-ttu-id="04e4d-147">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04e4d-147">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04e4d-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04e4d-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="04e4d-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04e4d-149">Request</span></span>
<span data-ttu-id="04e4d-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04e4d-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings
Content-type: application/json
Content-length: 167

{
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "lastManualSyncTriggerDateTime": "2016-12-31T23:57:54.7364636-08:00",
  "syncStatus": "inProgress"
}
```

### <a name="response"></a><span data-ttu-id="04e4d-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="04e4d-151">Response</span></span>
<span data-ttu-id="04e4d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04e4d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





