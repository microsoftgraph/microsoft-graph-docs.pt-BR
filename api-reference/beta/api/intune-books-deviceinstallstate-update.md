---
title: Atualizar deviceInstallState
description: Atualizar as propriedades de um objeto deviceInstallState.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 65569fbe609b8404d7e55ad6de452e30d3bd1cbf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939697"
---
# <a name="update-deviceinstallstate"></a><span data-ttu-id="be9d6-103">Atualizar deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="be9d6-103">Update deviceInstallState</span></span>

> <span data-ttu-id="be9d6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="be9d6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be9d6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="be9d6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="be9d6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="be9d6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be9d6-107">Atualizar as propriedades de um objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="be9d6-107">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="be9d6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="be9d6-108">Prerequisites</span></span>
<span data-ttu-id="be9d6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be9d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be9d6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be9d6-111">Permission type</span></span>|<span data-ttu-id="be9d6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="be9d6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be9d6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be9d6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="be9d6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be9d6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="be9d6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be9d6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be9d6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be9d6-116">Not supported.</span></span>|
|<span data-ttu-id="be9d6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be9d6-117">Application</span></span>|<span data-ttu-id="be9d6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be9d6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be9d6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be9d6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="be9d6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be9d6-120">Request headers</span></span>
|<span data-ttu-id="be9d6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="be9d6-121">Header</span></span>|<span data-ttu-id="be9d6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="be9d6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be9d6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="be9d6-123">Authorization</span></span>|<span data-ttu-id="be9d6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be9d6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be9d6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="be9d6-125">Accept</span></span>|<span data-ttu-id="be9d6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="be9d6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be9d6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be9d6-127">Request body</span></span>
<span data-ttu-id="be9d6-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="be9d6-128">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

<span data-ttu-id="be9d6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="be9d6-129">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

|<span data-ttu-id="be9d6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be9d6-130">Property</span></span>|<span data-ttu-id="be9d6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="be9d6-131">Type</span></span>|<span data-ttu-id="be9d6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="be9d6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be9d6-133">id</span><span class="sxs-lookup"><span data-stu-id="be9d6-133">id</span></span>|<span data-ttu-id="be9d6-134">String</span><span class="sxs-lookup"><span data-stu-id="be9d6-134">String</span></span>|<span data-ttu-id="be9d6-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="be9d6-135">Key of the entity.</span></span>|
|<span data-ttu-id="be9d6-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="be9d6-136">deviceName</span></span>|<span data-ttu-id="be9d6-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be9d6-137">String</span></span>|<span data-ttu-id="be9d6-138">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="be9d6-138">Device name.</span></span>|
|<span data-ttu-id="be9d6-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="be9d6-139">deviceId</span></span>|<span data-ttu-id="be9d6-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be9d6-140">String</span></span>|<span data-ttu-id="be9d6-141">ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="be9d6-141">Device Id.</span></span>|
|<span data-ttu-id="be9d6-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="be9d6-142">lastSyncDateTime</span></span>|<span data-ttu-id="be9d6-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be9d6-143">DateTimeOffset</span></span>|<span data-ttu-id="be9d6-144">Última sincronização de data e hora.</span><span class="sxs-lookup"><span data-stu-id="be9d6-144">Last sync date and time.</span></span>|
|<span data-ttu-id="be9d6-145">installState</span><span class="sxs-lookup"><span data-stu-id="be9d6-145">installState</span></span>|[<span data-ttu-id="be9d6-146">installState</span><span class="sxs-lookup"><span data-stu-id="be9d6-146">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="be9d6-147">O estado de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="be9d6-147">The install state of the eBook.</span></span> <span data-ttu-id="be9d6-148">Os valores possíveis são: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="be9d6-148">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="be9d6-149">errorCode</span><span class="sxs-lookup"><span data-stu-id="be9d6-149">errorCode</span></span>|<span data-ttu-id="be9d6-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be9d6-150">String</span></span>|<span data-ttu-id="be9d6-151">O código de erro de falhas de instalação.</span><span class="sxs-lookup"><span data-stu-id="be9d6-151">The error code for install failures.</span></span>|
|<span data-ttu-id="be9d6-152">osVersion</span><span class="sxs-lookup"><span data-stu-id="be9d6-152">osVersion</span></span>|<span data-ttu-id="be9d6-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be9d6-153">String</span></span>|<span data-ttu-id="be9d6-154">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="be9d6-154">OS Version.</span></span>|
|<span data-ttu-id="be9d6-155">osDescription</span><span class="sxs-lookup"><span data-stu-id="be9d6-155">osDescription</span></span>|<span data-ttu-id="be9d6-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be9d6-156">String</span></span>|<span data-ttu-id="be9d6-157">Descrição do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="be9d6-157">OS Description.</span></span>|
|<span data-ttu-id="be9d6-158">userName</span><span class="sxs-lookup"><span data-stu-id="be9d6-158">userName</span></span>|<span data-ttu-id="be9d6-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be9d6-159">String</span></span>|<span data-ttu-id="be9d6-160">Nome de usuário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="be9d6-160">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="be9d6-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="be9d6-161">Response</span></span>
<span data-ttu-id="be9d6-162">Se tiver êxito, esse método retornará um código de resposta `200 OK` e um objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be9d6-162">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be9d6-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be9d6-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="be9d6-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be9d6-164">Request</span></span>
<span data-ttu-id="be9d6-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="be9d6-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="be9d6-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="be9d6-166">Response</span></span>
<span data-ttu-id="be9d6-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="be9d6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





