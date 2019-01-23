---
title: Atualizar deviceManagementScriptUserState
description: Atualize as propriedades de um objeto deviceManagementScriptUserState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c2f25746d54bf1d7c8f9a03fcefc9cecb826de68
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419937"
---
# <a name="update-devicemanagementscriptuserstate"></a><span data-ttu-id="aa5a6-103">Atualizar deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="aa5a6-103">Update deviceManagementScriptUserState</span></span>

> <span data-ttu-id="aa5a6-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="aa5a6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="aa5a6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="aa5a6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aa5a6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="aa5a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa5a6-107">Atualize as propriedades de um objeto [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="aa5a6-107">Update the properties of a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa5a6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aa5a6-108">Prerequisites</span></span>
<span data-ttu-id="aa5a6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="aa5a6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="aa5a6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa5a6-111">Permission type</span></span>|<span data-ttu-id="aa5a6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aa5a6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa5a6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa5a6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aa5a6-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa5a6-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="aa5a6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa5a6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa5a6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa5a6-116">Not supported.</span></span>|
|<span data-ttu-id="aa5a6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa5a6-117">Application</span></span>|<span data-ttu-id="aa5a6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa5a6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa5a6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa5a6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

## <a name="request-headers"></a><span data-ttu-id="aa5a6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa5a6-120">Request headers</span></span>
|<span data-ttu-id="aa5a6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aa5a6-121">Header</span></span>|<span data-ttu-id="aa5a6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="aa5a6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa5a6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa5a6-123">Authorization</span></span>|<span data-ttu-id="aa5a6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa5a6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa5a6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aa5a6-125">Accept</span></span>|<span data-ttu-id="aa5a6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aa5a6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa5a6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa5a6-127">Request body</span></span>
<span data-ttu-id="aa5a6-128">No corpo da solicitação, fornece uma representação JSON para o objeto [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="aa5a6-128">In the request body, supply a JSON representation for the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

<span data-ttu-id="aa5a6-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span><span class="sxs-lookup"><span data-stu-id="aa5a6-129">The following table shows the properties that are required when you create the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>

|<span data-ttu-id="aa5a6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aa5a6-130">Property</span></span>|<span data-ttu-id="aa5a6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa5a6-131">Type</span></span>|<span data-ttu-id="aa5a6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa5a6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa5a6-133">id</span><span class="sxs-lookup"><span data-stu-id="aa5a6-133">id</span></span>|<span data-ttu-id="aa5a6-134">String</span><span class="sxs-lookup"><span data-stu-id="aa5a6-134">String</span></span>|<span data-ttu-id="aa5a6-135">Chave da entidade de estado de usuário de script para gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aa5a6-135">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="aa5a6-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aa5a6-136">successDeviceCount</span></span>|<span data-ttu-id="aa5a6-137">Int32</span><span class="sxs-lookup"><span data-stu-id="aa5a6-137">Int32</span></span>|<span data-ttu-id="aa5a6-138">Contagem de dispositivo de sucesso para usuário específico.</span><span class="sxs-lookup"><span data-stu-id="aa5a6-138">Success device count for specific user.</span></span>|
|<span data-ttu-id="aa5a6-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aa5a6-139">errorDeviceCount</span></span>|<span data-ttu-id="aa5a6-140">Int32</span><span class="sxs-lookup"><span data-stu-id="aa5a6-140">Int32</span></span>|<span data-ttu-id="aa5a6-141">Contagem de dispositivo de erro para usuário específico.</span><span class="sxs-lookup"><span data-stu-id="aa5a6-141">Error device count for specific user.</span></span>|
|<span data-ttu-id="aa5a6-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="aa5a6-142">userPrincipalName</span></span>|<span data-ttu-id="aa5a6-143">String</span><span class="sxs-lookup"><span data-stu-id="aa5a6-143">String</span></span>|<span data-ttu-id="aa5a6-144">Nome do princípio de usuário do usuário específico.</span><span class="sxs-lookup"><span data-stu-id="aa5a6-144">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="aa5a6-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa5a6-145">Response</span></span>
<span data-ttu-id="aa5a6-146">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa5a6-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa5a6-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa5a6-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa5a6-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa5a6-148">Request</span></span>
<span data-ttu-id="aa5a6-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa5a6-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aa5a6-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa5a6-150">Response</span></span>
<span data-ttu-id="aa5a6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa5a6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




