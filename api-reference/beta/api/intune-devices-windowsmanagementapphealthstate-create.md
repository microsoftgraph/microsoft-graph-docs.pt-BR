---
title: Criar windowsManagementAppHealthState
description: Crie um novo objeto de windowsManagementAppHealthState.
ms.openlocfilehash: e815a86001e75e2350e0ea1b5bb73a8dfd87f58a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035625"
---
# <a name="create-windowsmanagementapphealthstate"></a><span data-ttu-id="60e5a-103">Criar windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="60e5a-103">Create windowsManagementAppHealthState</span></span>

> <span data-ttu-id="60e5a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="60e5a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60e5a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="60e5a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="60e5a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="60e5a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60e5a-107">Crie um novo objeto de [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="60e5a-107">Create a new [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="60e5a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="60e5a-108">Prerequisites</span></span>
<span data-ttu-id="60e5a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60e5a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60e5a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60e5a-111">Permission type</span></span>|<span data-ttu-id="60e5a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="60e5a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60e5a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60e5a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="60e5a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60e5a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="60e5a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60e5a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60e5a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60e5a-116">Not supported.</span></span>|
|<span data-ttu-id="60e5a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60e5a-117">Application</span></span>|<span data-ttu-id="60e5a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60e5a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60e5a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60e5a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsManagementApp/healthStates
```

## <a name="request-headers"></a><span data-ttu-id="60e5a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60e5a-120">Request headers</span></span>
|<span data-ttu-id="60e5a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="60e5a-121">Header</span></span>|<span data-ttu-id="60e5a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="60e5a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60e5a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="60e5a-123">Authorization</span></span>|<span data-ttu-id="60e5a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60e5a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60e5a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="60e5a-125">Accept</span></span>|<span data-ttu-id="60e5a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="60e5a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60e5a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60e5a-127">Request body</span></span>
<span data-ttu-id="60e5a-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsManagementAppHealthState.</span><span class="sxs-lookup"><span data-stu-id="60e5a-128">In the request body, supply a JSON representation for the windowsManagementAppHealthState object.</span></span>

<span data-ttu-id="60e5a-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsManagementAppHealthState.</span><span class="sxs-lookup"><span data-stu-id="60e5a-129">The following table shows the properties that are required when you create the windowsManagementAppHealthState.</span></span>

|<span data-ttu-id="60e5a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60e5a-130">Property</span></span>|<span data-ttu-id="60e5a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="60e5a-131">Type</span></span>|<span data-ttu-id="60e5a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="60e5a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60e5a-133">id</span><span class="sxs-lookup"><span data-stu-id="60e5a-133">id</span></span>|<span data-ttu-id="60e5a-134">String</span><span class="sxs-lookup"><span data-stu-id="60e5a-134">String</span></span>|<span data-ttu-id="60e5a-135">Identificador exclusivo para o estado de integridade de aplicativo de gerenciamento do Windows</span><span class="sxs-lookup"><span data-stu-id="60e5a-135">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="60e5a-136">healthState</span><span class="sxs-lookup"><span data-stu-id="60e5a-136">healthState</span></span>|[<span data-ttu-id="60e5a-137">healthState</span><span class="sxs-lookup"><span data-stu-id="60e5a-137">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="60e5a-138">Estado de integridade do aplicativo do gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="60e5a-138">Windows management app health state.</span></span> <span data-ttu-id="60e5a-139">Os valores possíveis são: `unknown`, `healthy`, `unhealthy`.</span><span class="sxs-lookup"><span data-stu-id="60e5a-139">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="60e5a-140">installedVersion</span><span class="sxs-lookup"><span data-stu-id="60e5a-140">installedVersion</span></span>|<span data-ttu-id="60e5a-141">String</span><span class="sxs-lookup"><span data-stu-id="60e5a-141">String</span></span>|<span data-ttu-id="60e5a-142">Versão instalada do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="60e5a-142">Windows management app installed version.</span></span>|
|<span data-ttu-id="60e5a-143">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="60e5a-143">lastCheckInDateTime</span></span>|<span data-ttu-id="60e5a-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60e5a-144">DateTimeOffset</span></span>|<span data-ttu-id="60e5a-145">Aplicativo de gerenciamento do Windows hora do último check-in.</span><span class="sxs-lookup"><span data-stu-id="60e5a-145">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="60e5a-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="60e5a-146">deviceName</span></span>|<span data-ttu-id="60e5a-147">String</span><span class="sxs-lookup"><span data-stu-id="60e5a-147">String</span></span>|<span data-ttu-id="60e5a-148">Nome do dispositivo no qual o Windows o aplicativo de gerenciamento está instalado.</span><span class="sxs-lookup"><span data-stu-id="60e5a-148">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="60e5a-149">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="60e5a-149">deviceOSVersion</span></span>|<span data-ttu-id="60e5a-150">String</span><span class="sxs-lookup"><span data-stu-id="60e5a-150">String</span></span>|<span data-ttu-id="60e5a-151">Versão do sistema operacional do Windows 10 do dispositivo no qual o Windows o aplicativo de gerenciamento está instalado.</span><span class="sxs-lookup"><span data-stu-id="60e5a-151">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="60e5a-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="60e5a-152">Response</span></span>
<span data-ttu-id="60e5a-153">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60e5a-153">If successful, this method returns a `201 Created` response code and a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60e5a-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60e5a-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="60e5a-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60e5a-155">Request</span></span>
<span data-ttu-id="60e5a-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60e5a-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates
Content-type: application/json
Content-length: 300

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "healthState": "healthy",
  "installedVersion": "Installed Version value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
  "deviceName": "Device Name value",
  "deviceOSVersion": "Device OSVersion value"
}
```

### <a name="response"></a><span data-ttu-id="60e5a-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="60e5a-157">Response</span></span>
<span data-ttu-id="60e5a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60e5a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 349

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "id": "5c7e50fb-50fb-5c7e-fb50-7e5cfb507e5c",
  "healthState": "healthy",
  "installedVersion": "Installed Version value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
  "deviceName": "Device Name value",
  "deviceOSVersion": "Device OSVersion value"
}
```





