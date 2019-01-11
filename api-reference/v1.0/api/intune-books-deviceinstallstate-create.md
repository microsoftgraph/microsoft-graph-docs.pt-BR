---
title: Criar deviceInstallState
description: Criar um novo objeto deviceInstallState.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 49979b883ffef895124d8bb57837d5c5103a0d67
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825477"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="3692e-103">Criar deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="3692e-103">Create deviceInstallState</span></span>

> <span data-ttu-id="3692e-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3692e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3692e-105">Criar um novo objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="3692e-105">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3692e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3692e-106">Prerequisites</span></span>
<span data-ttu-id="3692e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3692e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3692e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3692e-109">Permission type</span></span>|<span data-ttu-id="3692e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3692e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3692e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3692e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3692e-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3692e-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3692e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3692e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3692e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3692e-114">Not supported.</span></span>|
|<span data-ttu-id="3692e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3692e-115">Application</span></span>|<span data-ttu-id="3692e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3692e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3692e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3692e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="3692e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3692e-118">Request headers</span></span>
|<span data-ttu-id="3692e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3692e-119">Header</span></span>|<span data-ttu-id="3692e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="3692e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3692e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3692e-121">Authorization</span></span>|<span data-ttu-id="3692e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3692e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3692e-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3692e-123">Accept</span></span>|<span data-ttu-id="3692e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3692e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3692e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3692e-125">Request body</span></span>
<span data-ttu-id="3692e-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceInstallState.</span><span class="sxs-lookup"><span data-stu-id="3692e-126">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="3692e-127">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceInstallState.</span><span class="sxs-lookup"><span data-stu-id="3692e-127">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="3692e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3692e-128">Property</span></span>|<span data-ttu-id="3692e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="3692e-129">Type</span></span>|<span data-ttu-id="3692e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="3692e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3692e-131">id</span><span class="sxs-lookup"><span data-stu-id="3692e-131">id</span></span>|<span data-ttu-id="3692e-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3692e-132">String</span></span>|<span data-ttu-id="3692e-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3692e-133">Key of the entity.</span></span>|
|<span data-ttu-id="3692e-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="3692e-134">deviceName</span></span>|<span data-ttu-id="3692e-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3692e-135">String</span></span>|<span data-ttu-id="3692e-136">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3692e-136">Device name.</span></span>|
|<span data-ttu-id="3692e-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="3692e-137">deviceId</span></span>|<span data-ttu-id="3692e-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3692e-138">String</span></span>|<span data-ttu-id="3692e-139">ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3692e-139">Device Id.</span></span>|
|<span data-ttu-id="3692e-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3692e-140">lastSyncDateTime</span></span>|<span data-ttu-id="3692e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3692e-141">DateTimeOffset</span></span>|<span data-ttu-id="3692e-142">Última sincronização de data e hora.</span><span class="sxs-lookup"><span data-stu-id="3692e-142">Last sync date and time.</span></span>|
|<span data-ttu-id="3692e-143">installState</span><span class="sxs-lookup"><span data-stu-id="3692e-143">installState</span></span>|[<span data-ttu-id="3692e-144">installState</span><span class="sxs-lookup"><span data-stu-id="3692e-144">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="3692e-145">O estado de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="3692e-145">The install state of the eBook.</span></span> <span data-ttu-id="3692e-146">Os valores possíveis são: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="3692e-146">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="3692e-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="3692e-147">errorCode</span></span>|<span data-ttu-id="3692e-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3692e-148">String</span></span>|<span data-ttu-id="3692e-149">O código de erro de falhas de instalação.</span><span class="sxs-lookup"><span data-stu-id="3692e-149">The error code for install failures.</span></span>|
|<span data-ttu-id="3692e-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="3692e-150">osVersion</span></span>|<span data-ttu-id="3692e-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3692e-151">String</span></span>|<span data-ttu-id="3692e-152">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="3692e-152">OS Version.</span></span>|
|<span data-ttu-id="3692e-153">osDescription</span><span class="sxs-lookup"><span data-stu-id="3692e-153">osDescription</span></span>|<span data-ttu-id="3692e-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3692e-154">String</span></span>|<span data-ttu-id="3692e-155">Descrição do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="3692e-155">OS Description.</span></span>|
|<span data-ttu-id="3692e-156">userName</span><span class="sxs-lookup"><span data-stu-id="3692e-156">userName</span></span>|<span data-ttu-id="3692e-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3692e-157">String</span></span>|<span data-ttu-id="3692e-158">Nome de usuário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3692e-158">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="3692e-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="3692e-159">Response</span></span>
<span data-ttu-id="3692e-160">Se tiver êxito, esse método retornará um código de resposta `201 Created` e um objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3692e-160">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3692e-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3692e-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="3692e-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3692e-162">Request</span></span>
<span data-ttu-id="3692e-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3692e-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3692e-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="3692e-164">Response</span></span>
<span data-ttu-id="3692e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3692e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



