---
title: Criar deviceManagementScriptAssignment
description: Crie um novo objeto de deviceManagementScriptAssignment.
ms.openlocfilehash: 7191b08e0517e219e8fcc97778424ed3e35540ea
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038527"
---
# <a name="create-devicemanagementscriptassignment"></a><span data-ttu-id="b6bcb-103">Criar deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="b6bcb-103">Create deviceManagementScriptAssignment</span></span>

> <span data-ttu-id="b6bcb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b6bcb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6bcb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b6bcb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6bcb-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b6bcb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6bcb-107">Crie um novo objeto de [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b6bcb-107">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b6bcb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6bcb-108">Prerequisites</span></span>
<span data-ttu-id="b6bcb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6bcb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6bcb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6bcb-111">Permission type</span></span>|<span data-ttu-id="b6bcb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b6bcb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6bcb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6bcb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6bcb-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6bcb-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b6bcb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6bcb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6bcb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6bcb-116">Not supported.</span></span>|
|<span data-ttu-id="b6bcb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6bcb-117">Application</span></span>|<span data-ttu-id="b6bcb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6bcb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6bcb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6bcb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="b6bcb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6bcb-120">Request headers</span></span>
|<span data-ttu-id="b6bcb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6bcb-121">Header</span></span>|<span data-ttu-id="b6bcb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b6bcb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6bcb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6bcb-123">Authorization</span></span>|<span data-ttu-id="b6bcb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6bcb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6bcb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b6bcb-125">Accept</span></span>|<span data-ttu-id="b6bcb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6bcb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6bcb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6bcb-127">Request body</span></span>
<span data-ttu-id="b6bcb-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementScriptAssignment.</span><span class="sxs-lookup"><span data-stu-id="b6bcb-128">In the request body, supply a JSON representation for the deviceManagementScriptAssignment object.</span></span>

<span data-ttu-id="b6bcb-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o deviceManagementScriptAssignment.</span><span class="sxs-lookup"><span data-stu-id="b6bcb-129">The following table shows the properties that are required when you create the deviceManagementScriptAssignment.</span></span>

|<span data-ttu-id="b6bcb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6bcb-130">Property</span></span>|<span data-ttu-id="b6bcb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6bcb-131">Type</span></span>|<span data-ttu-id="b6bcb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6bcb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6bcb-133">id</span><span class="sxs-lookup"><span data-stu-id="b6bcb-133">id</span></span>|<span data-ttu-id="b6bcb-134">String</span><span class="sxs-lookup"><span data-stu-id="b6bcb-134">String</span></span>|<span data-ttu-id="b6bcb-135">Chave da entidade de atribuição de grupo de script para gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b6bcb-135">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="b6bcb-136">destino</span><span class="sxs-lookup"><span data-stu-id="b6bcb-136">target</span></span>|[<span data-ttu-id="b6bcb-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b6bcb-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b6bcb-138">A Id de grupo do Active Directory do Windows Azure Pretendemos o script.</span><span class="sxs-lookup"><span data-stu-id="b6bcb-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="b6bcb-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6bcb-139">Response</span></span>
<span data-ttu-id="b6bcb-140">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6bcb-140">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6bcb-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6bcb-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="b6bcb-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6bcb-142">Request</span></span>
<span data-ttu-id="b6bcb-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6bcb-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="b6bcb-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6bcb-144">Response</span></span>
<span data-ttu-id="b6bcb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6bcb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





