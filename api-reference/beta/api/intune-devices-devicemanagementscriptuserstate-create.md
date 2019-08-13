---
title: Criar deviceManagementScriptUserState
description: Criar um novo objeto deviceManagementScriptUserState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 44ae00acbd0b68feca4f8a611291670940d861ee
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36348834"
---
# <a name="create-devicemanagementscriptuserstate"></a><span data-ttu-id="8e927-103">Criar deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="8e927-103">Create deviceManagementScriptUserState</span></span>

> <span data-ttu-id="8e927-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8e927-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e927-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8e927-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e927-106">Criar um novo objeto [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="8e927-106">Create a new [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e927-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8e927-107">Prerequisites</span></span>
<span data-ttu-id="8e927-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e927-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e927-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e927-110">Permission type</span></span>|<span data-ttu-id="8e927-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8e927-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e927-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e927-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8e927-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e927-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8e927-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e927-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e927-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e927-115">Not supported.</span></span>|
|<span data-ttu-id="8e927-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e927-116">Application</span></span>|<span data-ttu-id="8e927-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e927-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e927-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e927-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

## <a name="request-headers"></a><span data-ttu-id="8e927-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e927-119">Request headers</span></span>
|<span data-ttu-id="8e927-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e927-120">Header</span></span>|<span data-ttu-id="8e927-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8e927-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e927-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e927-122">Authorization</span></span>|<span data-ttu-id="8e927-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e927-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e927-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8e927-124">Accept</span></span>|<span data-ttu-id="8e927-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8e927-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e927-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e927-126">Request body</span></span>
<span data-ttu-id="8e927-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementScriptUserState.</span><span class="sxs-lookup"><span data-stu-id="8e927-127">In the request body, supply a JSON representation for the deviceManagementScriptUserState object.</span></span>

<span data-ttu-id="8e927-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementScriptUserState.</span><span class="sxs-lookup"><span data-stu-id="8e927-128">The following table shows the properties that are required when you create the deviceManagementScriptUserState.</span></span>

|<span data-ttu-id="8e927-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e927-129">Property</span></span>|<span data-ttu-id="8e927-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e927-130">Type</span></span>|<span data-ttu-id="8e927-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e927-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e927-132">id</span><span class="sxs-lookup"><span data-stu-id="8e927-132">id</span></span>|<span data-ttu-id="8e927-133">String</span><span class="sxs-lookup"><span data-stu-id="8e927-133">String</span></span>|<span data-ttu-id="8e927-134">Chave da entidade de estado do usuário de script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8e927-134">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="8e927-135">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8e927-135">successDeviceCount</span></span>|<span data-ttu-id="8e927-136">Int32</span><span class="sxs-lookup"><span data-stu-id="8e927-136">Int32</span></span>|<span data-ttu-id="8e927-137">Contagem de dispositivos com êxito para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="8e927-137">Success device count for specific user.</span></span>|
|<span data-ttu-id="8e927-138">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8e927-138">errorDeviceCount</span></span>|<span data-ttu-id="8e927-139">Int32</span><span class="sxs-lookup"><span data-stu-id="8e927-139">Int32</span></span>|<span data-ttu-id="8e927-140">Contagem de dispositivos de erro para usuário específico.</span><span class="sxs-lookup"><span data-stu-id="8e927-140">Error device count for specific user.</span></span>|
|<span data-ttu-id="8e927-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8e927-141">userPrincipalName</span></span>|<span data-ttu-id="8e927-142">String</span><span class="sxs-lookup"><span data-stu-id="8e927-142">String</span></span>|<span data-ttu-id="8e927-143">Nome principal do usuário do usuário específico.</span><span class="sxs-lookup"><span data-stu-id="8e927-143">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="8e927-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e927-144">Response</span></span>
<span data-ttu-id="8e927-145">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e927-145">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e927-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e927-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e927-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e927-147">Request</span></span>
<span data-ttu-id="8e927-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e927-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
Content-type: application/json
Content-length: 180

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="8e927-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e927-149">Response</span></span>
<span data-ttu-id="8e927-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e927-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






