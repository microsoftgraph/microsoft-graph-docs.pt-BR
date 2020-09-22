---
title: Atualizar deviceManagementScriptUserState
description: Atualiza as propriedades de um objeto deviceManagementScriptUserState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 180f39c2cab106e7fd83846c8f84786b13944a75
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994663"
---
# <a name="update-devicemanagementscriptuserstate"></a><span data-ttu-id="6cafc-103">Atualizar deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="6cafc-103">Update deviceManagementScriptUserState</span></span>

<span data-ttu-id="6cafc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cafc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6cafc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6cafc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6cafc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6cafc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cafc-107">Atualiza as propriedades de um objeto [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="6cafc-107">Update the properties of a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6cafc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6cafc-108">Prerequisites</span></span>
<span data-ttu-id="6cafc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cafc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cafc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6cafc-111">Permission type</span></span>|<span data-ttu-id="6cafc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6cafc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cafc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6cafc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6cafc-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cafc-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6cafc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6cafc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cafc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cafc-116">Not supported.</span></span>|
|<span data-ttu-id="6cafc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6cafc-117">Application</span></span>|<span data-ttu-id="6cafc-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cafc-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cafc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6cafc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

## <a name="request-headers"></a><span data-ttu-id="6cafc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6cafc-120">Request headers</span></span>
|<span data-ttu-id="6cafc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6cafc-121">Header</span></span>|<span data-ttu-id="6cafc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6cafc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cafc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6cafc-123">Authorization</span></span>|<span data-ttu-id="6cafc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6cafc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cafc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6cafc-125">Accept</span></span>|<span data-ttu-id="6cafc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6cafc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cafc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6cafc-127">Request body</span></span>
<span data-ttu-id="6cafc-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="6cafc-128">In the request body, supply a JSON representation for the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

<span data-ttu-id="6cafc-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span><span class="sxs-lookup"><span data-stu-id="6cafc-129">The following table shows the properties that are required when you create the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>

|<span data-ttu-id="6cafc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6cafc-130">Property</span></span>|<span data-ttu-id="6cafc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6cafc-131">Type</span></span>|<span data-ttu-id="6cafc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cafc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cafc-133">id</span><span class="sxs-lookup"><span data-stu-id="6cafc-133">id</span></span>|<span data-ttu-id="6cafc-134">String</span><span class="sxs-lookup"><span data-stu-id="6cafc-134">String</span></span>|<span data-ttu-id="6cafc-135">Chave da entidade de estado do usuário de script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="6cafc-135">Key of the device management script user state entity.</span></span> <span data-ttu-id="6cafc-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6cafc-136">This property is read-only.</span></span>|
|<span data-ttu-id="6cafc-137">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6cafc-137">successDeviceCount</span></span>|<span data-ttu-id="6cafc-138">Int32</span><span class="sxs-lookup"><span data-stu-id="6cafc-138">Int32</span></span>|<span data-ttu-id="6cafc-139">Contagem de dispositivos com êxito para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="6cafc-139">Success device count for specific user.</span></span>|
|<span data-ttu-id="6cafc-140">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6cafc-140">errorDeviceCount</span></span>|<span data-ttu-id="6cafc-141">Int32</span><span class="sxs-lookup"><span data-stu-id="6cafc-141">Int32</span></span>|<span data-ttu-id="6cafc-142">Contagem de dispositivos de erro para usuário específico.</span><span class="sxs-lookup"><span data-stu-id="6cafc-142">Error device count for specific user.</span></span>|
|<span data-ttu-id="6cafc-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6cafc-143">userPrincipalName</span></span>|<span data-ttu-id="6cafc-144">String</span><span class="sxs-lookup"><span data-stu-id="6cafc-144">String</span></span>|<span data-ttu-id="6cafc-145">Nome principal do usuário do usuário específico.</span><span class="sxs-lookup"><span data-stu-id="6cafc-145">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="6cafc-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cafc-146">Response</span></span>
<span data-ttu-id="6cafc-147">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6cafc-147">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cafc-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6cafc-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cafc-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6cafc-149">Request</span></span>
<span data-ttu-id="6cafc-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6cafc-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6cafc-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cafc-151">Response</span></span>
<span data-ttu-id="6cafc-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6cafc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






