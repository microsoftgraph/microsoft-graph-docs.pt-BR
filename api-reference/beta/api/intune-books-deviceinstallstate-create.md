---
title: Criar deviceInstallState
description: Criar um novo objeto deviceInstallState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eff7e9940ed5a371eb33de50a0f4aec0a3198224
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35959457"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="4e229-103">Criar deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="4e229-103">Create deviceInstallState</span></span>

> <span data-ttu-id="4e229-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4e229-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e229-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4e229-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e229-106">Criar um novo objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="4e229-106">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e229-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4e229-107">Prerequisites</span></span>
<span data-ttu-id="4e229-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e229-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e229-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e229-110">Permission type</span></span>|<span data-ttu-id="4e229-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4e229-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e229-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e229-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4e229-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e229-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4e229-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e229-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e229-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e229-115">Not supported.</span></span>|
|<span data-ttu-id="4e229-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e229-116">Application</span></span>|<span data-ttu-id="4e229-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e229-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e229-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e229-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="4e229-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e229-119">Request headers</span></span>
|<span data-ttu-id="4e229-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4e229-120">Header</span></span>|<span data-ttu-id="4e229-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4e229-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e229-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e229-122">Authorization</span></span>|<span data-ttu-id="4e229-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e229-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e229-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4e229-124">Accept</span></span>|<span data-ttu-id="4e229-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4e229-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e229-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e229-126">Request body</span></span>
<span data-ttu-id="4e229-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceInstallState.</span><span class="sxs-lookup"><span data-stu-id="4e229-127">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="4e229-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceInstallState.</span><span class="sxs-lookup"><span data-stu-id="4e229-128">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="4e229-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e229-129">Property</span></span>|<span data-ttu-id="4e229-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e229-130">Type</span></span>|<span data-ttu-id="4e229-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e229-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e229-132">id</span><span class="sxs-lookup"><span data-stu-id="4e229-132">id</span></span>|<span data-ttu-id="4e229-133">String</span><span class="sxs-lookup"><span data-stu-id="4e229-133">String</span></span>|<span data-ttu-id="4e229-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4e229-134">Key of the entity.</span></span>|
|<span data-ttu-id="4e229-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="4e229-135">deviceName</span></span>|<span data-ttu-id="4e229-136">String</span><span class="sxs-lookup"><span data-stu-id="4e229-136">String</span></span>|<span data-ttu-id="4e229-137">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4e229-137">Device name.</span></span>|
|<span data-ttu-id="4e229-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="4e229-138">deviceId</span></span>|<span data-ttu-id="4e229-139">String</span><span class="sxs-lookup"><span data-stu-id="4e229-139">String</span></span>|<span data-ttu-id="4e229-140">ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4e229-140">Device Id.</span></span>|
|<span data-ttu-id="4e229-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4e229-141">lastSyncDateTime</span></span>|<span data-ttu-id="4e229-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e229-142">DateTimeOffset</span></span>|<span data-ttu-id="4e229-143">Última sincronização de data e hora.</span><span class="sxs-lookup"><span data-stu-id="4e229-143">Last sync date and time.</span></span>|
|<span data-ttu-id="4e229-144">installState</span><span class="sxs-lookup"><span data-stu-id="4e229-144">installState</span></span>|[<span data-ttu-id="4e229-145">installState</span><span class="sxs-lookup"><span data-stu-id="4e229-145">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="4e229-146">O estado de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="4e229-146">The install state of the eBook.</span></span> <span data-ttu-id="4e229-147">Os valores possíveis são: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="4e229-147">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="4e229-148">errorCode</span><span class="sxs-lookup"><span data-stu-id="4e229-148">errorCode</span></span>|<span data-ttu-id="4e229-149">String</span><span class="sxs-lookup"><span data-stu-id="4e229-149">String</span></span>|<span data-ttu-id="4e229-150">O código de erro de falhas de instalação.</span><span class="sxs-lookup"><span data-stu-id="4e229-150">The error code for install failures.</span></span>|
|<span data-ttu-id="4e229-151">osVersion</span><span class="sxs-lookup"><span data-stu-id="4e229-151">osVersion</span></span>|<span data-ttu-id="4e229-152">String</span><span class="sxs-lookup"><span data-stu-id="4e229-152">String</span></span>|<span data-ttu-id="4e229-153">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="4e229-153">OS Version.</span></span>|
|<span data-ttu-id="4e229-154">osDescription</span><span class="sxs-lookup"><span data-stu-id="4e229-154">osDescription</span></span>|<span data-ttu-id="4e229-155">String</span><span class="sxs-lookup"><span data-stu-id="4e229-155">String</span></span>|<span data-ttu-id="4e229-156">Descrição do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="4e229-156">OS Description.</span></span>|
|<span data-ttu-id="4e229-157">userName</span><span class="sxs-lookup"><span data-stu-id="4e229-157">userName</span></span>|<span data-ttu-id="4e229-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e229-158">String</span></span>|<span data-ttu-id="4e229-159">Nome de usuário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4e229-159">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="4e229-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e229-160">Response</span></span>
<span data-ttu-id="4e229-161">Se tiver êxito, esse método retornará um código de resposta `201 Created` e um objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e229-161">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e229-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4e229-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e229-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e229-163">Request</span></span>
<span data-ttu-id="4e229-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e229-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
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

### <a name="response"></a><span data-ttu-id="4e229-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e229-165">Response</span></span>
<span data-ttu-id="4e229-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4e229-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





