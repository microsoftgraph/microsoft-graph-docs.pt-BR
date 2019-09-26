---
title: Atualizar deviceInstallState
description: Atualizar as propriedades de um objeto deviceInstallState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5d04cfeeb552f6e41990d97d17aa691ef8dbddac
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37171327"
---
# <a name="update-deviceinstallstate"></a><span data-ttu-id="83c91-103">Atualizar deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="83c91-103">Update deviceInstallState</span></span>

> <span data-ttu-id="83c91-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="83c91-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83c91-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="83c91-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83c91-106">Atualizar as propriedades de um objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="83c91-106">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83c91-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="83c91-107">Prerequisites</span></span>
<span data-ttu-id="83c91-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83c91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83c91-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83c91-110">Permission type</span></span>|<span data-ttu-id="83c91-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="83c91-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83c91-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83c91-112">Delegated (work or school account)</span></span>|<span data-ttu-id="83c91-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83c91-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="83c91-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83c91-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83c91-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83c91-115">Not supported.</span></span>|
|<span data-ttu-id="83c91-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83c91-116">Application</span></span>|<span data-ttu-id="83c91-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83c91-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="83c91-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83c91-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="83c91-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83c91-119">Request headers</span></span>
|<span data-ttu-id="83c91-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="83c91-120">Header</span></span>|<span data-ttu-id="83c91-121">Valor</span><span class="sxs-lookup"><span data-stu-id="83c91-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83c91-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="83c91-122">Authorization</span></span>|<span data-ttu-id="83c91-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83c91-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83c91-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="83c91-124">Accept</span></span>|<span data-ttu-id="83c91-125">application/json</span><span class="sxs-lookup"><span data-stu-id="83c91-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83c91-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83c91-126">Request body</span></span>
<span data-ttu-id="83c91-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="83c91-127">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

<span data-ttu-id="83c91-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="83c91-128">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

|<span data-ttu-id="83c91-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83c91-129">Property</span></span>|<span data-ttu-id="83c91-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="83c91-130">Type</span></span>|<span data-ttu-id="83c91-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="83c91-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83c91-132">id</span><span class="sxs-lookup"><span data-stu-id="83c91-132">id</span></span>|<span data-ttu-id="83c91-133">String</span><span class="sxs-lookup"><span data-stu-id="83c91-133">String</span></span>|<span data-ttu-id="83c91-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="83c91-134">Key of the entity.</span></span>|
|<span data-ttu-id="83c91-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="83c91-135">deviceName</span></span>|<span data-ttu-id="83c91-136">String</span><span class="sxs-lookup"><span data-stu-id="83c91-136">String</span></span>|<span data-ttu-id="83c91-137">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="83c91-137">Device name.</span></span>|
|<span data-ttu-id="83c91-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="83c91-138">deviceId</span></span>|<span data-ttu-id="83c91-139">String</span><span class="sxs-lookup"><span data-stu-id="83c91-139">String</span></span>|<span data-ttu-id="83c91-140">ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="83c91-140">Device Id.</span></span>|
|<span data-ttu-id="83c91-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="83c91-141">lastSyncDateTime</span></span>|<span data-ttu-id="83c91-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83c91-142">DateTimeOffset</span></span>|<span data-ttu-id="83c91-143">Última sincronização de data e hora.</span><span class="sxs-lookup"><span data-stu-id="83c91-143">Last sync date and time.</span></span>|
|<span data-ttu-id="83c91-144">installState</span><span class="sxs-lookup"><span data-stu-id="83c91-144">installState</span></span>|[<span data-ttu-id="83c91-145">installState</span><span class="sxs-lookup"><span data-stu-id="83c91-145">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="83c91-146">O estado de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="83c91-146">The install state of the eBook.</span></span> <span data-ttu-id="83c91-147">Os valores possíveis são: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="83c91-147">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="83c91-148">errorCode</span><span class="sxs-lookup"><span data-stu-id="83c91-148">errorCode</span></span>|<span data-ttu-id="83c91-149">String</span><span class="sxs-lookup"><span data-stu-id="83c91-149">String</span></span>|<span data-ttu-id="83c91-150">O código de erro de falhas de instalação.</span><span class="sxs-lookup"><span data-stu-id="83c91-150">The error code for install failures.</span></span>|
|<span data-ttu-id="83c91-151">osVersion</span><span class="sxs-lookup"><span data-stu-id="83c91-151">osVersion</span></span>|<span data-ttu-id="83c91-152">String</span><span class="sxs-lookup"><span data-stu-id="83c91-152">String</span></span>|<span data-ttu-id="83c91-153">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="83c91-153">OS Version.</span></span>|
|<span data-ttu-id="83c91-154">osDescription</span><span class="sxs-lookup"><span data-stu-id="83c91-154">osDescription</span></span>|<span data-ttu-id="83c91-155">String</span><span class="sxs-lookup"><span data-stu-id="83c91-155">String</span></span>|<span data-ttu-id="83c91-156">Descrição do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="83c91-156">OS Description.</span></span>|
|<span data-ttu-id="83c91-157">userName</span><span class="sxs-lookup"><span data-stu-id="83c91-157">userName</span></span>|<span data-ttu-id="83c91-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83c91-158">String</span></span>|<span data-ttu-id="83c91-159">Nome de usuário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="83c91-159">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="83c91-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="83c91-160">Response</span></span>
<span data-ttu-id="83c91-161">Se tiver êxito, esse método retornará um código de resposta `200 OK` e um objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83c91-161">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83c91-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83c91-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="83c91-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83c91-163">Request</span></span>
<span data-ttu-id="83c91-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="83c91-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```

### <a name="response"></a><span data-ttu-id="83c91-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="83c91-165">Response</span></span>
<span data-ttu-id="83c91-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83c91-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "b9feb68f-b68f-b9fe-8fb6-feb98fb6feb9",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```




