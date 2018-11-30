---
title: Atualizar deviceManagementScriptAssignment
description: Atualize as propriedades de um objeto deviceManagementScriptAssignment.
ms.openlocfilehash: c69cc71181eb1a46a3505e474991079e5e196590
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040463"
---
# <a name="update-devicemanagementscriptassignment"></a><span data-ttu-id="9829a-103">Atualizar deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="9829a-103">Update deviceManagementScriptAssignment</span></span>

> <span data-ttu-id="9829a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9829a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9829a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9829a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9829a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9829a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9829a-107">Atualize as propriedades de um objeto [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="9829a-107">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9829a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9829a-108">Prerequisites</span></span>
<span data-ttu-id="9829a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9829a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9829a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9829a-111">Permission type</span></span>|<span data-ttu-id="9829a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9829a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9829a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9829a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9829a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9829a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9829a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9829a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9829a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9829a-116">Not supported.</span></span>|
|<span data-ttu-id="9829a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9829a-117">Application</span></span>|<span data-ttu-id="9829a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9829a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9829a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9829a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="9829a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9829a-120">Request headers</span></span>
|<span data-ttu-id="9829a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9829a-121">Header</span></span>|<span data-ttu-id="9829a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9829a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9829a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9829a-123">Authorization</span></span>|<span data-ttu-id="9829a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9829a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9829a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9829a-125">Accept</span></span>|<span data-ttu-id="9829a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9829a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9829a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9829a-127">Request body</span></span>
<span data-ttu-id="9829a-128">No corpo da solicitação, fornece uma representação JSON para o objeto [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="9829a-128">In the request body, supply a JSON representation for the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

<span data-ttu-id="9829a-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9829a-129">The following table shows the properties that are required when you create the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>

|<span data-ttu-id="9829a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9829a-130">Property</span></span>|<span data-ttu-id="9829a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9829a-131">Type</span></span>|<span data-ttu-id="9829a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9829a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9829a-133">id</span><span class="sxs-lookup"><span data-stu-id="9829a-133">id</span></span>|<span data-ttu-id="9829a-134">String</span><span class="sxs-lookup"><span data-stu-id="9829a-134">String</span></span>|<span data-ttu-id="9829a-135">Chave da entidade de atribuição de grupo de script para gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9829a-135">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="9829a-136">destino</span><span class="sxs-lookup"><span data-stu-id="9829a-136">target</span></span>|[<span data-ttu-id="9829a-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9829a-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9829a-138">A Id de grupo do Active Directory do Windows Azure Pretendemos o script.</span><span class="sxs-lookup"><span data-stu-id="9829a-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="9829a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="9829a-139">Response</span></span>
<span data-ttu-id="9829a-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9829a-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9829a-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9829a-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="9829a-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9829a-142">Request</span></span>
<span data-ttu-id="9829a-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9829a-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="9829a-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="9829a-144">Response</span></span>
<span data-ttu-id="9829a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9829a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





