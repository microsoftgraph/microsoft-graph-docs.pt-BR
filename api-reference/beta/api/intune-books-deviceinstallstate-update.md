---
title: Atualizar deviceInstallState
description: Atualizar as propriedades de um objeto deviceInstallState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 940c2e88761aefa5bc18c71b7d785c5ceb0b9647
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131887"
---
# <a name="update-deviceinstallstate"></a><span data-ttu-id="151ae-103">Atualizar deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="151ae-103">Update deviceInstallState</span></span>

<span data-ttu-id="151ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="151ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="151ae-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="151ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="151ae-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="151ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="151ae-107">Atualizar as propriedades de um objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="151ae-107">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="151ae-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="151ae-108">Prerequisites</span></span>
<span data-ttu-id="151ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="151ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="151ae-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="151ae-111">Permission type</span></span>|<span data-ttu-id="151ae-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="151ae-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="151ae-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="151ae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="151ae-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="151ae-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="151ae-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="151ae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="151ae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="151ae-116">Not supported.</span></span>|
|<span data-ttu-id="151ae-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="151ae-117">Application</span></span>|<span data-ttu-id="151ae-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="151ae-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="151ae-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="151ae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="151ae-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="151ae-120">Request headers</span></span>
|<span data-ttu-id="151ae-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="151ae-121">Header</span></span>|<span data-ttu-id="151ae-122">Valor</span><span class="sxs-lookup"><span data-stu-id="151ae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="151ae-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="151ae-123">Authorization</span></span>|<span data-ttu-id="151ae-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="151ae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="151ae-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="151ae-125">Accept</span></span>|<span data-ttu-id="151ae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="151ae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="151ae-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="151ae-127">Request body</span></span>
<span data-ttu-id="151ae-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="151ae-128">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

<span data-ttu-id="151ae-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="151ae-129">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

|<span data-ttu-id="151ae-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="151ae-130">Property</span></span>|<span data-ttu-id="151ae-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="151ae-131">Type</span></span>|<span data-ttu-id="151ae-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="151ae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="151ae-133">id</span><span class="sxs-lookup"><span data-stu-id="151ae-133">id</span></span>|<span data-ttu-id="151ae-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="151ae-134">String</span></span>|<span data-ttu-id="151ae-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="151ae-135">Key of the entity.</span></span>|
|<span data-ttu-id="151ae-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="151ae-136">deviceName</span></span>|<span data-ttu-id="151ae-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="151ae-137">String</span></span>|<span data-ttu-id="151ae-138">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="151ae-138">Device name.</span></span>|
|<span data-ttu-id="151ae-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="151ae-139">deviceId</span></span>|<span data-ttu-id="151ae-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="151ae-140">String</span></span>|<span data-ttu-id="151ae-141">ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="151ae-141">Device Id.</span></span>|
|<span data-ttu-id="151ae-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="151ae-142">lastSyncDateTime</span></span>|<span data-ttu-id="151ae-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="151ae-143">DateTimeOffset</span></span>|<span data-ttu-id="151ae-144">Última sincronização de data e hora.</span><span class="sxs-lookup"><span data-stu-id="151ae-144">Last sync date and time.</span></span>|
|<span data-ttu-id="151ae-145">installState</span><span class="sxs-lookup"><span data-stu-id="151ae-145">installState</span></span>|[<span data-ttu-id="151ae-146">installState</span><span class="sxs-lookup"><span data-stu-id="151ae-146">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="151ae-147">O estado de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="151ae-147">The install state of the eBook.</span></span> <span data-ttu-id="151ae-148">Os valores possíveis são: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="151ae-148">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="151ae-149">errorCode</span><span class="sxs-lookup"><span data-stu-id="151ae-149">errorCode</span></span>|<span data-ttu-id="151ae-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="151ae-150">String</span></span>|<span data-ttu-id="151ae-151">O código de erro de falhas de instalação.</span><span class="sxs-lookup"><span data-stu-id="151ae-151">The error code for install failures.</span></span>|
|<span data-ttu-id="151ae-152">osVersion</span><span class="sxs-lookup"><span data-stu-id="151ae-152">osVersion</span></span>|<span data-ttu-id="151ae-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="151ae-153">String</span></span>|<span data-ttu-id="151ae-154">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="151ae-154">OS Version.</span></span>|
|<span data-ttu-id="151ae-155">osDescription</span><span class="sxs-lookup"><span data-stu-id="151ae-155">osDescription</span></span>|<span data-ttu-id="151ae-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="151ae-156">String</span></span>|<span data-ttu-id="151ae-157">Descrição do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="151ae-157">OS Description.</span></span>|
|<span data-ttu-id="151ae-158">userName</span><span class="sxs-lookup"><span data-stu-id="151ae-158">userName</span></span>|<span data-ttu-id="151ae-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="151ae-159">String</span></span>|<span data-ttu-id="151ae-160">Nome de usuário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="151ae-160">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="151ae-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="151ae-161">Response</span></span>
<span data-ttu-id="151ae-162">Se tiver êxito, esse método retornará um código de resposta `200 OK` e um objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="151ae-162">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="151ae-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="151ae-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="151ae-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="151ae-164">Request</span></span>
<span data-ttu-id="151ae-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="151ae-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="151ae-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="151ae-166">Response</span></span>
<span data-ttu-id="151ae-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="151ae-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




