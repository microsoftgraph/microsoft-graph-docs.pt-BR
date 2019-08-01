---
title: Atualizar deviceInstallState
description: Atualizar as propriedades de um objeto deviceInstallState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5da7df5df6966cabf5b2435057a09399c00f8152
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015863"
---
# <a name="update-deviceinstallstate"></a><span data-ttu-id="06b84-103">Atualizar deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="06b84-103">Update deviceInstallState</span></span>

> <span data-ttu-id="06b84-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="06b84-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06b84-105">Atualizar as propriedades de um objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="06b84-105">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06b84-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06b84-106">Prerequisites</span></span>
<span data-ttu-id="06b84-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06b84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06b84-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06b84-109">Permission type</span></span>|<span data-ttu-id="06b84-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="06b84-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06b84-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06b84-111">Delegated (work or school account)</span></span>|<span data-ttu-id="06b84-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06b84-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="06b84-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06b84-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06b84-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06b84-114">Not supported.</span></span>|
|<span data-ttu-id="06b84-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06b84-115">Application</span></span>|<span data-ttu-id="06b84-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06b84-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06b84-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06b84-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="06b84-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06b84-118">Request headers</span></span>
|<span data-ttu-id="06b84-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06b84-119">Header</span></span>|<span data-ttu-id="06b84-120">Valor</span><span class="sxs-lookup"><span data-stu-id="06b84-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06b84-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="06b84-121">Authorization</span></span>|<span data-ttu-id="06b84-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06b84-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06b84-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="06b84-123">Accept</span></span>|<span data-ttu-id="06b84-124">application/json</span><span class="sxs-lookup"><span data-stu-id="06b84-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06b84-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06b84-125">Request body</span></span>
<span data-ttu-id="06b84-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="06b84-126">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

<span data-ttu-id="06b84-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="06b84-127">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

|<span data-ttu-id="06b84-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06b84-128">Property</span></span>|<span data-ttu-id="06b84-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="06b84-129">Type</span></span>|<span data-ttu-id="06b84-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="06b84-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06b84-131">id</span><span class="sxs-lookup"><span data-stu-id="06b84-131">id</span></span>|<span data-ttu-id="06b84-132">String</span><span class="sxs-lookup"><span data-stu-id="06b84-132">String</span></span>|<span data-ttu-id="06b84-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="06b84-133">Key of the entity.</span></span>|
|<span data-ttu-id="06b84-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="06b84-134">deviceName</span></span>|<span data-ttu-id="06b84-135">String</span><span class="sxs-lookup"><span data-stu-id="06b84-135">String</span></span>|<span data-ttu-id="06b84-136">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="06b84-136">Device name.</span></span>|
|<span data-ttu-id="06b84-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="06b84-137">deviceId</span></span>|<span data-ttu-id="06b84-138">String</span><span class="sxs-lookup"><span data-stu-id="06b84-138">String</span></span>|<span data-ttu-id="06b84-139">ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="06b84-139">Device Id.</span></span>|
|<span data-ttu-id="06b84-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="06b84-140">lastSyncDateTime</span></span>|<span data-ttu-id="06b84-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06b84-141">DateTimeOffset</span></span>|<span data-ttu-id="06b84-142">Última sincronização de data e hora.</span><span class="sxs-lookup"><span data-stu-id="06b84-142">Last sync date and time.</span></span>|
|<span data-ttu-id="06b84-143">installState</span><span class="sxs-lookup"><span data-stu-id="06b84-143">installState</span></span>|[<span data-ttu-id="06b84-144">installState</span><span class="sxs-lookup"><span data-stu-id="06b84-144">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="06b84-145">O estado de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="06b84-145">The install state of the eBook.</span></span> <span data-ttu-id="06b84-146">Os valores possíveis são: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="06b84-146">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="06b84-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="06b84-147">errorCode</span></span>|<span data-ttu-id="06b84-148">String</span><span class="sxs-lookup"><span data-stu-id="06b84-148">String</span></span>|<span data-ttu-id="06b84-149">O código de erro de falhas de instalação.</span><span class="sxs-lookup"><span data-stu-id="06b84-149">The error code for install failures.</span></span>|
|<span data-ttu-id="06b84-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="06b84-150">osVersion</span></span>|<span data-ttu-id="06b84-151">String</span><span class="sxs-lookup"><span data-stu-id="06b84-151">String</span></span>|<span data-ttu-id="06b84-152">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="06b84-152">OS Version.</span></span>|
|<span data-ttu-id="06b84-153">osDescription</span><span class="sxs-lookup"><span data-stu-id="06b84-153">osDescription</span></span>|<span data-ttu-id="06b84-154">String</span><span class="sxs-lookup"><span data-stu-id="06b84-154">String</span></span>|<span data-ttu-id="06b84-155">Descrição do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="06b84-155">OS Description.</span></span>|
|<span data-ttu-id="06b84-156">userName</span><span class="sxs-lookup"><span data-stu-id="06b84-156">userName</span></span>|<span data-ttu-id="06b84-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06b84-157">String</span></span>|<span data-ttu-id="06b84-158">Nome de usuário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="06b84-158">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="06b84-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="06b84-159">Response</span></span>
<span data-ttu-id="06b84-160">Se tiver êxito, esse método retornará um código de resposta `200 OK` e um objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06b84-160">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06b84-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06b84-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="06b84-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06b84-162">Request</span></span>
<span data-ttu-id="06b84-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06b84-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
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

### <a name="response"></a><span data-ttu-id="06b84-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="06b84-164">Response</span></span>
<span data-ttu-id="06b84-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06b84-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



