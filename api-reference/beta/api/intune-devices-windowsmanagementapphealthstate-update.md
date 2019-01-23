---
title: Atualizar windowsManagementAppHealthState
description: Atualize as propriedades de um objeto windowsManagementAppHealthState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: de395bdeba104ea3c5c30b8f33e8670a5f2e5480
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423150"
---
# <a name="update-windowsmanagementapphealthstate"></a><span data-ttu-id="fe832-103">Atualizar windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="fe832-103">Update windowsManagementAppHealthState</span></span>

> <span data-ttu-id="fe832-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="fe832-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fe832-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fe832-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe832-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="fe832-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe832-107">Atualize as propriedades de um objeto [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="fe832-107">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe832-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fe832-108">Prerequisites</span></span>
<span data-ttu-id="fe832-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fe832-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fe832-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe832-111">Permission type</span></span>|<span data-ttu-id="fe832-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fe832-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe832-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe832-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe832-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe832-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fe832-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe832-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe832-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe832-116">Not supported.</span></span>|
|<span data-ttu-id="fe832-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe832-117">Application</span></span>|<span data-ttu-id="fe832-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe832-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe832-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe832-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

## <a name="request-headers"></a><span data-ttu-id="fe832-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe832-120">Request headers</span></span>
|<span data-ttu-id="fe832-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fe832-121">Header</span></span>|<span data-ttu-id="fe832-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fe832-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe832-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe832-123">Authorization</span></span>|<span data-ttu-id="fe832-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe832-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe832-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fe832-125">Accept</span></span>|<span data-ttu-id="fe832-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe832-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe832-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe832-127">Request body</span></span>
<span data-ttu-id="fe832-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="fe832-128">In the request body, supply a JSON representation for the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

<span data-ttu-id="fe832-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span><span class="sxs-lookup"><span data-stu-id="fe832-129">The following table shows the properties that are required when you create the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>

|<span data-ttu-id="fe832-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe832-130">Property</span></span>|<span data-ttu-id="fe832-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe832-131">Type</span></span>|<span data-ttu-id="fe832-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe832-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe832-133">id</span><span class="sxs-lookup"><span data-stu-id="fe832-133">id</span></span>|<span data-ttu-id="fe832-134">String</span><span class="sxs-lookup"><span data-stu-id="fe832-134">String</span></span>|<span data-ttu-id="fe832-135">Identificador exclusivo para o estado de integridade de aplicativo de gerenciamento do Windows</span><span class="sxs-lookup"><span data-stu-id="fe832-135">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="fe832-136">healthState</span><span class="sxs-lookup"><span data-stu-id="fe832-136">healthState</span></span>|[<span data-ttu-id="fe832-137">healthState</span><span class="sxs-lookup"><span data-stu-id="fe832-137">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="fe832-138">Estado de integridade do aplicativo do gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="fe832-138">Windows management app health state.</span></span> <span data-ttu-id="fe832-139">Os valores possíveis são: `unknown`, `healthy`, `unhealthy`.</span><span class="sxs-lookup"><span data-stu-id="fe832-139">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="fe832-140">installedVersion</span><span class="sxs-lookup"><span data-stu-id="fe832-140">installedVersion</span></span>|<span data-ttu-id="fe832-141">String</span><span class="sxs-lookup"><span data-stu-id="fe832-141">String</span></span>|<span data-ttu-id="fe832-142">Versão instalada do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="fe832-142">Windows management app installed version.</span></span>|
|<span data-ttu-id="fe832-143">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="fe832-143">lastCheckInDateTime</span></span>|<span data-ttu-id="fe832-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe832-144">DateTimeOffset</span></span>|<span data-ttu-id="fe832-145">Aplicativo de gerenciamento do Windows hora do último check-in.</span><span class="sxs-lookup"><span data-stu-id="fe832-145">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="fe832-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="fe832-146">deviceName</span></span>|<span data-ttu-id="fe832-147">String</span><span class="sxs-lookup"><span data-stu-id="fe832-147">String</span></span>|<span data-ttu-id="fe832-148">Nome do dispositivo no qual o Windows o aplicativo de gerenciamento está instalado.</span><span class="sxs-lookup"><span data-stu-id="fe832-148">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="fe832-149">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="fe832-149">deviceOSVersion</span></span>|<span data-ttu-id="fe832-150">String</span><span class="sxs-lookup"><span data-stu-id="fe832-150">String</span></span>|<span data-ttu-id="fe832-151">Versão do sistema operacional do Windows 10 do dispositivo no qual o Windows o aplicativo de gerenciamento está instalado.</span><span class="sxs-lookup"><span data-stu-id="fe832-151">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="fe832-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe832-152">Response</span></span>
<span data-ttu-id="fe832-153">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe832-153">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe832-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe832-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe832-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe832-155">Request</span></span>
<span data-ttu-id="fe832-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe832-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
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

### <a name="response"></a><span data-ttu-id="fe832-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe832-157">Response</span></span>
<span data-ttu-id="fe832-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fe832-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




