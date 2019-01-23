---
title: Atualizar deviceInstallState
description: Atualizar as propriedades de um objeto deviceInstallState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3d73f1cc881d918f385bfdc8d98cf9a1451a554e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394786"
---
# <a name="update-deviceinstallstate"></a><span data-ttu-id="f9845-103">Atualizar deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="f9845-103">Update deviceInstallState</span></span>

> <span data-ttu-id="f9845-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f9845-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f9845-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f9845-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9845-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f9845-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9845-107">Atualizar as propriedades de um objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="f9845-107">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9845-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f9845-108">Prerequisites</span></span>
<span data-ttu-id="f9845-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f9845-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f9845-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9845-111">Permission type</span></span>|<span data-ttu-id="f9845-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f9845-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9845-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9845-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f9845-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9845-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f9845-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9845-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9845-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9845-116">Not supported.</span></span>|
|<span data-ttu-id="f9845-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9845-117">Application</span></span>|<span data-ttu-id="f9845-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9845-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9845-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9845-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="f9845-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9845-120">Request headers</span></span>
|<span data-ttu-id="f9845-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f9845-121">Header</span></span>|<span data-ttu-id="f9845-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f9845-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9845-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9845-123">Authorization</span></span>|<span data-ttu-id="f9845-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9845-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9845-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f9845-125">Accept</span></span>|<span data-ttu-id="f9845-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f9845-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9845-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9845-127">Request body</span></span>
<span data-ttu-id="f9845-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="f9845-128">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

<span data-ttu-id="f9845-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="f9845-129">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

|<span data-ttu-id="f9845-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9845-130">Property</span></span>|<span data-ttu-id="f9845-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9845-131">Type</span></span>|<span data-ttu-id="f9845-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9845-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9845-133">id</span><span class="sxs-lookup"><span data-stu-id="f9845-133">id</span></span>|<span data-ttu-id="f9845-134">String</span><span class="sxs-lookup"><span data-stu-id="f9845-134">String</span></span>|<span data-ttu-id="f9845-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f9845-135">Key of the entity.</span></span>|
|<span data-ttu-id="f9845-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="f9845-136">deviceName</span></span>|<span data-ttu-id="f9845-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9845-137">String</span></span>|<span data-ttu-id="f9845-138">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9845-138">Device name.</span></span>|
|<span data-ttu-id="f9845-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="f9845-139">deviceId</span></span>|<span data-ttu-id="f9845-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9845-140">String</span></span>|<span data-ttu-id="f9845-141">ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9845-141">Device Id.</span></span>|
|<span data-ttu-id="f9845-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f9845-142">lastSyncDateTime</span></span>|<span data-ttu-id="f9845-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9845-143">DateTimeOffset</span></span>|<span data-ttu-id="f9845-144">Última sincronização de data e hora.</span><span class="sxs-lookup"><span data-stu-id="f9845-144">Last sync date and time.</span></span>|
|<span data-ttu-id="f9845-145">installState</span><span class="sxs-lookup"><span data-stu-id="f9845-145">installState</span></span>|[<span data-ttu-id="f9845-146">installState</span><span class="sxs-lookup"><span data-stu-id="f9845-146">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="f9845-147">O estado de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="f9845-147">The install state of the eBook.</span></span> <span data-ttu-id="f9845-148">Os valores possíveis são: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f9845-148">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="f9845-149">errorCode</span><span class="sxs-lookup"><span data-stu-id="f9845-149">errorCode</span></span>|<span data-ttu-id="f9845-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9845-150">String</span></span>|<span data-ttu-id="f9845-151">O código de erro de falhas de instalação.</span><span class="sxs-lookup"><span data-stu-id="f9845-151">The error code for install failures.</span></span>|
|<span data-ttu-id="f9845-152">osVersion</span><span class="sxs-lookup"><span data-stu-id="f9845-152">osVersion</span></span>|<span data-ttu-id="f9845-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9845-153">String</span></span>|<span data-ttu-id="f9845-154">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="f9845-154">OS Version.</span></span>|
|<span data-ttu-id="f9845-155">osDescription</span><span class="sxs-lookup"><span data-stu-id="f9845-155">osDescription</span></span>|<span data-ttu-id="f9845-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9845-156">String</span></span>|<span data-ttu-id="f9845-157">Descrição do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="f9845-157">OS Description.</span></span>|
|<span data-ttu-id="f9845-158">userName</span><span class="sxs-lookup"><span data-stu-id="f9845-158">userName</span></span>|<span data-ttu-id="f9845-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9845-159">String</span></span>|<span data-ttu-id="f9845-160">Nome de usuário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9845-160">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="f9845-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9845-161">Response</span></span>
<span data-ttu-id="f9845-162">Se tiver êxito, esse método retornará um código de resposta `200 OK` e um objeto [deviceInstallState](../resources/intune-books-deviceinstallstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9845-162">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9845-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9845-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9845-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9845-164">Request</span></span>
<span data-ttu-id="f9845-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9845-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f9845-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9845-166">Response</span></span>
<span data-ttu-id="f9845-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9845-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




