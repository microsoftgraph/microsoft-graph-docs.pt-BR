---
title: Atualizar deviceManagementScriptUserState
description: Atualiza as propriedades de um objeto deviceManagementScriptUserState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2891bcf9b3b5614d4b7302339ebf05e6cc786d10
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35981483"
---
# <a name="update-devicemanagementscriptuserstate"></a><span data-ttu-id="8a580-103">Atualizar deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="8a580-103">Update deviceManagementScriptUserState</span></span>

> <span data-ttu-id="8a580-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8a580-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a580-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8a580-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a580-106">Atualiza as propriedades de um objeto [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="8a580-106">Update the properties of a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a580-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8a580-107">Prerequisites</span></span>
<span data-ttu-id="8a580-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a580-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a580-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a580-110">Permission type</span></span>|<span data-ttu-id="8a580-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8a580-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a580-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a580-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8a580-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a580-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8a580-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a580-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a580-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a580-115">Not supported.</span></span>|
|<span data-ttu-id="8a580-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a580-116">Application</span></span>|<span data-ttu-id="8a580-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a580-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a580-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a580-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

## <a name="request-headers"></a><span data-ttu-id="8a580-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a580-119">Request headers</span></span>
|<span data-ttu-id="8a580-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8a580-120">Header</span></span>|<span data-ttu-id="8a580-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8a580-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a580-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a580-122">Authorization</span></span>|<span data-ttu-id="8a580-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a580-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a580-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8a580-124">Accept</span></span>|<span data-ttu-id="8a580-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8a580-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a580-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a580-126">Request body</span></span>
<span data-ttu-id="8a580-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="8a580-127">In the request body, supply a JSON representation for the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

<span data-ttu-id="8a580-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span><span class="sxs-lookup"><span data-stu-id="8a580-128">The following table shows the properties that are required when you create the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>

|<span data-ttu-id="8a580-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8a580-129">Property</span></span>|<span data-ttu-id="8a580-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a580-130">Type</span></span>|<span data-ttu-id="8a580-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a580-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a580-132">id</span><span class="sxs-lookup"><span data-stu-id="8a580-132">id</span></span>|<span data-ttu-id="8a580-133">String</span><span class="sxs-lookup"><span data-stu-id="8a580-133">String</span></span>|<span data-ttu-id="8a580-134">Chave da entidade de estado do usuário de script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8a580-134">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="8a580-135">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8a580-135">successDeviceCount</span></span>|<span data-ttu-id="8a580-136">Int32</span><span class="sxs-lookup"><span data-stu-id="8a580-136">Int32</span></span>|<span data-ttu-id="8a580-137">Contagem de dispositivos com êxito para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="8a580-137">Success device count for specific user.</span></span>|
|<span data-ttu-id="8a580-138">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8a580-138">errorDeviceCount</span></span>|<span data-ttu-id="8a580-139">Int32</span><span class="sxs-lookup"><span data-stu-id="8a580-139">Int32</span></span>|<span data-ttu-id="8a580-140">Contagem de dispositivos de erro para usuário específico.</span><span class="sxs-lookup"><span data-stu-id="8a580-140">Error device count for specific user.</span></span>|
|<span data-ttu-id="8a580-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8a580-141">userPrincipalName</span></span>|<span data-ttu-id="8a580-142">String</span><span class="sxs-lookup"><span data-stu-id="8a580-142">String</span></span>|<span data-ttu-id="8a580-143">Nome principal do usuário do usuário específico.</span><span class="sxs-lookup"><span data-stu-id="8a580-143">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="8a580-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a580-144">Response</span></span>
<span data-ttu-id="8a580-145">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a580-145">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a580-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a580-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a580-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a580-147">Request</span></span>
<span data-ttu-id="8a580-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a580-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
Content-type: application/json
Content-length: 180

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="8a580-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a580-149">Response</span></span>
<span data-ttu-id="8a580-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8a580-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





