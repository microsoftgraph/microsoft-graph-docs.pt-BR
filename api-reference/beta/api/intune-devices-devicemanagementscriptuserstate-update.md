---
title: Atualizar deviceManagementScriptUserState
description: Atualize as propriedades de um objeto deviceManagementScriptUserState.
author: tfitzmac
ms.openlocfilehash: 4a2601df84b022d13fd45ef3c506a4ee229fe6ad
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307830"
---
# <a name="update-devicemanagementscriptuserstate"></a><span data-ttu-id="7e241-103">Atualizar deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="7e241-103">Update deviceManagementScriptUserState</span></span>

> <span data-ttu-id="7e241-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7e241-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e241-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7e241-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7e241-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7e241-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e241-107">Atualize as propriedades de um objeto [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="7e241-107">Update the properties of a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7e241-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7e241-108">Prerequisites</span></span>
<span data-ttu-id="7e241-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e241-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e241-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e241-111">Permission type</span></span>|<span data-ttu-id="7e241-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7e241-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e241-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e241-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7e241-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e241-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7e241-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e241-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e241-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e241-116">Not supported.</span></span>|
|<span data-ttu-id="7e241-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e241-117">Application</span></span>|<span data-ttu-id="7e241-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e241-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e241-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e241-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

## <a name="request-headers"></a><span data-ttu-id="7e241-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e241-120">Request headers</span></span>
|<span data-ttu-id="7e241-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7e241-121">Header</span></span>|<span data-ttu-id="7e241-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7e241-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e241-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e241-123">Authorization</span></span>|<span data-ttu-id="7e241-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e241-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e241-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7e241-125">Accept</span></span>|<span data-ttu-id="7e241-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7e241-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e241-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e241-127">Request body</span></span>
<span data-ttu-id="7e241-128">No corpo da solicitação, fornece uma representação JSON para o objeto [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="7e241-128">In the request body, supply a JSON representation for the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

<span data-ttu-id="7e241-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span><span class="sxs-lookup"><span data-stu-id="7e241-129">The following table shows the properties that are required when you create the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>

|<span data-ttu-id="7e241-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7e241-130">Property</span></span>|<span data-ttu-id="7e241-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e241-131">Type</span></span>|<span data-ttu-id="7e241-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e241-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e241-133">id</span><span class="sxs-lookup"><span data-stu-id="7e241-133">id</span></span>|<span data-ttu-id="7e241-134">String</span><span class="sxs-lookup"><span data-stu-id="7e241-134">String</span></span>|<span data-ttu-id="7e241-135">Chave da entidade de estado de usuário de script para gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7e241-135">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="7e241-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7e241-136">successDeviceCount</span></span>|<span data-ttu-id="7e241-137">Int32</span><span class="sxs-lookup"><span data-stu-id="7e241-137">Int32</span></span>|<span data-ttu-id="7e241-138">Contagem de dispositivo de sucesso para usuário específico.</span><span class="sxs-lookup"><span data-stu-id="7e241-138">Success device count for specific user.</span></span>|
|<span data-ttu-id="7e241-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7e241-139">errorDeviceCount</span></span>|<span data-ttu-id="7e241-140">Int32</span><span class="sxs-lookup"><span data-stu-id="7e241-140">Int32</span></span>|<span data-ttu-id="7e241-141">Contagem de dispositivo de erro para usuário específico.</span><span class="sxs-lookup"><span data-stu-id="7e241-141">Error device count for specific user.</span></span>|
|<span data-ttu-id="7e241-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7e241-142">userPrincipalName</span></span>|<span data-ttu-id="7e241-143">String</span><span class="sxs-lookup"><span data-stu-id="7e241-143">String</span></span>|<span data-ttu-id="7e241-144">Nome do princípio de usuário do usuário específico.</span><span class="sxs-lookup"><span data-stu-id="7e241-144">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="7e241-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e241-145">Response</span></span>
<span data-ttu-id="7e241-146">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e241-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e241-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e241-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="7e241-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e241-148">Request</span></span>
<span data-ttu-id="7e241-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e241-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
Content-type: application/json
Content-length: 110

{
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="7e241-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e241-150">Response</span></span>
<span data-ttu-id="7e241-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7e241-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





