---
title: Criar deviceInstallState
description: Criar um novo objeto deviceInstallState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 95822b40cb5be71994730c0c9fdf258f9af6d695
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759410"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="3152c-103">Criar deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="3152c-103">Create deviceInstallState</span></span>

<span data-ttu-id="3152c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3152c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3152c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3152c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3152c-106">Criar um novo objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="3152c-106">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3152c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3152c-107">Prerequisites</span></span>
<span data-ttu-id="3152c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3152c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3152c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3152c-110">Permission type</span></span>|<span data-ttu-id="3152c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3152c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3152c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3152c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3152c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3152c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3152c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3152c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3152c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3152c-115">Not supported.</span></span>|
|<span data-ttu-id="3152c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3152c-116">Application</span></span>|<span data-ttu-id="3152c-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3152c-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3152c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3152c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="3152c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3152c-119">Request headers</span></span>
|<span data-ttu-id="3152c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3152c-120">Header</span></span>|<span data-ttu-id="3152c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3152c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3152c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3152c-122">Authorization</span></span>|<span data-ttu-id="3152c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3152c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3152c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3152c-124">Accept</span></span>|<span data-ttu-id="3152c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3152c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3152c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3152c-126">Request body</span></span>
<span data-ttu-id="3152c-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceInstallState.</span><span class="sxs-lookup"><span data-stu-id="3152c-127">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="3152c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceInstallState.</span><span class="sxs-lookup"><span data-stu-id="3152c-128">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="3152c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3152c-129">Property</span></span>|<span data-ttu-id="3152c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3152c-130">Type</span></span>|<span data-ttu-id="3152c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3152c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3152c-132">id</span><span class="sxs-lookup"><span data-stu-id="3152c-132">id</span></span>|<span data-ttu-id="3152c-133">String</span><span class="sxs-lookup"><span data-stu-id="3152c-133">String</span></span>|<span data-ttu-id="3152c-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3152c-134">Key of the entity.</span></span>|
|<span data-ttu-id="3152c-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="3152c-135">deviceName</span></span>|<span data-ttu-id="3152c-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3152c-136">String</span></span>|<span data-ttu-id="3152c-137">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3152c-137">Device name.</span></span>|
|<span data-ttu-id="3152c-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="3152c-138">deviceId</span></span>|<span data-ttu-id="3152c-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3152c-139">String</span></span>|<span data-ttu-id="3152c-140">ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3152c-140">Device Id.</span></span>|
|<span data-ttu-id="3152c-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3152c-141">lastSyncDateTime</span></span>|<span data-ttu-id="3152c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3152c-142">DateTimeOffset</span></span>|<span data-ttu-id="3152c-143">Última sincronização de data e hora.</span><span class="sxs-lookup"><span data-stu-id="3152c-143">Last sync date and time.</span></span>|
|<span data-ttu-id="3152c-144">installState</span><span class="sxs-lookup"><span data-stu-id="3152c-144">installState</span></span>|[<span data-ttu-id="3152c-145">installState</span><span class="sxs-lookup"><span data-stu-id="3152c-145">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="3152c-146">O estado de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="3152c-146">The install state of the eBook.</span></span> <span data-ttu-id="3152c-147">Os valores possíveis são: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="3152c-147">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="3152c-148">errorCode</span><span class="sxs-lookup"><span data-stu-id="3152c-148">errorCode</span></span>|<span data-ttu-id="3152c-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3152c-149">String</span></span>|<span data-ttu-id="3152c-150">O código de erro de falhas de instalação.</span><span class="sxs-lookup"><span data-stu-id="3152c-150">The error code for install failures.</span></span>|
|<span data-ttu-id="3152c-151">osVersion</span><span class="sxs-lookup"><span data-stu-id="3152c-151">osVersion</span></span>|<span data-ttu-id="3152c-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3152c-152">String</span></span>|<span data-ttu-id="3152c-153">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="3152c-153">OS Version.</span></span>|
|<span data-ttu-id="3152c-154">osDescription</span><span class="sxs-lookup"><span data-stu-id="3152c-154">osDescription</span></span>|<span data-ttu-id="3152c-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3152c-155">String</span></span>|<span data-ttu-id="3152c-156">Descrição do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="3152c-156">OS Description.</span></span>|
|<span data-ttu-id="3152c-157">userName</span><span class="sxs-lookup"><span data-stu-id="3152c-157">userName</span></span>|<span data-ttu-id="3152c-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3152c-158">String</span></span>|<span data-ttu-id="3152c-159">Nome de usuário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3152c-159">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="3152c-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="3152c-160">Response</span></span>
<span data-ttu-id="3152c-161">Se tiver êxito, esse método retornará um código de resposta `201 Created` e um objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3152c-161">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3152c-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3152c-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="3152c-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3152c-163">Request</span></span>
<span data-ttu-id="3152c-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3152c-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
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

### <a name="response"></a><span data-ttu-id="3152c-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="3152c-165">Response</span></span>
<span data-ttu-id="3152c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3152c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




