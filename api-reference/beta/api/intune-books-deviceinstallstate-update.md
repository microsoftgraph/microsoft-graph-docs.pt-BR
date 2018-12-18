---
title: Atualizar deviceInstallState
description: Atualizar as propriedades de um objeto deviceInstallState.
author: tfitzmac
ms.openlocfilehash: 1f674b1c732b5804fd83c89620612354e8daccfa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325631"
---
# <a name="update-deviceinstallstate"></a><span data-ttu-id="4ea2c-103">Atualizar deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="4ea2c-103">Update deviceInstallState</span></span>

> <span data-ttu-id="4ea2c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4ea2c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ea2c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4ea2c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4ea2c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4ea2c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ea2c-107">Atualizar as propriedades de um objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="4ea2c-107">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4ea2c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4ea2c-108">Prerequisites</span></span>
<span data-ttu-id="4ea2c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ea2c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ea2c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ea2c-111">Permission type</span></span>|<span data-ttu-id="4ea2c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4ea2c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ea2c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ea2c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4ea2c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ea2c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4ea2c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ea2c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ea2c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ea2c-116">Not supported.</span></span>|
|<span data-ttu-id="4ea2c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ea2c-117">Application</span></span>|<span data-ttu-id="4ea2c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ea2c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ea2c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ea2c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="4ea2c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ea2c-120">Request headers</span></span>
|<span data-ttu-id="4ea2c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4ea2c-121">Header</span></span>|<span data-ttu-id="4ea2c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4ea2c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ea2c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ea2c-123">Authorization</span></span>|<span data-ttu-id="4ea2c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ea2c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ea2c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4ea2c-125">Accept</span></span>|<span data-ttu-id="4ea2c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4ea2c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ea2c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ea2c-127">Request body</span></span>
<span data-ttu-id="4ea2c-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="4ea2c-128">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

<span data-ttu-id="4ea2c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="4ea2c-129">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

|<span data-ttu-id="4ea2c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ea2c-130">Property</span></span>|<span data-ttu-id="4ea2c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ea2c-131">Type</span></span>|<span data-ttu-id="4ea2c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ea2c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ea2c-133">id</span><span class="sxs-lookup"><span data-stu-id="4ea2c-133">id</span></span>|<span data-ttu-id="4ea2c-134">String</span><span class="sxs-lookup"><span data-stu-id="4ea2c-134">String</span></span>|<span data-ttu-id="4ea2c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4ea2c-135">Key of the entity.</span></span>|
|<span data-ttu-id="4ea2c-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="4ea2c-136">deviceName</span></span>|<span data-ttu-id="4ea2c-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ea2c-137">String</span></span>|<span data-ttu-id="4ea2c-138">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4ea2c-138">Device name.</span></span>|
|<span data-ttu-id="4ea2c-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="4ea2c-139">deviceId</span></span>|<span data-ttu-id="4ea2c-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ea2c-140">String</span></span>|<span data-ttu-id="4ea2c-141">ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4ea2c-141">Device Id.</span></span>|
|<span data-ttu-id="4ea2c-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4ea2c-142">lastSyncDateTime</span></span>|<span data-ttu-id="4ea2c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ea2c-143">DateTimeOffset</span></span>|<span data-ttu-id="4ea2c-144">Última sincronização de data e hora.</span><span class="sxs-lookup"><span data-stu-id="4ea2c-144">Last sync date and time.</span></span>|
|<span data-ttu-id="4ea2c-145">installState</span><span class="sxs-lookup"><span data-stu-id="4ea2c-145">installState</span></span>|[<span data-ttu-id="4ea2c-146">installState</span><span class="sxs-lookup"><span data-stu-id="4ea2c-146">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="4ea2c-147">O estado de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="4ea2c-147">The install state of the eBook.</span></span> <span data-ttu-id="4ea2c-148">Os valores possíveis são: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="4ea2c-148">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="4ea2c-149">errorCode</span><span class="sxs-lookup"><span data-stu-id="4ea2c-149">errorCode</span></span>|<span data-ttu-id="4ea2c-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ea2c-150">String</span></span>|<span data-ttu-id="4ea2c-151">O código de erro de falhas de instalação.</span><span class="sxs-lookup"><span data-stu-id="4ea2c-151">The error code for install failures.</span></span>|
|<span data-ttu-id="4ea2c-152">osVersion</span><span class="sxs-lookup"><span data-stu-id="4ea2c-152">osVersion</span></span>|<span data-ttu-id="4ea2c-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ea2c-153">String</span></span>|<span data-ttu-id="4ea2c-154">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="4ea2c-154">OS Version.</span></span>|
|<span data-ttu-id="4ea2c-155">osDescription</span><span class="sxs-lookup"><span data-stu-id="4ea2c-155">osDescription</span></span>|<span data-ttu-id="4ea2c-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ea2c-156">String</span></span>|<span data-ttu-id="4ea2c-157">Descrição do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="4ea2c-157">OS Description.</span></span>|
|<span data-ttu-id="4ea2c-158">userName</span><span class="sxs-lookup"><span data-stu-id="4ea2c-158">userName</span></span>|<span data-ttu-id="4ea2c-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ea2c-159">String</span></span>|<span data-ttu-id="4ea2c-160">Nome de usuário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4ea2c-160">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="4ea2c-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ea2c-161">Response</span></span>
<span data-ttu-id="4ea2c-162">Se tiver êxito, esse método retornará um código de resposta `200 OK` e um objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ea2c-162">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ea2c-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ea2c-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="4ea2c-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ea2c-164">Request</span></span>
<span data-ttu-id="4ea2c-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ea2c-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
Content-type: application/json
Content-length: 317

{
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

### <a name="response"></a><span data-ttu-id="4ea2c-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ea2c-166">Response</span></span>
<span data-ttu-id="4ea2c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ea2c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





