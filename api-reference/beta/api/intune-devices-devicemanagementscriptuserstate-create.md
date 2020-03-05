---
title: Criar deviceManagementScriptUserState
description: Criar um novo objeto deviceManagementScriptUserState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3f0e4ddb8d64db0a9f1454b893b995a4d3ba2d29
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42469192"
---
# <a name="create-devicemanagementscriptuserstate"></a><span data-ttu-id="cab4b-103">Criar deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="cab4b-103">Create deviceManagementScriptUserState</span></span>

<span data-ttu-id="cab4b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cab4b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cab4b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cab4b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cab4b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cab4b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cab4b-107">Criar um novo objeto [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="cab4b-107">Create a new [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cab4b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cab4b-108">Prerequisites</span></span>
<span data-ttu-id="cab4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cab4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cab4b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cab4b-111">Permission type</span></span>|<span data-ttu-id="cab4b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cab4b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cab4b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cab4b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cab4b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cab4b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cab4b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cab4b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cab4b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cab4b-116">Not supported.</span></span>|
|<span data-ttu-id="cab4b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cab4b-117">Application</span></span>|<span data-ttu-id="cab4b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cab4b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cab4b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cab4b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

## <a name="request-headers"></a><span data-ttu-id="cab4b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cab4b-120">Request headers</span></span>
|<span data-ttu-id="cab4b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cab4b-121">Header</span></span>|<span data-ttu-id="cab4b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cab4b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cab4b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cab4b-123">Authorization</span></span>|<span data-ttu-id="cab4b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cab4b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cab4b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cab4b-125">Accept</span></span>|<span data-ttu-id="cab4b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cab4b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cab4b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cab4b-127">Request body</span></span>
<span data-ttu-id="cab4b-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementScriptUserState.</span><span class="sxs-lookup"><span data-stu-id="cab4b-128">In the request body, supply a JSON representation for the deviceManagementScriptUserState object.</span></span>

<span data-ttu-id="cab4b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementScriptUserState.</span><span class="sxs-lookup"><span data-stu-id="cab4b-129">The following table shows the properties that are required when you create the deviceManagementScriptUserState.</span></span>

|<span data-ttu-id="cab4b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cab4b-130">Property</span></span>|<span data-ttu-id="cab4b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cab4b-131">Type</span></span>|<span data-ttu-id="cab4b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cab4b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cab4b-133">id</span><span class="sxs-lookup"><span data-stu-id="cab4b-133">id</span></span>|<span data-ttu-id="cab4b-134">String</span><span class="sxs-lookup"><span data-stu-id="cab4b-134">String</span></span>|<span data-ttu-id="cab4b-135">Chave da entidade de estado do usuário de script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="cab4b-135">Key of the device management script user state entity.</span></span> <span data-ttu-id="cab4b-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cab4b-136">This property is read-only.</span></span>|
|<span data-ttu-id="cab4b-137">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cab4b-137">successDeviceCount</span></span>|<span data-ttu-id="cab4b-138">Int32</span><span class="sxs-lookup"><span data-stu-id="cab4b-138">Int32</span></span>|<span data-ttu-id="cab4b-139">Contagem de dispositivos com êxito para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="cab4b-139">Success device count for specific user.</span></span>|
|<span data-ttu-id="cab4b-140">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cab4b-140">errorDeviceCount</span></span>|<span data-ttu-id="cab4b-141">Int32</span><span class="sxs-lookup"><span data-stu-id="cab4b-141">Int32</span></span>|<span data-ttu-id="cab4b-142">Contagem de dispositivos de erro para usuário específico.</span><span class="sxs-lookup"><span data-stu-id="cab4b-142">Error device count for specific user.</span></span>|
|<span data-ttu-id="cab4b-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cab4b-143">userPrincipalName</span></span>|<span data-ttu-id="cab4b-144">String</span><span class="sxs-lookup"><span data-stu-id="cab4b-144">String</span></span>|<span data-ttu-id="cab4b-145">Nome principal do usuário do usuário específico.</span><span class="sxs-lookup"><span data-stu-id="cab4b-145">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="cab4b-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="cab4b-146">Response</span></span>
<span data-ttu-id="cab4b-147">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cab4b-147">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cab4b-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cab4b-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="cab4b-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cab4b-149">Request</span></span>
<span data-ttu-id="cab4b-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cab4b-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cab4b-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="cab4b-151">Response</span></span>
<span data-ttu-id="cab4b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cab4b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





