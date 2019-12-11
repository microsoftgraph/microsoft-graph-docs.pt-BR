---
title: Criar deviceManagementScriptUserState
description: Criar um novo objeto deviceManagementScriptUserState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b63be2874f9466a97fd4c2c867f85d80c2e4252a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944908"
---
# <a name="create-devicemanagementscriptuserstate"></a><span data-ttu-id="b7b9e-103">Criar deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="b7b9e-103">Create deviceManagementScriptUserState</span></span>

> <span data-ttu-id="b7b9e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b7b9e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7b9e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b7b9e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7b9e-106">Criar um novo objeto [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="b7b9e-106">Create a new [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7b9e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b7b9e-107">Prerequisites</span></span>
<span data-ttu-id="b7b9e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7b9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7b9e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7b9e-110">Permission type</span></span>|<span data-ttu-id="b7b9e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b7b9e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7b9e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7b9e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b7b9e-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7b9e-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b7b9e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7b9e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7b9e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7b9e-115">Not supported.</span></span>|
|<span data-ttu-id="b7b9e-116">Application</span><span class="sxs-lookup"><span data-stu-id="b7b9e-116">Application</span></span>|<span data-ttu-id="b7b9e-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7b9e-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7b9e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7b9e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

## <a name="request-headers"></a><span data-ttu-id="b7b9e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7b9e-119">Request headers</span></span>
|<span data-ttu-id="b7b9e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b7b9e-120">Header</span></span>|<span data-ttu-id="b7b9e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b7b9e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7b9e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7b9e-122">Authorization</span></span>|<span data-ttu-id="b7b9e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7b9e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7b9e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b7b9e-124">Accept</span></span>|<span data-ttu-id="b7b9e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b7b9e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7b9e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7b9e-126">Request body</span></span>
<span data-ttu-id="b7b9e-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementScriptUserState.</span><span class="sxs-lookup"><span data-stu-id="b7b9e-127">In the request body, supply a JSON representation for the deviceManagementScriptUserState object.</span></span>

<span data-ttu-id="b7b9e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementScriptUserState.</span><span class="sxs-lookup"><span data-stu-id="b7b9e-128">The following table shows the properties that are required when you create the deviceManagementScriptUserState.</span></span>

|<span data-ttu-id="b7b9e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7b9e-129">Property</span></span>|<span data-ttu-id="b7b9e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7b9e-130">Type</span></span>|<span data-ttu-id="b7b9e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7b9e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7b9e-132">id</span><span class="sxs-lookup"><span data-stu-id="b7b9e-132">id</span></span>|<span data-ttu-id="b7b9e-133">String</span><span class="sxs-lookup"><span data-stu-id="b7b9e-133">String</span></span>|<span data-ttu-id="b7b9e-134">Chave da entidade de estado do usuário de script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b7b9e-134">Key of the device management script user state entity.</span></span> <span data-ttu-id="b7b9e-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b7b9e-135">This property is read-only.</span></span>|
|<span data-ttu-id="b7b9e-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b7b9e-136">successDeviceCount</span></span>|<span data-ttu-id="b7b9e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b7b9e-137">Int32</span></span>|<span data-ttu-id="b7b9e-138">Contagem de dispositivos com êxito para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="b7b9e-138">Success device count for specific user.</span></span>|
|<span data-ttu-id="b7b9e-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b7b9e-139">errorDeviceCount</span></span>|<span data-ttu-id="b7b9e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b7b9e-140">Int32</span></span>|<span data-ttu-id="b7b9e-141">Contagem de dispositivos de erro para usuário específico.</span><span class="sxs-lookup"><span data-stu-id="b7b9e-141">Error device count for specific user.</span></span>|
|<span data-ttu-id="b7b9e-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b7b9e-142">userPrincipalName</span></span>|<span data-ttu-id="b7b9e-143">String</span><span class="sxs-lookup"><span data-stu-id="b7b9e-143">String</span></span>|<span data-ttu-id="b7b9e-144">Nome principal do usuário do usuário específico.</span><span class="sxs-lookup"><span data-stu-id="b7b9e-144">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="b7b9e-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7b9e-145">Response</span></span>
<span data-ttu-id="b7b9e-146">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7b9e-146">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7b9e-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7b9e-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7b9e-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7b9e-148">Request</span></span>
<span data-ttu-id="b7b9e-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7b9e-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates
Content-type: application/json
Content-length: 180

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="b7b9e-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7b9e-150">Response</span></span>
<span data-ttu-id="b7b9e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7b9e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





