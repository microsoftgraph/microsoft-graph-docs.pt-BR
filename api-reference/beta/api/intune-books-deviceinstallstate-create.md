---
title: Criar deviceInstallState
description: Criar um novo objeto deviceInstallState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f789dbde14ad59b587e6f0c8bfe87038eb0a0ac2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47975868"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="54892-103">Criar deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="54892-103">Create deviceInstallState</span></span>

<span data-ttu-id="54892-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54892-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54892-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="54892-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54892-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="54892-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54892-107">Criar um novo objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="54892-107">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54892-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="54892-108">Prerequisites</span></span>
<span data-ttu-id="54892-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54892-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54892-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54892-111">Permission type</span></span>|<span data-ttu-id="54892-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="54892-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54892-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54892-113">Delegated (work or school account)</span></span>|<span data-ttu-id="54892-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54892-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="54892-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54892-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54892-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54892-116">Not supported.</span></span>|
|<span data-ttu-id="54892-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54892-117">Application</span></span>|<span data-ttu-id="54892-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54892-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="54892-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54892-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="54892-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54892-120">Request headers</span></span>
|<span data-ttu-id="54892-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="54892-121">Header</span></span>|<span data-ttu-id="54892-122">Valor</span><span class="sxs-lookup"><span data-stu-id="54892-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54892-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="54892-123">Authorization</span></span>|<span data-ttu-id="54892-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54892-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54892-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="54892-125">Accept</span></span>|<span data-ttu-id="54892-126">application/json</span><span class="sxs-lookup"><span data-stu-id="54892-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54892-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54892-127">Request body</span></span>
<span data-ttu-id="54892-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceInstallState.</span><span class="sxs-lookup"><span data-stu-id="54892-128">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="54892-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceInstallState.</span><span class="sxs-lookup"><span data-stu-id="54892-129">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="54892-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54892-130">Property</span></span>|<span data-ttu-id="54892-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="54892-131">Type</span></span>|<span data-ttu-id="54892-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="54892-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54892-133">id</span><span class="sxs-lookup"><span data-stu-id="54892-133">id</span></span>|<span data-ttu-id="54892-134">String</span><span class="sxs-lookup"><span data-stu-id="54892-134">String</span></span>|<span data-ttu-id="54892-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="54892-135">Key of the entity.</span></span>|
|<span data-ttu-id="54892-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="54892-136">deviceName</span></span>|<span data-ttu-id="54892-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54892-137">String</span></span>|<span data-ttu-id="54892-138">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54892-138">Device name.</span></span>|
|<span data-ttu-id="54892-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="54892-139">deviceId</span></span>|<span data-ttu-id="54892-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54892-140">String</span></span>|<span data-ttu-id="54892-141">ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54892-141">Device Id.</span></span>|
|<span data-ttu-id="54892-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="54892-142">lastSyncDateTime</span></span>|<span data-ttu-id="54892-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54892-143">DateTimeOffset</span></span>|<span data-ttu-id="54892-144">Última sincronização de data e hora.</span><span class="sxs-lookup"><span data-stu-id="54892-144">Last sync date and time.</span></span>|
|<span data-ttu-id="54892-145">installState</span><span class="sxs-lookup"><span data-stu-id="54892-145">installState</span></span>|[<span data-ttu-id="54892-146">installState</span><span class="sxs-lookup"><span data-stu-id="54892-146">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="54892-147">O estado de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="54892-147">The install state of the eBook.</span></span> <span data-ttu-id="54892-148">Os valores possíveis são: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="54892-148">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="54892-149">errorCode</span><span class="sxs-lookup"><span data-stu-id="54892-149">errorCode</span></span>|<span data-ttu-id="54892-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54892-150">String</span></span>|<span data-ttu-id="54892-151">O código de erro de falhas de instalação.</span><span class="sxs-lookup"><span data-stu-id="54892-151">The error code for install failures.</span></span>|
|<span data-ttu-id="54892-152">osVersion</span><span class="sxs-lookup"><span data-stu-id="54892-152">osVersion</span></span>|<span data-ttu-id="54892-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54892-153">String</span></span>|<span data-ttu-id="54892-154">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="54892-154">OS Version.</span></span>|
|<span data-ttu-id="54892-155">osDescription</span><span class="sxs-lookup"><span data-stu-id="54892-155">osDescription</span></span>|<span data-ttu-id="54892-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54892-156">String</span></span>|<span data-ttu-id="54892-157">Descrição do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="54892-157">OS Description.</span></span>|
|<span data-ttu-id="54892-158">userName</span><span class="sxs-lookup"><span data-stu-id="54892-158">userName</span></span>|<span data-ttu-id="54892-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54892-159">String</span></span>|<span data-ttu-id="54892-160">Nome de usuário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54892-160">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="54892-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="54892-161">Response</span></span>
<span data-ttu-id="54892-162">Se tiver êxito, esse método retornará um código de resposta `201 Created` e um objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54892-162">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54892-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54892-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="54892-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54892-164">Request</span></span>
<span data-ttu-id="54892-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54892-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="54892-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="54892-166">Response</span></span>
<span data-ttu-id="54892-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54892-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






