---
title: Atualizar deviceManagementScriptUserState
description: Atualiza as propriedades de um objeto deviceManagementScriptUserState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7f2d37dec81fb45179fa28268c2a2c49bde219b1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944880"
---
# <a name="update-devicemanagementscriptuserstate"></a><span data-ttu-id="5896d-103">Atualizar deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="5896d-103">Update deviceManagementScriptUserState</span></span>

> <span data-ttu-id="5896d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5896d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5896d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5896d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5896d-106">Atualiza as propriedades de um objeto [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="5896d-106">Update the properties of a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5896d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5896d-107">Prerequisites</span></span>
<span data-ttu-id="5896d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5896d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5896d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5896d-110">Permission type</span></span>|<span data-ttu-id="5896d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5896d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5896d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5896d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5896d-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5896d-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5896d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5896d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5896d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5896d-115">Not supported.</span></span>|
|<span data-ttu-id="5896d-116">Application</span><span class="sxs-lookup"><span data-stu-id="5896d-116">Application</span></span>|<span data-ttu-id="5896d-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5896d-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5896d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5896d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

## <a name="request-headers"></a><span data-ttu-id="5896d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5896d-119">Request headers</span></span>
|<span data-ttu-id="5896d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5896d-120">Header</span></span>|<span data-ttu-id="5896d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5896d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5896d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5896d-122">Authorization</span></span>|<span data-ttu-id="5896d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5896d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5896d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5896d-124">Accept</span></span>|<span data-ttu-id="5896d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5896d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5896d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5896d-126">Request body</span></span>
<span data-ttu-id="5896d-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="5896d-127">In the request body, supply a JSON representation for the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

<span data-ttu-id="5896d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span><span class="sxs-lookup"><span data-stu-id="5896d-128">The following table shows the properties that are required when you create the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>

|<span data-ttu-id="5896d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5896d-129">Property</span></span>|<span data-ttu-id="5896d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5896d-130">Type</span></span>|<span data-ttu-id="5896d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5896d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5896d-132">id</span><span class="sxs-lookup"><span data-stu-id="5896d-132">id</span></span>|<span data-ttu-id="5896d-133">String</span><span class="sxs-lookup"><span data-stu-id="5896d-133">String</span></span>|<span data-ttu-id="5896d-134">Chave da entidade de estado do usuário de script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="5896d-134">Key of the device management script user state entity.</span></span> <span data-ttu-id="5896d-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5896d-135">This property is read-only.</span></span>|
|<span data-ttu-id="5896d-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5896d-136">successDeviceCount</span></span>|<span data-ttu-id="5896d-137">Int32</span><span class="sxs-lookup"><span data-stu-id="5896d-137">Int32</span></span>|<span data-ttu-id="5896d-138">Contagem de dispositivos com êxito para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="5896d-138">Success device count for specific user.</span></span>|
|<span data-ttu-id="5896d-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5896d-139">errorDeviceCount</span></span>|<span data-ttu-id="5896d-140">Int32</span><span class="sxs-lookup"><span data-stu-id="5896d-140">Int32</span></span>|<span data-ttu-id="5896d-141">Contagem de dispositivos de erro para usuário específico.</span><span class="sxs-lookup"><span data-stu-id="5896d-141">Error device count for specific user.</span></span>|
|<span data-ttu-id="5896d-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5896d-142">userPrincipalName</span></span>|<span data-ttu-id="5896d-143">String</span><span class="sxs-lookup"><span data-stu-id="5896d-143">String</span></span>|<span data-ttu-id="5896d-144">Nome principal do usuário do usuário específico.</span><span class="sxs-lookup"><span data-stu-id="5896d-144">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="5896d-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="5896d-145">Response</span></span>
<span data-ttu-id="5896d-146">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5896d-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5896d-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5896d-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="5896d-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5896d-148">Request</span></span>
<span data-ttu-id="5896d-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5896d-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
Content-type: application/json
Content-length: 180

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="5896d-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="5896d-150">Response</span></span>
<span data-ttu-id="5896d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5896d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 229

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "id": "d5a29103-9103-d5a2-0391-a2d50391a2d5",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
}
```





