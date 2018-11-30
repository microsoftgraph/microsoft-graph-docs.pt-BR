---
title: Criar deviceManagementScriptUserState
description: Crie um novo objeto de deviceManagementScriptUserState.
ms.openlocfilehash: 4d6aba6ae11f2d6250d20524a1e6f47e55bbda2a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037016"
---
# <a name="create-devicemanagementscriptuserstate"></a><span data-ttu-id="43767-103">Criar deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="43767-103">Create deviceManagementScriptUserState</span></span>

> <span data-ttu-id="43767-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="43767-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43767-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="43767-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43767-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="43767-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43767-107">Crie um novo objeto de [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="43767-107">Create a new [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="43767-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="43767-108">Prerequisites</span></span>
<span data-ttu-id="43767-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43767-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43767-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43767-111">Permission type</span></span>|<span data-ttu-id="43767-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="43767-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43767-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43767-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43767-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43767-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="43767-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43767-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43767-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43767-116">Not supported.</span></span>|
|<span data-ttu-id="43767-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43767-117">Application</span></span>|<span data-ttu-id="43767-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43767-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43767-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43767-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

## <a name="request-headers"></a><span data-ttu-id="43767-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43767-120">Request headers</span></span>
|<span data-ttu-id="43767-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="43767-121">Header</span></span>|<span data-ttu-id="43767-122">Valor</span><span class="sxs-lookup"><span data-stu-id="43767-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43767-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="43767-123">Authorization</span></span>|<span data-ttu-id="43767-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43767-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43767-125">Accept</span><span class="sxs-lookup"><span data-stu-id="43767-125">Accept</span></span>|<span data-ttu-id="43767-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43767-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43767-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43767-127">Request body</span></span>
<span data-ttu-id="43767-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementScriptUserState.</span><span class="sxs-lookup"><span data-stu-id="43767-128">In the request body, supply a JSON representation for the deviceManagementScriptUserState object.</span></span>

<span data-ttu-id="43767-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o deviceManagementScriptUserState.</span><span class="sxs-lookup"><span data-stu-id="43767-129">The following table shows the properties that are required when you create the deviceManagementScriptUserState.</span></span>

|<span data-ttu-id="43767-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43767-130">Property</span></span>|<span data-ttu-id="43767-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="43767-131">Type</span></span>|<span data-ttu-id="43767-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="43767-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43767-133">id</span><span class="sxs-lookup"><span data-stu-id="43767-133">id</span></span>|<span data-ttu-id="43767-134">String</span><span class="sxs-lookup"><span data-stu-id="43767-134">String</span></span>|<span data-ttu-id="43767-135">Chave da entidade de estado de usuário de script para gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="43767-135">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="43767-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="43767-136">successDeviceCount</span></span>|<span data-ttu-id="43767-137">Int32</span><span class="sxs-lookup"><span data-stu-id="43767-137">Int32</span></span>|<span data-ttu-id="43767-138">Contagem de dispositivo de sucesso para usuário específico.</span><span class="sxs-lookup"><span data-stu-id="43767-138">Success device count for specific user.</span></span>|
|<span data-ttu-id="43767-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="43767-139">errorDeviceCount</span></span>|<span data-ttu-id="43767-140">Int32</span><span class="sxs-lookup"><span data-stu-id="43767-140">Int32</span></span>|<span data-ttu-id="43767-141">Contagem de dispositivo de erro para usuário específico.</span><span class="sxs-lookup"><span data-stu-id="43767-141">Error device count for specific user.</span></span>|
|<span data-ttu-id="43767-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="43767-142">userPrincipalName</span></span>|<span data-ttu-id="43767-143">String</span><span class="sxs-lookup"><span data-stu-id="43767-143">String</span></span>|<span data-ttu-id="43767-144">Nome do princípio de usuário do usuário específico.</span><span class="sxs-lookup"><span data-stu-id="43767-144">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="43767-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="43767-145">Response</span></span>
<span data-ttu-id="43767-146">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43767-146">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43767-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43767-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="43767-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43767-148">Request</span></span>
<span data-ttu-id="43767-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="43767-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="43767-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="43767-150">Response</span></span>
<span data-ttu-id="43767-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43767-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





